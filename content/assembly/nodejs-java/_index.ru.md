---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
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
head_title: "{index-content-nodejs-java.head_title}"
head_description: "{index-content-nodejs-java.head_description}"

############################# Header ############################
title: "{index-content-nodejs-java.title}"
description: "{index-content-nodejs-java.description}"
words:
  for: "для"

actions:
  main: "{index-content-nodejs-java.actions_main}"
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
  title: "{index-content-nodejs-java.code_title}"
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
  description: "{index-content-nodejs-java.overview_description}"
  features:
    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_1.title}"
      content: "{index-content-nodejs-java.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_2.title}"
      content: "{index-content-nodejs-java.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_3.title}"
      content: "{index-content-nodejs-java.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформенная независимость"
  description: "{index-content-nodejs-java.platforms_description}"
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
    {index-content-nodejs-java.formats_description}
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
  title: "{index-content-nodejs-java.features.title}"
  description: "{index-content-nodejs-java.features.description}"

  items:
    # feature loop
    - icon: "preview"
      title: "{index-content-nodejs-java.features.feature_1.title}"
      content: "{index-content-nodejs-java.features.feature_1.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_2.title}"
      content: "{index-content-nodejs-java.features.feature_2.content}"

    # feature loop
    - icon: "two_pages"
      title: "{index-content-nodejs-java.features.feature_3.title}"
      content: "{index-content-nodejs-java.features.feature_3.content}"

    # feature loop
    - icon: "document_settings"
      title: "{index-content-nodejs-java.features.feature_4.title}"
      content: "{index-content-nodejs-java.features.feature_4.content}"

    # feature loop
    - icon: "text"
      title: "{index-content-nodejs-java.features.feature_5.title}"
      content: "{index-content-nodejs-java.features.feature_5.content}"

    # feature loop
    - icon: "add"
      title: "{index-content-nodejs-java.features.feature_6.title}"
      content: "{index-content-nodejs-java.features.feature_6.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_7.title}"
      content: "{index-content-nodejs-java.features.feature_7.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-nodejs-java.features.feature_8.title}"
      content: "{index-content-nodejs-java.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-nodejs-java.features.feature_9.title}"
      content: "{index-content-nodejs-java.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
        ```java {style=abap}
        // Вставьте этот шаблон на страницу документа:
        // Индикаторы производительности менеджеров
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Укажите путь к шаблону
        String template = "Bulleted List Template.docx";

        // Установите путь к выходному файлу
        String result = "Result Report.docx"

        // Получите данные менеджеров из источника JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Сгенерируйте отчет с заполненными данными
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
        ```java {style=abap}   
        // Добавьте шаблон заголовка диаграммы в презентацию:
        // Доходы клиентов <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Также включите шаблон данных диаграммы:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Укажите путь к шаблону диаграммы
        String template = "Pie Chart Template.pptx";

        // Установите путь к выходному файлу
        String result = "Result Report.pptx"

        // Получите данные клиентов из источника XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Сгенерируйте диаграмму и сохраните результат
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---