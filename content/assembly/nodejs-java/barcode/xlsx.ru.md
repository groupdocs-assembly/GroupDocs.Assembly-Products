



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: ru
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Добавление штрих-кодов в файлы XLSX с использованием JavaScript"
head_description: "Генерируйте и встраивайте штрих-коды в ваши документы и электронные письма с помощью API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Создание штрих-кодов для файлов XLSX с использованием Node.js" 
description: "С помощью GroupDocs.Assembly for Node.js via Java вы можете динамически генерировать, настраивать и встраивать штрих-коды в документы XLSX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Начать"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Введение в GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) позволяет создавать профессиональные документы, объединяя данные из нескольких источников. Добавляйте графики, таблицы, списки, изображения и штрих-коды в ваши файлы. Используйте шаблоны, чтобы организовывать контент именно там, где это необходимо. Работает более чем с 50 форматами, включая PDFs, документы Office и электронные письма.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для добавления штрих-кода в файлы XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) позволяет встраивать штрих-коды в документы XLSX. Поддерживает более 60 типов штрих-кодов, включая 1D и 2D форматы.
      
      1. Создайте шаблон XLSX с заполнителями для штрих-кодов.
      2. Получите данные из совместимого источника.
      3. Установите параметры штрих-кода, такие как размер и разрешение.
      4. Сохраните окончательный документ с встроенным штрих-кодом.
   
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
        // Используйте этот тег в шаблоне, чтобы включить штрих-код в выходной документ
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Укажите путь к файлу шаблона
        const template = "barcode_template.xlsx";

        // Загрузите необходимые данные из вашего источника
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Сохраните документ с примененным штрих-кодом
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Генерация документов с шаблонами на основе данных"
  description: "С помощью GroupDocs.Assembly for Node.js via Java вы можете создавать профессиональные файлы в популярных форматах, без проблем встраивая графики, таблицы, списки, ссылки, изображения и штрих-коды."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Основные возможности GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Создание отчетов с бизнес-данными"
      content: "Используйте API для быстрого и точного заполнения шаблонов данными из таких форматов, как JSON, XML и CSV."

    # feature loop
    - title: "Добавление визуальных элементов"
      content: "GroupDocs.Assembly поддерживает вставку элементов, таких как графики, таблицы, списки, текст, ссылки, изображения и штрих-коды в реальном времени."

    # feature loop
    - title: "Управление размещением данных"
      content: "С помощью шаблонов на основе LINQ вы можете точно позиционировать данные, обходить массивы и применять пользовательское форматирование программно."

    # feature loop
    - title: "Совместимость с множеством форматов"
      content: "Работайте с такими файлами, как документы MS Office, PDFs, HTML, файлы OpenOffice и электронные письма. Объединяйте несколько документов при необходимости."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Пример: Программная генерация штрих-кода"
      content: |
        Этот пример демонстрирует, как программно сгенерировать и вставить штрих-код в документ XLSX.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Создайте шаблон с заполнителем для штрих-кода
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Укажите путь к файлу шаблона
          const template = "barcode_template.xlsx";

          // Получите данные из источника
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Создайте объект источника данных с необходимыми деталями
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Инициализируйте экземпляр DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Настройте конфигурацию штрих-кода
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Сохраните документ с включенным штрих-кодом
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: "Изучите ключевые возможности"
    exclude: "barcode"
    description: "Упрощайте обработку документов с помощью расширенных инструментов и возможностей автоматизации."
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поддерживаемые форматы файлов для создания отчетов"
    exclude: "XLSX"
    description: "Node.js via Java обрабатывает более 50 типов файлов, что упрощает объединение данных и обработку шаблонов для достижения высококачественных результатов."
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