<% configRef "..\\..\\configs\\table\\format_pdf_net.yml" %>
<% include "..\\..\\data\\format_data.md" %>

---
############################# Static ############################
layout: "format"
date:  <% date "utcnow" %>
draft: false
lang: <% lower ( get "lang") %>
format: <% get "FileformatCap" %>
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "<% (dict "head.title") %>"
head_description: "<% (dict "head.description") %>"

############################# Header ############################
title: "<% (dict "header.title") %>" 
description: "<% (dict "header.description") %>"
subtitle: "<% (dict "header.subtitle") %>" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "<% (dict "header.action_title") %>"
      link: "<% get "ReleaseDownloads" %>"
      
############################# About ############################
about:
    enable: true
    title: "<% (dict "about.title") %>"
    link: "/assembly/<% get "ProdCode" %>/"
    link_title: "<% "{common-content.texts.learn_more}" %>"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       <% (dict "about.content") %>

############################# Steps ############################
steps:
    enable: true
    title: "<% "{steps.title}" %>"
    content: |
      <% "{steps.content.title}" %>
      
      1. <% "{texts_pdf.step_1}" %>
      2. <% "{steps.content.step_2}" %>
      3. <% "{steps.content.step_3}" %>
      4. <% "{texts_pdf.step_4}" %>
   
    code:
      platform: "net"
      copy_title: "<% "{common-content.format-code.copy_title}" %>"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "<% "{common-content.format-code.result_title}" %>"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "<% "{common-content.format-code.copy_tip}" %>"
        copy_done: "<% "{common-content.format-code.copy_done}" %>"
      links:
        #  loop
        - title: "<% "{common-content.format-code.links.title_1}" %>"
          link: "<% get "MoreLink" %>"
        #  loop
        - title: "<% "{common-content.format-code.links.title_2}" %>"
          link: "<% get "DocsUrl" %>"
          
      content: |
        ```csharp {style=abap}
        // <% "{examples.comment_1}" %>
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // <% "{examples.comment_2}" %>
        // <% "{texts_pdf.comment_tmp}" %>
        string template = "table_template.docx";

        // <% "{examples.comment_3}" %>
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // <% "{examples.comment_4}" %>
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.<% get "fileformat" %>", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "<% "{more_features.title}" %>"
  description: "<% "{more_features.description}" %>"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "<% "{more_features.image_description}" %>"
  features:
    # feature loop
    - title: "<% "{more_features.feature_1.title}" %>"
      content: "<% "{more_features.feature_1.content}" %>"

    # feature loop
    - title: "<% "{more_features.feature_2.title}" %>"
      content: "<% "{more_features.feature_2.content}" %>"

    # feature loop
    - title: "<% "{more_features.feature_3.title}" %>"
      content: "<% "{more_features.feature_3.content}" %>"

    # feature loop
    - title: "<% "{more_features.feature_4.title}" %>"
      content: "<% "{more_features.feature_4.content}" %>"
      
  code_samples_ext:
    # code sample ext loop
    - title: "<% "{code_1.title}" %>"
      content: |
        <% "{code_1.content}" %>
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // <% "{code_1.comment_1}" %>
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // <% "{code_1.comment_2}" %>
          // <% "{texts_pdf.comment_tmp}" %>
          string template = "table_template.docx";

          // <% "{code_1.comment_3}" %>
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // <% "{code_1.comment_4}" %>
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // <% "{code_1.comment_5}" %>
          DocumentAssembler asm = new DocumentAssembler();

          // <% "{code_1.comment_6}" %>
          asm.AssembleDocument(template, "result.<% get "fileformat" %>", data);
          ```
        platform: "net"
        copy_title: "<% "{common-content.format-code.copy_title}" %>"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "<% "{common-content.format-code.copy_tip}" %>"
          copy_done: "<% "{common-content.format-code.copy_done}" %>"
        top_links:
          #  loop
          - title: "<% "{common-content.format-code.result_title_bottom}" %>"
            icon: "download"
            link: "/examples/assembly/formats/assembly_<% get "OperationLow" %>.<% get "fileformat" %>"
        links:
          #  loop
          - title: "<% "{common-content.format-code.links.title_1}" %>"
            link: "<% get "MoreLink" %>"
          #  loop
          - title: "<% "{common-content.format-code.links.title_2}" %>"
            link: "<% get "DocsUrl" %>"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "<% "{common-content.format-actions.title}" %>"
  description: "<% "{common-content.format-actions.description}" %>"
  items:
    #  loop
    - title: "<% "{common-content.format-actions.comment_1}" %>"
      link: "<% get "ReleaseDownloads" %>"
      color: "red"
        #  loop
    - title: "<% "{common-content.format-actions.comment_2}" %>"
      link: "<% get "PricesUrl" %>"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "<% (dict "operations.title") %>"
    exclude: "<% get "OperationLow" %>"
    description: "<% (dict "operations.description") %>"
<% include "..\\..\\data\\operations_others.md" %>

############################# More Formats ########################
more_formats:
    enable: true
    title: "<% (dict "formats.title") %>"
    exclude: "<% get "FileFormatUp" %>"
    description: "<% (dict "formats.description") %>"
<% include "..\\..\\data\\format_others.md" %>

---