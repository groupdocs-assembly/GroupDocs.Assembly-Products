<% configRef "..\\..\\configs\\index\\index.yml" %>
<% include "..\\..\\data\\family_data.md" %>
---
############################# Static ############################
layout: "family"
date:  <% date "utcnow" %>
draft: false

product: "Assembly"
product_tag: "assembly"

lang: <% lower ( get "lang") %>

############################# Head ############################
head_title: "<% "{index-content.head_title}" %>"
head_description: "<% "{index-content.head_description}" %>"

############################# Header ############################
title: "<% "{index-content.title}" %>"
description:  |
  <% "{index-content.description_1}" %>

  <% "{index-content.description_2}" %>

  <% "{index-content.description_3}" %>

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "<% "{index-content.platforms.head_title}" %>"
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content.platforms.description}" %>"
  details_link_title: "<% "{index-content.platforms.learn_more}" %>"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> <% "{index-content.platforms.any_other_text_editor}" %>
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "<% "{index-content.features.title}" %>"
  description: "<% "{index-content.features.description}" %>"

  items:
    # items loop
    - icon: "additional"
      title: "<% "{index-content.features.feature_1.title}" %>"
      content: "<% "{index-content.features.feature_1.content}" %>"

    # items loop
    - icon: "manipulate"
      title: "<% "{index-content.features.feature_2.title}" %>"
      content: "<% "{index-content.features.feature_2.content}" %>"

    # items loop
    - icon: "structure"
      title: "<% "{index-content.features.feature_3.title}" %>"
      content: "<% "{index-content.features.feature_3.content}" %>"

    # items loop
    - icon: "merge"
      title: "<% "{index-content.features.feature_4.title}" %>"
      content: "<% "{index-content.features.feature_4.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.index_title}" %>"
  description: "<% "{index-content.code_samples.index_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content.code_samples.sample_index.title}" %>"
      content: |
       <% "{index-content.code_samples.sample_index.content}" %>
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            DocumentAssembler assembler = new DocumentAssembler();

            //<% "{index-content.code_samples.sample_index.comment_2}" %>
            var tmp_path = "barcode_template.docx";

            //<% "{index-content.code_samples.sample_index.comment_3}" %>
            var res_path = "result.docx";

            //<% "{index-content.code_samples.sample_index.comment_4}" %>
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //<% "{index-content.code_samples.sample_index.comment_5}" %>
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            DocumentAssembler assembler = new DocumentAssembler();
            
            //<% "{index-content.code_samples.sample_index.comment_2}" %>
            String tmp_path = "barcode_template.docx";

            //<% "{index-content.code_samples.sample_index.comment_3}" %>
            String res_path = "result.docx";

            //<% "{index-content.code_samples.sample_index.comment_4}" %>
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // <% "{index-content.code_samples.sample_index.comment_5}" %>
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            const assembler = new assemblyLib.DocumentAssembler();
            
            //<% "{index-content.code_samples.sample_index.comment_2}" %>
            const tmp_path = "barcode_template.docx";

            //<% "{index-content.code_samples.sample_index.comment_3}" %>
            const res_path = "result.docx";

            //<% "{index-content.code_samples.sample_index.comment_4}" %>
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // <% "{index-content.code_samples.sample_index.comment_5}" %>
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "<% "{index-content.formats.title}" %>"
  description: "<% "{index-content.formats.description}" %>"

############################# Metrics ###############################
metrics:
  enable: true
  title: "<% "{index-content.metrics.title}" %>"
  description: "<% "{index-content.metrics.description}" %>"

  items:
    # items loop
    - number: "50+"
      title: "<% "{index-content.metrics.item_1.title}" %>"
      content: "<% "{index-content.metrics.item_1.description}" %>"

    # items loop
    - number: "650k"
      title: "<% "{index-content.metrics.item_2.title}" %>"
      content: "<% "{index-content.metrics.item_2.description}" %>"

    # items loop
    - number: "18k"
      title: "<% "{index-content.metrics.item_3.title}" %>"
      content: "<% "{index-content.metrics.item_3.description}" %>"

    # items loop
    - number: "150+"
      title: "<% "{index-content.metrics.item_4.title}" %>"
      content: "<% "{index-content.metrics.item_4.description}" %>"


############################# Customers ###############################
customers:
  enable: true
  title: "<% "{index-content.customers.title}" %>"
  description: "<% "{index-content.customers.description}" %>"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description_index}" %>"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "<% "{index-content.faq.title}" %>"
  description: "<% "{index-content.faq.description}" %>"

  items:
    # items loop
    - question: "<% "{index-content.faq.item_1.question}" %>"
      answer: "<% "{index-content.faq.item_1.answer}" %>"

    # items loop
    - question: "<% "{index-content.faq.item_2.question}" %>"
      answer: "<% "{index-content.faq.item_2.answer}" %>"

    # items loop
    - question: "<% "{index-content.faq.item_3.question}" %>"
      answer: "<% "{index-content.faq.item_3.answer}" %>"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "<% "{index-content.cloud_links.title}" %>"
  description: "<% "{index-content.cloud_links.description}" %>"
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "<% "{index-content.cloud_links.item_1.content}" %>"
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "<% "{index-content.cloud_links.item_2.content}" %>"
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "<% "{index-content.cloud_links.item_3.content}" %>"
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "<% "{index-content.app_links.title}" %>"
  description: "<% "{index-content.app_links.description}" %>"

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "<% "{index-content.app_links.item_1.content}" %>"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "<% "{index-content.app_links.item_2.content}" %>"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "<% "{index-content.app_links.item_3.content}" %>"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---