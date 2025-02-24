



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: ru
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Генерация списков в документах DOCX с помощь C#"
head_description: "API GroupDocs.Assembly for .NET позволяет разработчикам динамически создавать и встраивать заполненные данными списки в документы и шаблоны."

############################# Header ############################
title: "Добавьте списки на основе данных в документы DOCX с использованием нашего API .NET" 
description: "GroupDocs.Assembly for .NET предлагает мощные инструменты для динамической генерации и встраивания списков в документы DOCX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатную пробную версию"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Обзор GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) разработан для упрощения создания документов и отчетов за счет бесшовной интеграции данных из различных источников. Заполняйте шаблоны списками, диаграммами, таблицами, штрих-кодами или текстом и точно размещайте содержимое с помощью расширенного разметки. С поддержкой более 50 форматов, включая PDF, файлы MS Office и электронные письма, он идеален для автоматизации рабочих процессов документов.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для добавления списка с данными в документ DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) упрощает вставку списков, основанных на данных, в шаблоны DOCX. Создавайте и настраивайте списки без лишних проблем.
      
      1. Подготовьте шаблон DOCX с заполнителями для списка.
      2. Установите путь к шаблону.
      3. Получите данные из поддерживаемых источников, таких как JSON или XML.
      4. Сохраните окончательный документ с встроенным списком.
   
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
        // Добавьте этот тег в ваш шаблон, чтобы указать, где будет отображаться список
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Укажите путь к файлу шаблона
        string template = "list_template.docx";

        // Извлеките данные из вашего выбранного источника
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Сохраните документ с сгенерированным списком
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Создавайте документы, заполняя шаблоны структурированными данными"
  description: "GroupDocs.Assembly for .NET упрощает создание документов, основанных на данных. Динамически добавляйте списки, таблицы, штрих-коды, диаграммы, изображения и другие элементы с помощью расширенных шаблонов."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Функции GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерация отчетов на основе бизнес-данных"
      content: "API заполняет документы в популярных форматах, используя данные из источников, таких как JSON, XML, CSV и т.д., с точностью и эффективностью."

    # feature loop
    - title: "Используйте списки и другие элементы для представления данных"
      content: "GroupDocs.Assembly позволяет встраивать списки, таблицы и диаграммы вместе с текстом, штрих-кодами, гиперссылками и изображениями для создания хорошо структурированных документов."

    # feature loop
    - title: "Вставляйте данные точно в нужное место"
      content: "Используйте синтаксис на основе LINQ для точного позиционирования списков и других элементов данных. Используйте циклы для динамического заполнения списков и применяйте пользовательское форматирование программно."

    # feature loop
    - title: "Поддержка множества форматов документов"
      content: "Генерируйте и управляйте документами в различных форматах, таких как MS Office, OpenOffice, PDF, HTML и электронные письма. Легко интегрируйте несколько документов в один."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как динамически сгенерировать список"
      content: |
        Этот пример демонстрирует, как встроить динамически сгенерированный список в документ DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Добавьте тег-заполнитель в ваш шаблон для списка
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Укажите путь к файлу шаблона
          string template = "numlist_template.docx";

          // Извлеките данные для заполнения списка
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Создайте объект источника данных с необходимой информацией
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Инициализируйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Сохраните окончательный документ с сгенерированным списком
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "Изучите ключевые возможности"
    exclude: "list"
    description: "Наша платформа построена для упрощения создания и интеграции контента документов, основанного на данных."
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
    title: "Создание структурированных документов в популярных форматах"
    exclude: "DOCX"
    description: ".NET поддерживает более 50 форматов, позволяя вам бесшовно объединять данные и шаблоны для получения аккуратных, структурированных результатов."
    items: 
          
        # format loop 1
        - name: "Создать список в PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Создать список в DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Создать список в PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Создать список в XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---