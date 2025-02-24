



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: ru
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Создавайте таблицы в документах DOCX с помощью C#"
head_description: "API GroupDocs.Assembly for .NET позволяет разработчикам легко добавлять и заполнять таблицы в документах и электронных письмах данными из динамических источников."

############################# Header ############################
title: "Генерируйте таблицы данных в документах DOCX с помощью нашего API .NET" 
description: "GroupDocs.Assembly for .NET позволяет динамически заполнять таблицы в документах DOCX данными из различных источников."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатную версию"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Обзор GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) предназначен для создания документов и отчетов путем заполнения шаблонов данными из нескольких источников. Легко вставляйте структурированные данные в таблицы, списки и диаграммы или динамически встраивайте изображения. Расширенный синтаксис обеспечивает точное размещение данных. Поддерживает более 50 форматов, включая PDF, документы MS Office и файлы электронной почты.

############################# Steps ############################
steps:
    enable: true
    title: "Как заполнить таблицу в документе DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) позволяет динамически заполнять таблицы в шаблонах для таких форматов, как DOCX. Вставляйте данные из различных источников в свои таблицы.
      
      1. Создайте шаблон DOCX с заполнителями для таблиц.
      2. Извлеките данные из любого поддерживаемого источника.
      3. Отфильтруйте данные, чтобы включить только необходимую информацию.
      4. Сохраните документ с заполненной таблицей.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Пример документа"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Добавьте эти теги в строку шаблона таблицы
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Установите путь к файлу шаблона
        string template = "table_template.docx";

        // Извлеките данные из поддерживаемого источника
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Сохраните документ с заполненной таблицей данными
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Генерация документов с динамическими таблицами"
  description: "GroupDocs.Assembly for .NET облегчает создание документов, автоматизируя заполнение таблиц и поддерживая дополнительные элементы, такие как диаграммы, списки и изображения с помощью шаблонов и расширенного разметки."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Создавайте отчеты из структурированных данных"
      content: "API обрабатывает данные из таких источников, как JSON, XML и CSV для эффективного и точного заполнения таблиц в офисных документах."

    # feature loop
    - title: "Визуальное отображение данных"
      content: "GroupDocs.Assembly позволяет создавать таблицы, списки и диаграммы, а также встраивать текст, ссылки и изображения для профессионального дизайна документов."

    # feature loop
    - title: "Точное размещение данных в таблице"
      content: "Используйте синтаксис на основе LINQ для динамического добавления строк и столбцов в таблицы. Настраивайте стили, включая цвета и форматирование, программно."

    # feature loop
    - title: "Поддержка широкого спектра форматов"
      content: "Обрабатывайте популярные форматы файлов, такие как MS Office, OpenOffice, PDF и HTML. Без проблем встраивайте заполненные таблицы в поддерживаемые типы документов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как динамически заполнить таблицу данных"
      content: |
        Этот пример демонстрирует, как заполнить таблицу в документе DOCX с помощью динамических данных.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Подготовьте шаблон с заполнителем для таблицы
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Укажите путь к файлу шаблона
          string template = "table_template.docx";

          // Извлеките данные из выбранного источника
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Создайте объект источника данных с необходимыми данными
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Инициализируйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Сохраните завершенный документ с заполненной таблицей
          asm.AssembleDocument(template, "result.docx", data);
          ```
        platform: "net"
        copy_title: "Копировать"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.docx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Изучите возможности GroupDocs.Assembly бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачать с Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Узнать о лицензировании"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Изучите ключевые функции"
    exclude: "table"
    description: "Наше решение упрощает создание профессиональных документов с динамически заполняемыми таблицами и дополнительными элементами."
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Создавайте отчеты с детальными таблицами"
    exclude: "DOCX"
    description: ".NET позволяет создавать подробные отчеты путем заполнения шаблонов таблицами и другими элементами данных в более чем 50 поддерживаемых форматах."
    items: 
          
        # format loop 1
        - name: "Добавить таблицу в PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Добавить таблицу в DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Добавить таблицу в PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Добавить таблицу в XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---