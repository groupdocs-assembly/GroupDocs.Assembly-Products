



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:16
draft: false
lang: de
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: ""
head_description: ""

############################# Header ############################
title: "" 
description: ""
subtitle: "" 

header_actions:
  enable: true
  items:
    #  loop
    - title: ""
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: ""
    link: "/assembly/nodejs-java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {steps.content.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {steps.content.step_4}
   
    code:
      platform: "java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Beispieldokument"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "Klicken Sie zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "list_template.pptx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "{more_features.image_description}"
  features:
    # feature loop
    - title: "{more_features.feature_1.title}"
      content: "{more_features.feature_1.content}"

    # feature loop
    - title: "{more_features.feature_2.title}"
      content: "{more_features.feature_2.content}"

    # feature loop
    - title: "{more_features.feature_3.title}"
      content: "{more_features.feature_3.content}"

    # feature loop
    - title: "{more_features.feature_4.title}"
      content: "{more_features.feature_4.content}"
      
  code_samples_ext:
    # code sample ext loop
    - title: "{code_1.title}"
      content: |
        {code_1.content}
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // {code_1.comment_1}
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          const template = "numlist_template.pptx";

          // {code_1.comment_3}
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // {code_1.comment_4}
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // {code_1.comment_5}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.pptx", data);
          ```
        platform: "java"
        copy_title: "Kopieren"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "Klicken Sie zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Laden Sie das Ergebnis herunter"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.pptx"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Bereit anzufangen?"
  description: "Erforschen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Herunterladen von NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Erfahren Sie mehr über Lizenzen"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "list"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "PPTX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Erstellen Sie eine Liste in einem PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Erstellen Sie eine Liste in einem DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Erstellen Sie eine Liste in einem PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Erstellen Sie eine Liste in einem XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---