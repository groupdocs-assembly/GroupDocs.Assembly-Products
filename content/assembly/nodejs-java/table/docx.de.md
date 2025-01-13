



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:21
draft: false
lang: de
format: Docx
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
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
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
        ```java {style=abap}
        // {examples.comment_1}
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // {examples.comment_2}
        String template = "table_template.docx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_table.webp" # 500x500 px
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
          ```java {style=abap}
          // {code_1.comment_1}
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // {code_1.comment_2}
          String template = "table_template.docx";

          // {code_1.comment_3}
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // {code_1.comment_5}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.docx", data);
          ```
        platform: "java"
        copy_title: "Kopieren"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "Klicken Sie zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Laden Sie das Ergebnis herunter"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.docx"
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
    exclude: "table"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "DOCX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Fügen Sie eine Tabelle zu einem PDF hinzu"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Fügen Sie eine Tabelle zu einem DOCX hinzu"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Fügen Sie eine Tabelle zu einem PPTX hinzu"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Fügen Sie eine Tabelle zu einem XLSX hinzu"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---