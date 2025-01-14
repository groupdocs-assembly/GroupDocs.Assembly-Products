



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:13
draft: false
lang: fr
format: Pdf
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
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {texts_pdf.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {texts_pdf.step_4}
   
    code:
      platform: "java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Document d'exemple"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        // {texts_pdf.comment_tmp}
        const template = "barcode_template.docx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // {texts_pdf.step_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
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
          // {texts_pdf.comment_tmp}
          const template = "barcode_template.docx";

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
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "Copier"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/assembly/formats/assembly_barcode.pdf"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Découvrez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Télécharger depuis NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "En savoir plus sur les licences"
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
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "PDF"
    description: ""
    items: 
          
        # format loop 1
        - name: "Ajouter un code-barres à un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Ajouter un code-barres à un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ajouter un code-barres à un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Ajouter un code-barres à un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---