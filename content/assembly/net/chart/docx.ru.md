



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: ru
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Создание графиков в файлах DOCX с использованием C#"
head_description: "API GroupDocs.Assembly for .NET упрощает для разработчиков процесс генерации и вставки графиков или диаграмм в документы динамически с использованием данных в реальном времени."

############################# Header ############################
title: "Встраивание графиков в файлы DOCX с помощью API .NET" 
description: "GroupDocs.Assembly for .NET предлагает мощный способ заполнить файлы DOCX динамическими данными и без труда интегрировать графики."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Попробуйте бесплатно"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Что такое GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) – это инструмент, предназначенный для упрощения создания документов и отчетов путем интеграции данных из различных источников. Генерируйте графики, таблицы, списки, штрих-коды и изображения динамически. Расширенные параметры форматирования позволяют точно размещать и настраивать ваш контент. Он поддерживает более 50 форматов файлов, включая PDF, документы MS Office и электронные письма.

############################# Steps ############################
steps:
    enable: true
    title: "Как добавить график в документ DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) упрощает процесс генерации и встраивания графиков в ваши шаблоны DOCX. Поддерживаются различные типы графиков, такие как столбчатые, круговые и линейные.
      
      1. Создайте шаблон DOCX с заполняемыми местами для графиков.
      2. Получите ваши данные из совместимого источника.
      3. Определите параметры графика, такие как тип, метки и цветовая схема.
      4. Сохраните обновленный файл с встроенным графиком.
   
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
        // Включите этот тег в свой шаблон для генерации графика
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Укажите путь к вашему шаблону
        string template = "chart_template.docx";

        // Загрузите данные из предпочитаемого источника
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Сохраните документ с встраиваемым графиком
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Добавляйте динамические графики в ваши документы без усилий"
  description: "GroupDocs.Assembly for .NET упрощает создание документов на основе данных в широко используемых форматах. Используйте шаблоны для вставки графиков, таблиц, штрих-кодов, списков, гиперссылок и изображений с передовой динамической интеграцией данных."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Преобразуйте данные в профессиональные графики"
      content: "Преобразуйте данные из JSON, XML, CSV и других источников в визуально привлекательные графики всего за несколько шагов с использованием нашего API."

    # feature loop
    - title: "Создавайте визуально привлекательный контент"
      content: "GroupDocs.Assembly поддерживает множество типов графиков, таких как столбчатые диаграммы, круговые диаграммы и линейные графики. Объедините их с таблицами, штрих-кодами, изображениями и другими элементами для создания профессиональных отчетов."

    # feature loop
    - title: "Точно позиционируйте и настраивайте графики"
      content: "С помощью синтаксиса LINQ вы можете динамически генерировать и размещать графики именно там, где это необходимо. Легко настраивайте стили, цвета и макет в соответствии с вашими требованиями."

    # feature loop
    - title: "Работает с различными форматами файлов"
      content: "Создавайте документы в популярных форматах, таких как MS Office, PDF, OpenOffice и HTML. Встраивайте графики без особых усилий в любой поддерживаемый формат с полной совместимостью."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Создание графика программным путем"
      content: |
        Этот пример демонстрирует, как динамически создать и встроить график в документ DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Подготовьте шаблон с заполняемым местом для графика
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Укажите путь к файлу шаблона
          string template = "table_template.docx";

          // Получите данные из вашего источника
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Сформируйте объект данных с необходимой информацией
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Настройте свойства графика, такие как тип и внешний вид
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Инициализируйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Экспортируйте документ с включенным графиком
          asm.AssembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "Откройте для себя ключевые возможности"
    exclude: "chart"
    description: "Наша платформа помогает вам создавать привлекательные, ориентированные на данные документы, адаптированные к вашим нуждам."
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
    title: "Создавайте визуально насыщенные отчеты в нескольких форматах"
    exclude: "DOCX"
    description: ".NET позволяет вам генерировать документы с интегрированными графиками в более чем 50 поддерживаемых форматах, без проблем комбинируя шаблоны с вашими данными."
    items: 
          
        # format loop 1
        - name: "Диаграммы в PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Диаграммы в DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Диаграммы в PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Диаграммы в XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---