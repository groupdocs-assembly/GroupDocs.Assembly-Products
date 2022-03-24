---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API для автоматизации документов, сборки и создания отчетов"
head_description: "C# .NET Автоматизация документов, сборка и создание отчетов API. Создавайте PDF, Word, Excel, PPTX, HTML и электронные документы из пользовательских шаблонов.."

############################# Header ############################
title: ".NET API автоматизации документов и отчетности"
description: "Создание отчетов в приложениях .NET путем определения шаблонов и объединения данных."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "/border/groupdocs-assembly-net.svg"
        product: "GroupDocs.Assembly"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for .NET API помогает создавать мощные приложения для автоматизации документов и создания отчетов с возможностью создания отчетов на основе настраиваемых шаблонов в C#, ASP.NET и других приложениях, связанных с .NET. С помощью всего нескольких строк кода библиотека отчетов .NET интеллектуально собирает заданные данные из определенного шаблона документа и создает красивые отчеты в предпочтительном формате вывода, извлекая данные из различных источников данных (базы данных, XML, JSON, ODATA, CSV, Пользовательские объекты .NET).

      Он поддерживает синтаксис шаблонов на основе LINQ, и пользователи могут легко создавать выходные документы во всех широко используемых форматах бизнес-файлов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, листы Excel, презентации и слайды PowerPoint. Свойства форматирования для элементов шаблона также можно настроить, манипулируя текстом, HTML и условными блоками, изображениями, диаграммами, штрих-кодами, гиперссылками, сводными таблицами и т. д.

      GroupDocs.Assembly для .NET можно использовать для разработки приложений в любой среде разработки, предназначенной для платформы .NET. Он совместим со всеми языками на базе .NET и поддерживает популярные операционные системы (Windows, линукс, MacOS), на которые можно установить Mono или .NET framework (включая .NET Core).

    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приведен обзор GroupDocs.Assembly для .NET:
      
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
          Ниже перечислены поддерживаемые [форматы файлов документов](https://docs.groupdocs.com/assembly/net/supported-document-formats/) для API создания документов .NET.

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
          GroupDocs.Assembly for .NET поддерживает следующие Операционные системы, Frameworks & Менеджер пакетовs:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Windows
                * Windows-сервер
                * Windows Azure
                * линукс

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * .NET Framework 2.0 или выше
                * Монофреймворк 1.2 или выше

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Менеджер пакетов"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Среды разработки"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * МоноДевелопмент

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Assembly для функций .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Работает с несколькими форматами данных"

      # feature loop
      - icon: "fas fa-eye"
        content: "Возможность манипулировать данными с использованием формул и последовательных операций с данными"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Отформатируйте строки в синтаксисе шаблона так, чтобы они были Upper, Lower, Capital, FirstCap"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Выполнение порядкового, кардинального, алфавитно-числового форматирования в синтаксисе шаблона"

      # feature loop
      - icon: "fas fa-code"
        content: "Определение переменных в документах шаблона и поддержка текстовых комментариев в тегах синтаксиса шаблона"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Динамически вставляйте содержимое внешних документов в свои отчеты"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Динамическое создание изображения штрих-кода в отчетах и установка цвета фона для документов HTML"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Динамически назначать атрибуты телу сообщения электронной почты и вставлять гиперссылки в отчеты"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Динамическое создание вложений в сообщения электронной почты"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Поддержка аналога поля Microsoft Word NEXT"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Обновление полей при сборке документов Word Processing"

      # feature loop
      - icon: "fas fa-columns"
        content: "Вычислить формулу при сборке электронных таблиц"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Формат Числовой, Текстовый, Изображение, Диаграмма, Элементы Дата-Время Шаблона"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Загрузка и сохранение собранных форматов презентационных документов POT и OTP"

      # feature loop
      - icon: "fas fa-print"
        content: "Использование синтаксиса на основе LINQ для шаблона и выполнение условного форматирования текста элементов шаблона"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Измените формат файла собранного документа, используя расширение файла или явные спецификации"

      # feature loop
      - icon: "fas fa-lock"
        content: "Упорядоченный список поддерживается для Markdown - Сохраняйте недавно собранные электронные письма и документы Word в Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Поддерживает отчеты различных типов, например, диаграммы, списки, таблицы, изображения и т. д."
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Синтаксические ошибки встроенного шаблона в сгенерированных документах вместо создания исключений"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Загружайте шаблоны документов из HTML с помощью ресурсов и сохраняйте собранные документы Word, Excel, PowerPoint и электронные письма в HTML с помощью ресурсов"

      # feature loop
      - icon: "fas fa-heading"
        content: "Динамическое добавление нумерации списка перезапуска в форматах документов Word и электронной почте с телами HTML и RTF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Динамическая вставка изображений и документов из байтов в кодировке Base64 and adjust checkbox value settings of Word documents"

      # feature loop
      - icon: "fas fa-cube"
        content: "Растянуть изображение в текстовом поле Word, Excel, презентаций и электронных писем с сохранением соотношения сторон изображения"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Динамическое добавление ссылок и закладок в форматы документов и присвоение имен диапазонам ячеек электронных таблиц Excel"

    больше_функций:
      # more_feature_loop
      - title: "Поддержка элементов шаблона"
        content: |
          GroupDocs.Assembly for .NET API дает вам возможность работать с многочисленными элементами шаблона. Вы можете работать с блоками форматированного текста, блоками HTML, изображениями, диаграммами, гиперссылками и штрих-кодами (через шрифты штрих-кода). Также поддерживаются повторяющиеся блоки и условные блоки, включая элементы списка и строки таблицы. Вы также можете динамически объединять ячейки таблицы, содержащие один и тот же текст, на основе шаблонных выражений для электронных таблиц, презентаций, документов и электронных писем с телами HTML и RTF.

      # more_feature_loop
      - title: "Работа со списками отчетов"
        content: |
          С помощью GroupDocs.Assembly for .NET API вы можете работать со списками отчетов следующих трех типов:

          * Маркированный список
          * Нумерованный список
          * Colored Нумерованный список

      # more_feature_loop
      - title: "Работа с отчетами в виде диаграмм"
        content: |
          GroupDocs.Assembly для .NET поддерживает следующие типы отчетов в виде диаграмм:

          * Пузырьковая диаграмма, которая отображает три измерения данных
          * Столбчатая диаграмма
          * Круговая диаграмма
          * Точечная диаграмма
          * Диаграмма серии (цветная)

      # more_feature_loop
      - title: "Работа с табличными отчетами"
        content: |
          GroupDocs.Assembly для .NET поддерживает следующие типы табличных отчетов:

          * Таблица Master-Detail
          * Таблица с выделенными строками
          * Таблица с альтернативным содержимым
          * Таблица с фильтрацией, группировкой и упорядочением
          
          Вы также можете использовать полосы данных в строках таблицы.

      # more_feature_loop
      - title: "Простая интеграция"
        content: |
          Вы можете легко интегрировать GroupDocs.Assembly for .NET API с вашим .NET-приложением, написав всего несколько строк кода. Ниже приведен пример кода для создания отчета в открытом документе. format:

          ```cs
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
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
        - img_alt: "GroupDocs.Assembly for Java"
          image: "/border/groupdocs-assembly-java.svg"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
