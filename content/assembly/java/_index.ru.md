---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Automation Assembly и API генератора динамических отчетов"
head_description: "Java API для автоматизации документов, сборки и отчетности. Создавайте отчеты из пользовательских шаблонов. Сборка PDF Word Excel PPTX HTML из источников данных DB, JSON, OДата и XML."

############################# Header ############################
title: "Java API для автоматизации документов и отчетов"
description: "Создание приложений автоматизации документов для получения данных; поместите его в настраиваемые шаблоны и создавайте динамические отчеты через Java API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "/border/groupdocs-assembly-java.svg"
        product: "GroupDocs.Assembly"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Обзор"

            # button loop
            - link: "#features"
              text: "Функции"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/assembly"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java API помогает быстро разрабатывать приложения для автоматизации документов и создания отчетов на Java для создания настраиваемых отчетов на основе шаблонов без установки какого-либо внешнего программного обеспечения. Механизм генерации отчетов извлекает данные из шаблона документа, собирает их и генерирует отчеты в указанном формате вывода в соответствии с заданным синтаксисом. Он позволяет динамически настраивать и вставлять свойства форматирования элементов шаблона и поддерживает различные источники данных (JSON, XML, OДата, базы данных, CSV, электронную таблицу в виде таблицы данных, таблицу обработки текста в виде таблицы данных и базы данных) для извлечения данных из.

      Библиотека сборки документов распознает несколько форматов документов и позволяет создавать шаблоны во всех поддерживаемых типах файлов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, листы Excel, презентации PowerPoint и текст. Он поддерживает синтаксис шаблона на основе LINQ, и пользователи также могут динамически настраивать и вставлять свойства форматирования элементов шаблона.

      GroupDocs.Assembly for Java легко интегрируется с новыми или существующими Java-приложениями. Он полностью совместим со всеми версиями Java и поддерживает популярные операционные системы (Windows, линукс, MacOS), способные запускать среду выполнения Java.

    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приведен обзор GroupDocs.Assembly для Java:

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Обзор"
          content: |
            * Формулировка данных
            * Форматирование данных
            * Автоматизация данных
            * Создать шаблон
            * Форматирование элемента шаблона
            * Генерация отчета
      
      ## TAB TWO ##
      tab_two:
        description: |
          Ниже перечислены поддерживаемые [форматы файлов документов](https://docs.groupdocs.com/assembly/java/supported-document-formats/) для API создания документов Java.

        left:
          enable: true
          table:
            # table loop
            - title: "Форматы Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            # table loop
            - title: "Поддерживаемые источники данных"
              content: |
                * База данных
                * XML
                * OДата
                * JSON
                * CSV
                * Пользовательские объекты .NET
                * Электронная таблица как таблица данных
                * Таблица обработки текстов как таблица данных

        right:
          enable: true
          table:
            # table loop
            - title: "Другие форматы"
              content: |
                * **OpenOffice Document Formats**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **Markdown Документация File**: MD
                * **Other**: TXT

            # table loop
            - title: "Поддержка межформатной сборки"
              content: |
                * Обработка текстов **TO** Обработка текстов, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Электронная таблица **TO** Электронная таблица, HTML, PDF, XPS, TIFF, MHTML
                * Презентация **TO** Презентация, HTML, PDF, XPS, TIFF
                * Электронная почта **TO** Обработка текстов, электронная почта, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML и TXT **TO** Обработка текстов, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Assembly for Java supports following Операционные системы, Frameworks & Менеджер пакетовs:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Microsoft Windows
                * Сервер Microsoft Windows
                * линукс
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * Java 7 (1.7) и выше

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Среды разработки"
              content: |
                * NetBeans
                * IntelliJ ИДЕЯ
                * Затмение
            # table loop
            - icon: "fas fa-tools"
              title: "Инструмент автоматизации сборки"
              content: |
                * Мавен

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Assembly для функций Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Настройка изображения в текстовом поле Word, Excel, презентаций и электронных писем с сохранением соотношения сторон изображения"

      # feature loop
      - icon: "fas fa-eye"
        content: "Используйте формулы и выполняйте последовательные операции с данными — применяйте формулу во время сборки электронной таблицы"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Применение форматирования Upper, Lower, Capital, FirstCap к строкам в синтаксисе шаблона"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Поддержка синтаксиса шаблона Форматирование порядкового, кардинального, алфавитно-числового характера"

      # feature loop
      - icon: "fas fa-code"
        content: "Поддержка шаблонов документов с пользовательскими переменными и текстовыми комментариями в тегах синтаксиса шаблона"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Динамически вставлять содержимое документа в отчет"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Динамическая настройка цвета фона HTML-документов и создание штрих-кода в отчетах"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Динамически вставляйте гиперссылки в отчеты и применяйте атрибуты к телу сообщения электронной почты"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Динамическое вложение вложений электронной почты и обновление полей во время сборки документа Word Processing"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Поддержка NEXT Field Аналог Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Динамическое добавление ссылок и закладок в форматы документов и присвоение имен диапазонам ячеек электронных таблиц Excel"

      # feature loop
      - icon: "fas fa-columns"
        content: "Загрузка и сохранение собранных форматов презентационных документов POT и OTP"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Форматирование шаблона для числовых, текстовых, графических, датовых и графических элементов"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Динамическая вставка изображений и документов из байтов в кодировке Base64"

      # feature loop
      - icon: "fas fa-print"
        content: "Синтаксис шаблона на основе LINQ"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Изменить формат собранного файла, используя явные спецификации или расширение файла"

      # feature loop
      - icon: "fas fa-lock"
        content: "Упорядоченный список поддерживается для Markdown - Сохраняйте недавно собранные электронные письма и документы Word в Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Создание различных типов отчетов, например, диаграмм, изображений, таблиц, списков и т. д."
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Синтаксические ошибки встроенного шаблона в сгенерированных документах вместо создания исключений"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Динамический перезапуск нумерованного списка в документах Word, а также электронных писем с телами HTML и RTF"

      # feature loop
      - icon: "fas fa-heading"
        content: "Поддержка таблиц, автоссылок, встроенных ссылок и изображений для собранных документов Markdown"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Динамическое создание штрих-кодов (расширенный купон GS1-128 AI 8102 и купон UPCA и GS1 Databar)"

      # feature loop
      - icon: "fas fa-cube"
        content: "Загружайте шаблоны документов из HTML с помощью ресурсов и сохраняйте собранные документы Word, Excel, PowerPoint и электронные письма в HTML с помощью ресурсов"

    больше_функций:
      # more_feature_loop
      - title: "Управление элементами шаблона"
        content: |
          Управляйте многочисленными элементами шаблона с помощью API GroupDocs.Assembly для Java. Элементы шаблона, с которыми вы можете работать, включают текстовые блоки, изображения, гиперссылки, блоки HTML, штрих-коды (через шрифты штрих-кода) и диаграммы. Вы также можете применять повторяющиеся блоки и условные блоки для элементов списка и строк таблицы. Динамическое объединение ячеек таблицы, содержащих один и тот же текст, на основе шаблонных выражений для документов, презентаций, электронных таблиц и электронных писем с текстами HTML и RTF.
      
      # more_feature_loop
      - title: "Работа со списками отчетов"
        content: |
          Используя GroupDocs.Assembly for Java API, поддерживаются следующие типы отчетов списка:

          * Маркированный список
          * Нумерованный список
          * Colored Нумерованный список

      # more_feature_loop
      - title: "Манипулировать отчетами диаграммы"
        content: |
          GroupDocs.Assembly для Java поддерживает следующие типы отчетов в виде диаграмм:

          * Пузырьковая диаграмма, которая отображает три измерения данных
          * Столбчатая диаграмма
          * Круговая диаграмма
          * Точечная диаграмма
          * Диаграмма серии (цветная)

      # more_feature_loop
      - title: "Манипуляции с табличными отчетами"
        content: |
          GroupDocs.Assembly для Java поддерживает следующие типы табличных отчетов:

          * Таблица Master-Detail
          * Таблица с выделенными строками
          * Таблица с альтернативным содержимым
          * Таблица с фильтрацией, группировкой и упорядочением

          Вы также можете использовать полосы данных в строках таблицы.

      # more_feature_loop
      - title: "Манипулировать отчетами диаграммы"
        content: |
          Интеграция GroupDocs.Assembly for Java API с вашим Java-приложением очень проста. Ниже приведен пример блока кода, который генерирует отчет в формате OpenDocument с использованием Java: 

          ```java
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Assembly предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "/border/groupdocs-assembly-net.svg"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---