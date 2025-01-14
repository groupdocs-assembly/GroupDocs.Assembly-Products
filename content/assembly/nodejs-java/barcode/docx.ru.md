



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:12
draft: false
lang: ru
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
    link_title: "Узнать больше"
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
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Пример документа"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "barcode_template.docx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
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
          asm.assembleDocument(template, "result.docx", data);
          ```
        platform: "java"
        copy_title: "Копировать"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_barcode.docx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Изучите возможности GroupDocs.Assembly бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачать с NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Узнать о лицензировании"
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
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "DOCX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Добавить штрих-код в PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Добавить штрих-код в DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Добавить штрих-код в PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Добавить штрих-код в XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---