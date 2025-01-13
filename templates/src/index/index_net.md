<% configRef "..\\..\\configs\\index\\index_net.yml" %>
<% include "..\\..\\data\\platform_data.md" %>
---
############################# Static ############################
layout: "landing"
date: <% date "utcnow" %>
draft: false

lang: <% lower ( get "lang") %>
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

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
head_title: "<% "{index-content-net.head_title}" %>"
head_description: "<% "{index-content-net.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-net.title}" %>"
description: "<% "{index-content-net.description}" %>"
words:
  for: "<% "{index-content.words_for}" %>"

actions:
  main: "<% "{index-content-net.actions_main}" %>"
  main_link: "<% get "PackageUrl" %>"
  alt: "<% "{index-content.actions.alt}" %>"
  alt_link: "<% get "PricesUrl" %>"
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description}" %>"

release:
  title: "<% "{index-content.release_title}" %>"
  notes: "<% "{index-content.release_notes}" %>"
  downloads: "<% "{index-content.release_downloads}" %>"
  link: "<% "{products.net.release_downloads}" %>"

code:
  title: "<% "{index-content-net.code_title}" %>"
  more: "<% "{index-content.code_more}" %>"
  more_link: "<% dict "products.net.more_link" %>"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // <% "{index-content.code_comment_1}" %>
    string template = "chart_template.docx";

    // <% "{index-content.code_comment_2}" %>
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // <% "{index-content.code_comment_3}" %>
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // <% "{index-content.code_comment_4}" %>
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // <% "{index-content.code_comment_5}" %>
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "<% "{index-content.overview_title}" %>"
  description: "<% "{index-content-net.overview_description}" %>"
  features:
    # feature loop
    - title: "<% "{index-content-net.overview_feature_1.title}" %>"
      content: "<% "{index-content-net.overview_feature_1.description}" %>"

    # feature loop
    - title: "<% "{index-content-net.overview_feature_2.title}" %>"
      content: "<% "{index-content-net.overview_feature_2.description}" %>"

    # feature loop
    - title: "<% "{index-content-net.overview_feature_3.title}" %>"
      content: "<% "{index-content-net.overview_feature_3.description}" %>"

############################# Platforms ############################
platforms:
  enable: true
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content-net.platforms_description}" %>"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "<% "{index-content.formats_title}" %>"
  description: |
    <% "{index-content-net.formats_description}" %>
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
  title: "<% "{index-content-net.features.title}" %>"
  description: "<% "{index-content-net.features.description}" %>"

  items:
    # feature loop
    - icon: "preview"
      title: "<% "{index-content-net.features.feature_1.title}" %>"
      content: "<% "{index-content-net.features.feature_1.content}" %>"

    # feature loop
    - icon: "manipulate"
      title: "<% "{index-content-net.features.feature_2.title}" %>"
      content: "<% "{index-content-net.features.feature_2.content}" %>"

    # feature loop
    - icon: "two_pages"
      title: "<% "{index-content-net.features.feature_3.title}" %>"
      content: "<% "{index-content-net.features.feature_3.content}" %>"

    # feature loop
    - icon: "document_settings"
      title: "<% "{index-content-net.features.feature_4.title}" %>"
      content: "<% "{index-content-net.features.feature_4.content}" %>"

    # feature loop
    - icon: "text"
      title: "<% "{index-content-net.features.feature_5.title}" %>"
      content: "<% "{index-content-net.features.feature_5.content}" %>"

    # feature loop
    - icon: "add"
      title: "<% "{index-content-net.features.feature_6.title}" %>"
      content: "<% "{index-content-net.features.feature_6.content}" %>"

    # feature loop
    - icon: "manipulate"
      title: "<% "{index-content-net.features.feature_7.title}" %>"
      content: "<% "{index-content-net.features.feature_7.content}" %>"

    # feature loop
    - icon: "convert"
      title: "<% "{index-content-net.features.feature_8.title}" %>"
      content: "<% "{index-content-net.features.feature_8.content}" %>"

    # feature loop
    - icon: "update"
      title: "<% "{index-content-net.features.feature_9.title}" %>"
      content: "<% "{index-content-net.features.feature_9.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.title}" %>"
  description: "<% "{index-content-net.code_samples_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content-net.code_title_sample_1}" %>"
      content: |
        <% "{index-content-net.code_samples_sample_1_content_1}" %> <% "{index-content-net.code_samples_sample_1_content_2}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_1.code_title}" %>">}}
        ```csharp {style=abap}
        // <% "{index-content.code_samples.sample_1.comment_1}" %>
        // <% "{index-content.code_samples.sample_1.comment_2}" %>
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // <% "{index-content.code_samples.sample_1.comment_3}" %>
        string template = "Bulleted List Template.docx";

        // <% "{index-content.code_samples.sample_1.comment_4}" %>
        string result = "Result Report.docx"

        // <% "{index-content.code_samples.sample_1.comment_5}" %>
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // <% "{index-content.code_samples.sample_1.comment_6}" %>
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "<% "{index-content-net.code_title_sample_2}" %>"
      content: |
        <% "{index-content-net.code_samples_sample_2_content_1}" %> <% "{index-content-net.code_samples_sample_2_content_2}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_2.code_title}" %>">}}
        ```csharp {style=abap}
        // <% "{index-content.code_samples.sample_2.comment_1}" %>
        // <% "{index-content.code_samples.sample_2.comment_2}" %> <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // <% "{index-content.code_samples.sample_2.comment_3}" %>
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // <% "{index-content.code_samples.sample_2.comment_4}" %>
        string template = "Pie Chart Template.pptx";

        // <% "{index-content.code_samples.sample_2.comment_5}" %>
        string result = "Result Report.pptx"

        // <% "{index-content.code_samples.sample_2.comment_6}" %>
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // <% "{index-content.code_samples.sample_2.comment_7}" %>
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---