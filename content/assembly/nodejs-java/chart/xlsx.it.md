



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:17
draft: false
lang: it
format: Xlsx
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
    link_title: "Scopri di più"
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
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento di esempio"
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
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```java {style=abap}
        // {examples.comment_1}
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // {examples.comment_2}
        String template = "chart_template.xlsx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_chart.webp" # 500x500 px
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
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // {code_1.comment_2}
          String template = "table_template.xlsx";

          // {code_1.comment_3}
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // {code_1.comment_5}
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // {code_1.comment_6}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_7}
          asm.assembleDocument(template, "result.xlsx", data, design);
          ```
        platform: "java"
        copy_title: "Copia"
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
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica il risultato"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.xlsx"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Esplora le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Scarica da NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Scopri di più sulle licenze"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "chart"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "XLSX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Grafici in PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Grafici in DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Grafici in PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Grafici in XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---