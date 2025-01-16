



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:02
draft: false
lang: ru
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Объединение документов в PPTX с помощью JavaScript"
head_description: "GroupDocs.Assembly позволяет быстро объединять файлы PPTX с помощью JavaScript за несколько простых шагов."

############################# Header ############################
title: "Легкое объединение содержимого в файлах PPTX" 
description: "С помощью GroupDocs.Assembly for Node.js via Java интеграция одного файла PPTX в другой происходит быстро и точно. Получите гибкие и надежные инструменты для безупречного объединения."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Попробуйте бесплатно"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Обзор GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) предлагает мощные возможности управления документами. Объединяйте один файл с другим, поддерживая более 50 форматов, таких как PDF и MS Office. Настраивайте макеты, редактируйте содержимое и организуйте документы так, как вам нужно.

############################# Steps ############################
steps:
    enable: true
    title: "Как объединить документ в файл PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) упрощает вставку одного файла PPTX в другой с настраиваемыми параметрами.
      
      1. Создайте шаблон PPTX с заполнителями для содержимого.
      2. Установите путь к шаблону.
      3. Укажите путь к документу для объединения.
      4. Экспортируйте окончательный файл с объединенным содержимым.
   
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
        // Вставьте этот тег в свой шаблон, чтобы определить, где будет встроен документ
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Установите путь к основному шаблону
        const template = "doc_template.pptx";

        // Укажите путь к документу, который вы хотите объединить
        const data 
            = new assemblyLib.DataSourceInfo("insert.pptx", "doc_expression");

        // Сохраните конечный результат с встроенным документом
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Мощные инструменты для интеграции документов"
  description: "GroupDocs.Assembly for Node.js via Java упрощает встраивание файлов различных форматов и предлагает полную настройку. Обеспечьте постоянные, профессиональные результаты каждый раз."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Ключевые возможности GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерация отчетов с бизнес-данными"
      content: "Извлекайте данные из источников JSON, XML или CSV для быстрого и точного создания комплексных отчетов и документов."

    # feature loop
    - title: "Добавление богатых визуальных элементов"
      content: "GroupDocs.Assembly позволяет включать таблицы, диаграммы, списки, изображения и штрих-коды наряду с текстом и гиперссылками."

    # feature loop
    - title: "Точное размещение данных"
      content: "Используйте шаблоны LINQ для точного позиционирования данных, работы с повторяющимися элементами, такими как массивы, и простого настраивания стилей."

    # feature loop
    - title: "Работа с различными форматами"
      content: "Эффективно объединяйте содержимое в таких форматах, как PDF, файлы MS Office, HTML и OpenOffice, обеспечивая гибкость для всех проектов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Программное встраивание изображения в документ"
      content: |
        Этот пример демонстрирует, как вставить изображение в файл PPTX с помощью GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Добавьте заполнитель в шаблон для изображения
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Укажите путь к файлу шаблона
          const template = "template.pptx";

          // Установите путь к изображению, которое хотите встроить
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Инициализируйте объект DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Сохраните документ с включенным изображением
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Основные функции на первый взгляд"
    exclude: "document"
    description: "Изучите комплексные инструменты, которые предлагает GroupDocs.Assembly для эффективного и бесшовного объединения документов."
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Объединение документов в различных форматах"
    exclude: "PPTX"
    description: "Используйте Node.js via Java для объединения содержимого более чем в 50 форматах файлов, гарантируя профессиональные и гладкие результаты."
    items: 
          
        # format loop 1
        - name: "Вставить документ в PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Вставить документ в DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Вставить документ в PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Вставить документ в XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---