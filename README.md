# ojs3-import-xml-template
Own examples of xml files for importing articles and releases using the Native XML Plugin in [Open Journal Systems 3](https://pkp.sfu.ca/ojs/). Based on examples of export articles and issues in OJS's native XML format and examples in [PKP Community Forum](https://forum.pkp.sfu.ca/).

Files with comments for manual or programmatic (database or scripts) data formatting.

### One Article with/without embed base64 file
```one-article-with-embed-files.xml``` - next commit.

```one-article-without-embed-file.xml``` — A quick and simple example of article markup for import. First, the article is import without embedded filesand then through **Submissions Archives** added the necessary files to the article.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE issue PUBLIC "-//PKP//OJS Articles and Issues XML//EN" "http://pkp.sfu.ca/ojs/dtds/native.dtd">
<article xmlns="http://pkp.sfu.ca" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" locale="uk_UA" date_submitted="2018-01-12" date_published="2015-05-06" section_ref="articles" seq="1" access_status="0" xsi:schemaLocation="http://pkp.sfu.ca native.xsd" stage="production">
  <!-- date_submitted= Curent date, date_published= Date of publishing Issue, section_ref= Section in Issue  -->
    <id type="internal" advice="ignore"><!-- Next ID from OJS or blank --></id>
    <title locale="en_US"><!-- Issue title in English or blank --></title>
    <title locale="uk_UA"><!-- Article title in Ukrainian or other non-English languages --></title>
    <abstract locale="en_US"><!-- Abstract in English or blank --></abstract>
    <abstract locale="uk_UA"><!-- Abstract in Ukrainian or other non-English languages --></abstract>
    <copyrightHolder locale="en_US"><!-- Copyright Holder in English or blank --></copyrightHolder>
    <copyrightHolder locale="uk_UA"><!-- Copyright Holder in Ukrainian or other non-English languages --></copyrightHolder>
    <copyrightYear><!-- Copyright Year --></copyrightYear>
    <keywords locale="en_US">
        <keyword><!-- Article Keyword in English --></keyword>
        <keyword><!-- Article Keyword in English --></keyword>
    </keywords>
    <keywords locale="uk_UA">
        <keyword><!-- Keyword in Ukrainian or other non-English languages --></keyword>
        <keyword><!-- Keyword in Ukrainian or other non-English languages --></keyword>
    </keywords>
    <authors xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://pkp.sfu.ca native.xsd">
      <author include_in_browse="true" user_group_ref="Author">
  <!-- user_group_ref= User group in your system for this Author -->
        <firstname><!-- First name or Name and patronymic --></firstname>
        <lastname><!-- Last name --></lastname>
        <affiliation locale="en_US"><!-- Affiliation in English --></affiliation>
        <affiliation locale="uk_UA"><!-- Affiliation in Ukrainian or other non-English languages --></affiliation>
        <country><!-- Country code, for example: UA --></country>
        <email><!-- Author Email --></email>
        <orcid><!-- ORCiD full URL, for example: https://orcid.org/XXXX-XXXX-XXXX-XXXX --></orcid>
        <biography locale="en_US"><!-- About Author or Supervisor Additional Information in English --></biography>
        <biography locale="uk_UA"><!-- About Author or Supervisor Additional Information in Ukrainian or other non-English languages --></biography>
      </author>
    </authors>
    <issue_identification>
      <number><!-- Issue number, for example: 1 --></number>
      <year><!-- Year of issues publication --></year>
      <title locale="en_US"><!-- Issue title in English --></title>
      <title locale="uk_UA"><!-- Issue title in Ukrainian or other non-English languages --></title>
    </issue_identification>
    <pages><!-- Pages of article, for example: 164-170 --></pages>
  </article>
```

### Blank dir
The directory **blank** contains empty blank files for importing article or issues. 
The issues file is an example for formatting a group of authors.

