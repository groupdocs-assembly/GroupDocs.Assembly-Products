---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: ru
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Инструментарий Node.js для создания, автоматизации и настройки документов"
head_description: "Библиотека Node.js для автоматизации рабочих процессов с документами. Генерируйте файлы PDF, Word, Excel, PowerPoint, HTML и электронную почту из своих шаблонов."

############################# Header ############################
title: "API Node.js для упрощенной автоматизации документов и отчетов"
description: "Оптимизируйте генерацию отчетов на JavaScript, объединяя ваши данные с заранее созданными шаблонами."
words:
  for: "для"

actions:
  main: "Начните пробный период на NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Assembly бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Смотрите, что нового"
  downloads: "Загрузки"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Создание диаграммы в документе Word с использованием Node.js"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Путь к основному шаблону
    const template = "chart_template.docx";

    // Получите данные о продуктивности менеджеров из источника
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Создайте экземпляр DataSourceInfo с данными
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Установите цвета диаграммы, используя другой DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Заполните шаблон данными и сохраните его на выходе
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Assembly"
  description: "Библиотека Node.js для программного создания документов с интегрированной обработкой данных."
  features:
    # feature loop
    - title: "Интеграция бизнес-данных в шаблоны с помощью JavaScript"
      content: "Генерируйте качественные отчеты, встраивая JSON, XML или другие данные в шаблоны с использованием GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Управление встроенным контентом"
      content: "Автоматически заполняйте таблицы, диаграммы и другие визуальные элементы в ваших документах с помощью внешних данных."

    # feature loop
    - title: "Настраиваемые параметры"
      content: "GroupDocs.Assembly for Node.js via Java позволяет добавлять функции, такие как штрих-коды, извлечение данных из URL и экспорт файлов в различных форматах."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформенная независимость"
  description: "GroupDocs.Assembly for Node.js via Java без проблем интегрируется с ведущими операционными системами, фреймворками и менеджерами пакетов."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Assembly for Node.js via Java поддерживает широкий спектр [форматов документов](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Форматы Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Изображения и другие форматы
        * **Портативный:** PDF
        * **Изображения:** SVG, TIFF
        * **Другие офисные форматы:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Другие форматы
        * **Веб:** HTML, MHTML
        * **Электронные письма:** EML, MSG, EMLX
        * **Другое:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Ключевые функции GroupDocs.Assembly"
  description: "Создавайте динамические документы и отчеты с мощными инструментами управления данными."

  items:
    # feature loop
    - icon: "preview"
      title: "Насыщенные визуальные данные"
      content: "Интегрируйте диаграммы, таблицы, изображения и списки в ваши документы с полной настройкой."

    # feature loop
    - icon: "manipulate"
      title: "Преобразование ваших данных"
      content: "Используйте инструменты, такие как формулы и сортировка, для структурирования и отображения информации эффективно."

    # feature loop
    - icon: "two_pages"
      title: "Широкая совместимость форматов"
      content: "Работайте без проблем с популярными форматами файлов для шаблонов и выходных данных."

    # feature loop
    - icon: "document_settings"
      title: "Расширенная настройка шаблонов"
      content: "Форматируйте шаблоны с числовыми, алфавитными и другими стилевыми опциями."

    # feature loop
    - icon: "text"
      title: "Динамическая генерация штрих-кодов"
      content: "Создавайте и встраивайте изображения штрих-кодов прямо в ваши документы по запросу."

    # feature loop
    - icon: "add"
      title: "Гибкое стилизация текста"
      content: "Применяйте текстовые стили, такие как прописные или заглавные буквы, в ваших шаблонах."

    # feature loop
    - icon: "manipulate"
      title: "Динамическая вставка контента"
      content: "Включайте контент из внешних файлов динамически во время генерации документа."

    # feature loop
    - icon: "convert"
      title: "Экспорт в различные форматы"
      content: "Сохраняйте документы в нескольких форматах с вашими указанными конфигурациями."

    # feature loop
    - icon: "update"
      title: "Динамическая интеграция медиа"
      content: "Вставляйте изображения или другие элементы, используя данные Base64 при создании документов."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Изучите практические примеры использования GroupDocs.Assembly для выполнения распространенных задач."
  items:
    # code sample loop
    - title: "Добавление маркированного списка в документы Word"
      content: |
        Узнайте, как создать [маркированные списки](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) в документах Word для эффективной организации данных. Этот пример демонстрирует, как сгенерировать маркированный список с использованием GroupDocs.Assembly.
        {{< landing/code title="Добавление маркированного списка в документы Word">}}
        ```javascript {style=abap}
        // Вставьте этот шаблон на страницу документа:
        // Индикаторы производительности менеджеров
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Укажите путь к шаблону
        const template = "Bulleted List Template.docx";

        // Установите путь к выходному файлу
        const result = "Result Report.docx"

        // Получите данные менеджеров из источника JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Сгенерируйте отчет с заполненными данными
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Вставка круговых диаграмм в PowerPoint"
      content: |
        Узнайте, как использовать шаблоны и XML для добавления [круговых диаграмм](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) в ваши презентации. Улучшите ваши отчеты с круговыми диаграммами для визуального и четкого представления данных.
        {{< landing/code title="Вставка круговых диаграмм в PowerPoint">}}
        ```javascript {style=abap} 
        // Добавьте шаблон заголовка диаграммы в презентацию:
        // Доходы клиентов <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Также включите шаблон данных диаграммы:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Укажите путь к шаблону диаграммы
        const template = "Pie Chart Template.pptx";

        // Установите путь к выходному файлу
        const result = "Result Report.pptx"

        // Получите данные клиентов из источника XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Сгенерируйте диаграмму и сохраните результат
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---