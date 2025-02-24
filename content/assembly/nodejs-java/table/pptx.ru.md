



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: ru
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Вставка таблиц в документы PPTX с помощью JavaScript"
head_description: "Используйте GroupDocs.Assembly for Node.js via Java для быстрого встраивания таблиц в документы или электронные письма, получая данные из различных источников."

############################# Header ############################
title: "Просто добавляйте таблицы в файлы PPTX с Node.js" 
description: "С GroupDocs.Assembly for Node.js via Java заполнение таблиц в документах PPTX происходит эффективно, используя данные из множества источников."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Начните бесплатный пробный период"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Введение в GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) — это мощный инструмент для автоматизации создания документов. Он позволяет вставлять таблицы, диаграммы, списки и изображения в шаблоны с точным размещением содержимого. Поддерживая более 50 форматов файлов, включая PDF, Word и электронную почту, он упрощает генерацию отчетов и выполнение других задач.

############################# Steps ############################
steps:
    enable: true
    title: "Как добавить данные в таблицу в PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) позволяет быстро заполнять шаблоны таблиц для файлов PPTX с использованием динамических источников данных.
      
      1. Создайте шаблон PPTX с заполнителями для строк и столбцов таблицы.
      2. Загрузите данные из поддерживаемого источника, например, JSON или CSV.
      3. Организуйте и отформатируйте данные по мере необходимости.
      4. Сгенерируйте документ с заполненной таблицей.
   
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
        // Включите эти теги в заполнители строк таблицы вашего шаблона
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Укажите путь к файлу шаблона
        const template = "table_template.pptx";

        // Загрузите ваши данные из выбранного источника
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Сохраните финальный документ с заполненной таблицей
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Добавляйте таблицы, основанные на данных, в документы"
  description: "GroupDocs.Assembly for Node.js via Java позволяет пользователям автоматически создавать таблицы, а также встраивать диаграммы, изображения и списки с использованием шаблонов."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Ключевые особенности GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерация таблиц из структурированных данных"
      content: "Получайте данные из JSON, XML, CSV и других форматов для автоматического заполнения таблиц в документах."

    # feature loop
    - title: "Создание высококачественного визуального контента"
      content: "Используйте GroupDocs.Assembly для разработки профессиональных таблиц, диаграмм и списков, а также для добавления ссылок, изображений и текста для улучшения внешнего вида документа."

    # feature loop
    - title: "Динамическое размещение содержимого таблицы"
      content: "Добавляйте строки и столбцы программно с помощью шаблонов на основе LINQ и настраивайте стили, такие как шрифты, цвета и выравнивание."

    # feature loop
    - title: "Бесшовная работа с различными форматами"
      content: "Создавайте или редактируйте таблицы в MS Office, OpenOffice, PDF, HTML и других форматах, объединяя их в файлы по мере необходимости."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как программно заполнить таблицу"
      content: |
        Этот пример демонстрирует, как заполнить таблицу в документе PPTX данными из внешнего источника.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Разработайте шаблон с заполнителями для таблицы
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Укажите путь к файлу шаблона
          const template = "table_template.pptx";

          // Загрузите необходимые данные из вашего источника
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Организуйте данные в необходимую структуру
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Инициализируйте DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Сохраните выходной документ с заполненной таблицей
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "Основные функции в одном взгляде"
    exclude: "table"
    description: "Наш API автоматизирует создание таблиц и улучшает генерацию документов с помощью универсальных инструментов и шаблонов."
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
    title: "Генерация таблиц в различных форматах"
    exclude: "PPTX"
    description: "С Node.js via Java заполняйте шаблоны и создавайте обширные таблицы более чем в 50 поддерживаемых типах файлов."
    items: 
          
        # format loop 1
        - name: "Добавить таблицу в PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Добавить таблицу в DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Добавить таблицу в PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Добавить таблицу в XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---