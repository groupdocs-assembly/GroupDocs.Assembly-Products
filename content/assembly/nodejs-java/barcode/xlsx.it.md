



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:12
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
        command: "npm i @groupdocs/groupdocs.assembly"
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
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "barcode_template.xlsx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
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
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          const template = "barcode_template.xlsx";

          // {code_1.comment_3}
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // {code_1.comment_4}
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // {code_1.comment_5}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_6}
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // {code_1.comment_7}
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Copia"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica il risultato"
            icon: "download"
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    exclude: "barcode"
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
        - name: "Aggiungi un codice a barre a un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Aggiungi un codice a barre a un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Aggiungi un codice a barre a un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Aggiungi un codice a barre a un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---