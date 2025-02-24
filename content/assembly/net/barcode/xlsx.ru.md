



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: ru
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Генерация штрих-кодов в документах XLSX с помощью C#"
head_description: "API GroupDocs.Assembly for .NET позволяет разработчикам динамически создавать и встраивать изображения штрих-кодов в документы и электронные письма."

############################# Header ############################
title: "Добавьте штрих-коды в документы XLSX с помощью нашего API .NET" 
description: "GroupDocs.Assembly for .NET полностью поддерживает создание и встраивание штрих-кодов в документы XLSX динамически."
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
       [GroupDocs.Assembly for .NET](/assembly/net/) разработан, чтобы помочь вам генерировать документы и отчеты, интегрируя данные из множества источников. Заполняйте документы текстом или числовыми данными, создавайте диаграммы, таблицы и списки или вставляйте изображения и штрих-коды на лету. Используйте расширенный разметку для точного размещения данных. Поддерживает более 50 форматов, включая PDF, файлы MS Office и электронные письма.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для добавления сгенерированного штрих-кода в документ XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) упрощает вставку штрих-кодов в шаблоны в таких форматах, как XLSX. Поддерживает более 60 типов штрих-кодов, включая одноразмерные и двумерные форматы.
      
      1. Подготовьте шаблон XLSX с заполнителями для штрих-кодов.
      2. Получите данные из любого поддерживаемого источника данных.
      3. Настройте дополнительные параметры, такие как размер или разрешение штрих-кода.
      4. Сохраните шаблон с штрих-кодом как новый документ.
   
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
        // Вставьте этот тег в ваш шаблон для генерации штрих-кода в итоговом документе
        // <<barcode [barcode_expression] -barcode_type>>

        // Укажите путь к файлу шаблона
        string template = "barcode_template.xlsx";

        // Получите данные из вашего источника
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Сохраните документ с сгенерированным штрих-кодом
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Генерация документов путем заполнения шаблонов данными"
  description: "GroupDocs.Assembly for .NET создан для упрощения создания документов в популярных форматах. Добавляйте диаграммы, списки, таблицы, гиперссылки, изображения и штрих-коды с помощью расширенных шаблонов и разметки."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Особенности GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Создание отчетов на основе бизнес-данных"
      content: "Наш API эффективно заполняет документы в популярных офисных форматах, используя данные из таких источников, как JSON, XML и CSV."

    # feature loop
    - title: "Использование визуальных элементов для отображения данных"
      content: "GroupDocs.Assembly поддерживает встраивание нативных элементов, таких как списки, таблицы и диаграммы, наряду с текстом, гиперссылками, изображениями и динамически создаваемыми штрих-кодами."

    # feature loop
    - title: "Вставка данных в любом месте документа"
      content: "Используйте синтаксис на основе LINQ для точного размещения данных в нужных местах. Массивы могут быть вставлены с помощью циклов for-each, а форматирование (например, цвет) можно настраивать программно."

    # feature loop
    - title: "Поддерживает широкий спектр форматов"
      content: "Обрабатывайте популярные форматы файлов, такие как MS Office, OpenOffice, PDF, HTML и различные форматы электронных писем. Вставляйте один документ в другой по мере необходимости."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как динамически генерировать штрих-код"
      content: |
        Этот пример демонстрирует встраивание динамически сгенерированного штрих-кода в документ XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Используйте этот шаблон для вставки штрих-кода в документ
          // <<barcode [barcode_expression] -barcode_type>>

          // Укажите путь к файлу шаблона
          string template = "barcode_template.xlsx";

          // Получите данные из вашего выбранного источника
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Создайте объект источника данных только с необходимыми данными
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Инициализируйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Настройте дополнительные свойства штрих-кода
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // Сохраните финальный документ с встраиваемым штрих-кодом
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    exclude: "barcode"
    description: "Наше решение разработано для оптимизации обработки бизнес-документов."
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
    title: "Создание отчетов в популярных форматах"
    exclude: "XLSX"
    description: ".NET поддерживает генерацию отчетов более чем в 50 форматах, позволяя вам бесшовно объединять данные и шаблоны для выдающихся результатов."
    items: 
          
        # format loop 1
        - name: "Добавить штрих-код в PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Добавить штрих-код в DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Добавить штрих-код в PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Добавить штрих-код в XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---