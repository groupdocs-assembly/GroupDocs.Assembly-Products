



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: ru
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Встраивание одного документа в другой в формате XLSX с помощью API C#"
head_description: "Объединяйте документы XLSX с помощью C#. С GroupDocs.Assembly объединим файлы без усилий всего за несколько шагов."

############################# Header ############################
title: "Объединяйте документы в формате XLSX" 
description: "С помощью GroupDocs.Assembly for .NET вы можете быстро встроить один документ XLSX в другой. Этот API предоставляет мощные инструменты для точного объединения документов."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Что такое GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) — это мощный инструмент для составления и обработки документов. Он позволяет пользователям встраивать один документ в другой, обеспечивая бесшовное объединение контента. С поддержкой более 50 форматов — включая PDF, файлы MS Office и многое другое — вы можете организовать, редактировать и настраивать конечный результат в соответствии с вашими требованиями.

############################# Steps ############################
steps:
    enable: true
    title: "Как встроить документ в файл XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) позволяет вам без труда вставить один документ в другой файл XLSX. Объединяйте и настраивайте контент с точностью.
      
      1. Создайте шаблон XLSX с заполнителями для встраиваемого документа.
      2. Определите путь к файлу шаблона.
      3. Укажите путь к документу для встраивания.
      4. Сохраните окончательный файл с интегрированным контентом.
   
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
        // Добавьте этот тег в ваш шаблон, чтобы отметить точку вставки
        // <<doc [doc_expression]>>

        // Укажите путь к файлу шаблона
        string template = "doc_template.xlsx";

        // Укажите путь документа для встраивания
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // Сохраните объединенный документ
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Оптимизируйте объединение документов с помощью продвинутых инструментов"
  description: "Библиотека GroupDocs.Assembly for .NET упрощает встраивание одного документа в другой, поддерживая различные форматы файлов и предлагая настройки для бесшовной интеграции."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Ключевые особенности GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерация отчетов из бизнес-данных"
      content: "Автоматически заполняйте документы данными из JSON, XML, CSV или других источников, обеспечивая точные и эффективные рабочие процессы."

    # feature loop
    - title: "Обогащайте документы визуальными элементами"
      content: "GroupDocs.Assembly позволяет включать таблицы, графики и списки, а также текст, ссылки, изображения и динамически создаваемые штрих-коды."

    # feature loop
    - title: "Точно размещайте и форматируйте данные"
      content: "Шаблоны на основе LINQ предоставляют вам контроль над размещением данных, позволяют обрабатывать циклы для массивов и позволяют настраивать стиль, включая изменение цвета."

    # feature loop
    - title: "Работа с несколькими форматами файлов"
      content: "Просто встраивайте документы друг в друга в таких форматах, как MS Office, PDF, HTML, OpenOffice и других."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как программно встроить изображение в документ"
      content: |
        Этот пример демонстрирует, как вставить изображение в документ XLSX с использованием GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Добавьте тег-заполнитель в ваш шаблон
          // <<image [expression]>>

          // Укажите путь к файлу шаблона
          string template = "template.xlsx";

          // Установите путь к файлу изображения
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Инициализируйте экземпляр DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Сохраните документ с встроенным изображением
          asm.AssembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "Откройте для себя наши мощные инструменты"
    exclude: "document"
    description: "Изучите возможности, которые предлагает GroupDocs.Assembly для встраивания и объединения документов с точностью."
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Объединяйте документы в различных форматах"
    exclude: "XLSX"
    description: "С помощью API .NET вы можете комбинировать документы более чем в 50 поддерживаемых форматах. Легко встраивайте файлы или разделы в ваши окончательные документы."
    items: 
          
        # format loop 1
        - name: "Вставить документ в PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Вставить документ в DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Вставить документ в PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Вставить документ в XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---