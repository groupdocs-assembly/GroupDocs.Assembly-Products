



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: ru
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Вставка диаграмм в файлы XLSX с помощью JavaScript"
head_description: "С помощью GroupDocs.Assembly for Node.js via Java разработчики могут быстро создавать и встраивать динамические диаграммы в документы, используя живые источники данных."

############################# Header ############################
title: "Добавляйте диаграммы в файлы XLSX с помощью Node.js" 
description: "GroupDocs.Assembly for Node.js via Java упрощает процесс интеграции диаграмм в документы XLSX с вводом данных в реальном времени."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Начните бесплатно сегодня"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Обзор GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) — это мощное решение для создания автоматизированных документов и отчетов. Добавляйте диаграммы, таблицы, изображения, штрих-коды и списки в файлы с точностью и эффективностью. Эта универсальная платформа поддерживает более 50 форматов, включая PDF, документы Office и электронную почту.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для добавления диаграммы в документ XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) упрощает добавление диаграмм в файлы XLSX. Выберите из таких типов диаграмм, как столбчатые, линейные или круговые.
      
      1. Создайте шаблон XLSX с заполнителями для диаграмм.
      2. Загрузите данные из поддерживаемого источника.
      3. Настройте параметры диаграммы, включая тип, цвета и метки.
      4. Экспортируйте документ с встраиваемой диаграммой.
   
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
        // Включите этот тег в ваш шаблон для генерации диаграммы
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Укажите путь к файлу шаблона
        const template = "chart_template.xlsx";

        // Извлеките данные из вашей системы источника
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Сохраните окончательный документ со встроенной диаграммой
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Легко встраивайте диаграммы в ваши документы"
  description: "GroupDocs.Assembly for Node.js via Java упрощает создание документов с множеством функций в популярных файловых форматах. Используйте шаблоны для добавления диаграмм, таблиц, штрих-кодов, списков, изображений и многого другого с обновлениями данных в реальном времени."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Преобразуйте данные в профессиональные диаграммы"
      content: "Конвертируйте данные из таких источников, как JSON, XML или CSV, в высококачественные диаграммы, которые можно напрямую встроить в документы."

    # feature loop
    - title: "Создавайте потрясающие визуализации"
      content: "Генерируйте столбчатые диаграммы, круговые диаграммы и линейные графики, которые бесшовно интегрируются с другими элементами документа, такими как изображения, таблицы и штрих-коды."

    # feature loop
    - title: "Гибкое оформление и размещение диаграмм"
      content: "Используйте шаблоны LINQ для контроля позиционирования и оформления диаграмм, включая цвета, макеты и метки, для безупречной презентации."

    # feature loop
    - title: "Поддержка множества форматов файлов"
      content: "Создавайте документы в форматах, таких как MS Office, PDF, OpenOffice и HTML, с идеально интегрированными диаграммами для профессионального завершения."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Динамическое создание и вставка диаграмм"
      content: |
        В этом примере иллюстрируется, как программно создавать и встраивать диаграммы в файлы XLSX.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Настройте шаблон с заполнителем для диаграммы
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Определите путь к файлу шаблона
          const template = "table_template.xlsx";

          // Извлеките данные из выбранного источника
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Подготовьте объект данных, содержащий информацию о диаграмме
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Выберите тип диаграммы и настройте ее внешний вид
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Инициализируйте DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Сохраните обновленный документ с встроенной диаграммой
          asm.assembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Откройте для себя продвинутые функции"
    exclude: "chart"
    description: "Эта платформа упрощает создание документов с инструментами, предназначенными для визуализации данных и бесшовной интеграции."
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
    title: "Генерация отчетов в нескольких форматах файлов"
    exclude: "XLSX"
    description: "Node.js via Java поддерживает более 50 форматов, что упрощает комбинирование шаблонов с данными для получения отшлифованных документов."
    items: 
          
        # format loop 1
        - name: "Диаграммы в PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Диаграммы в DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Диаграммы в PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Диаграммы в XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---