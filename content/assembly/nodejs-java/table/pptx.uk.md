



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:18
draft: false
lang: uk
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
    link_title: "Дізнатися більше"
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
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Приклад документа"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "натисніть, щоб скопіювати"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "table_template.pptx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
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
          ```javascript {style=abap}
          // {code_1.comment_1}
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          const template = "table_template.pptx";

          // {code_1.comment_3}
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // {code_1.comment_4}
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // {code_1.comment_5}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.pptx", data);
          ```
        platform: "java"
        copy_title: "Копіювати"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "натисніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.pptx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Досліджуйте можливості GroupDocs.Assembly безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити з NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Дізнатися про ліцензування"
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
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "PPTX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Додати таблицю до PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Додати таблицю до DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Додати таблицю до PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Додати таблицю до XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---