<% configRef "..\\..\\configs\\index\\index_nodejs.yml" %>
<% include "..\\..\\data\\platform_data.md" %>
---
############################# Static ############################
layout: "landing"
date: <% date "utcnow" %>
draft: false

lang: <% lower ( get "lang") %>
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "<% "{index-content-nodejs-java.head_title}" %>"
head_description: "<% "{index-content-nodejs-java.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-nodejs-java.title}" %>"
description: "<% "{index-content-nodejs-java.description}" %>"
words:
  for: "<% "{index-content.words_for}" %>"

actions:
  main: "<% "{index-content-nodejs-java.actions_main}" %>"
  main_link: "<% get "PackageUrl" %>"
  alt: "<% "{index-content.actions.alt}" %>"
  alt_link: "<% get "PricesUrl" %>"
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description}" %>"

release:
  title: "<% "{index-content.release_title}" %>"
  notes: "<% "{index-content.release_notes}" %>"
  downloads: "<% "{index-content.release_downloads}" %>"
  link: "<% "{products.nodejs-java.release_downloads}" %>"

code:
  title: "<% "{index-content-nodejs-java.code_title}" %>"
  more: "<% "{index-content.code_more}" %>"
  more_link: "<% dict "products.nodejs-java.more_link" %>"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // <% "{index-content.code_comment_1}" %>
    const template = "chart_template.docx";

    // <% "{index-content.code_comment_2}" %>
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // <% "{index-content.code_comment_3}" %>
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // <% "{index-content.code_comment_4}" %>
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // <% "{index-content.code_comment_5}" %>
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "<% "{index-content.overview_title}" %>"
  description: "<% "{index-content-nodejs-java.overview_description}" %>"
  features:
    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_1.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_1.description}" %>"

    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_2.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_2.description}" %>"

    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_3.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_3.description}" %>"

############################# Platforms ############################
platforms:
  enable: true
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content-nodejs-java.platforms_description}" %>"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "<% "{index-content.formats_title}" %>"
  description: |
    <% "{index-content-nodejs-java.formats_description}" %>
  groups:
    # group loop
    - color: "green"
      content: |
        ### <% "{index-content.formats_groups.title_1}" %>
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### <% "{index-content.formats_groups.title_2}" %>
        * **<% "{index-content.formats_groups.format_portable}" %>:** PDF
        * **<% "{index-content.formats_groups.format_images}" %>:** SVG, TIFF
        * **<% "{index-content.formats_groups.format_other_office}" %>:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### <% "{index-content.formats_groups.title_3}" %>
        * **<% "{index-content.formats_groups.format_web}" %>:** HTML, MHTML
        * **<% "{index-content.formats_groups.format_emails}" %>:** EML, MSG, EMLX
        * **<% "{index-content.formats_groups.format_other}" %>:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "<% "{index-content-nodejs-java.features.title}" %>"
  description: "<% "{index-content-nodejs-java.features.description}" %>"

  items:
    # feature loop
    - icon: "preview"
      title: "<% "{index-content-nodejs-java.features.feature_1.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_1.content}" %>"

    # feature loop
    - icon: "manipulate"
      title: "<% "{index-content-nodejs-java.features.feature_2.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_2.content}" %>"

    # feature loop
    - icon: "two_pages"
      title: "<% "{index-content-nodejs-java.features.feature_3.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_3.content}" %>"

    # feature loop
    - icon: "document_settings"
      title: "<% "{index-content-nodejs-java.features.feature_4.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_4.content}" %>"

    # feature loop
    - icon: "text"
      title: "<% "{index-content-nodejs-java.features.feature_5.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_5.content}" %>"

    # feature loop
    - icon: "add"
      title: "<% "{index-content-nodejs-java.features.feature_6.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_6.content}" %>"

    # feature loop
    - icon: "manipulate"
      title: "<% "{index-content-nodejs-java.features.feature_7.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_7.content}" %>"

    # feature loop
    - icon: "convert"
      title: "<% "{index-content-nodejs-java.features.feature_8.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_8.content}" %>"

    # feature loop
    - icon: "update"
      title: "<% "{index-content-nodejs-java.features.feature_9.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_9.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.title}" %>"
  description: "<% "{index-content-nodejs-java.code_samples_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content-nodejs-java.code_title_sample_1}" %>"
      content: |
        <% "{index-content-nodejs-java.code_samples_sample_1_content_1}" %> <% "{index-content-nodejs-java.code_samples_sample_1_content_2}" %>
        {{< landing/code title="<% "{index-content-nodejs-java.code_title_sample_1}" %>">}}
        ```javascript {style=abap}
        // <% "{index-content.code_samples.sample_1.comment_1}" %>
        // <% "{index-content.code_samples.sample_1.comment_2}" %>
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // <% "{index-content.code_samples.sample_1.comment_3}" %>
        const template = "Bulleted List Template.docx";

        // <% "{index-content.code_samples.sample_1.comment_4}" %>
        const result = "Result Report.docx"

        // <% "{index-content.code_samples.sample_1.comment_5}" %>
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // <% "{index-content.code_samples.sample_1.comment_6}" %>
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "<% "{index-content-nodejs-java.code_title_sample_2}" %>"
      content: |
        <% "{index-content-nodejs-java.code_samples_sample_2_content_1}" %> <% "{index-content-nodejs-java.code_samples_sample_2_content_2}" %>
        {{< landing/code title="<% "{index-content-nodejs-java.code_title_sample_2}" %>">}}
        ```javascript {style=abap} 
        // <% "{index-content.code_samples.sample_2.comment_1}" %>
        // <% "{index-content.code_samples.sample_2.comment_2}" %> <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // <% "{index-content.code_samples.sample_2.comment_3}" %>
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // <% "{index-content.code_samples.sample_2.comment_4}" %>
        const template = "Pie Chart Template.pptx";

        // <% "{index-content.code_samples.sample_2.comment_5}" %>
        const result = "Result Report.pptx"

        // <% "{index-content.code_samples.sample_2.comment_6}" %>
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // <% "{index-content.code_samples.sample_2.comment_7}" %>
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---