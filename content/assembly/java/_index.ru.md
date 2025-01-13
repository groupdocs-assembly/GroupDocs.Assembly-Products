---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: ru
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

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
head_title: "Java-библиотека для создания, автоматизации документов и отчетности"
head_description: "Java-библиотека для автоматизации создания документов и генерации отчетов. Создавайте документы PDF, Word, Excel, PPTX, HTML и электронные письма с учетом пользовательских шаблонов."

############################# Header ############################
title: "Java API для автоматизации отчетов и документов"
description: "Упрощайте создание отчетов на Java, объединяя данные с шаблонами."
words:
  for: "для"

actions:
  main: "Получите пробную версию через Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Assembly бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Смотрите, что нового"
  downloads: "Загрузки"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Генерация диаграммы в DOCX с помощью Java"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Путь к основному шаблону
    String template = "chart_template.docx";

    // Получите данные о продуктивности менеджеров из источника
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Создайте экземпляр DataSourceInfo с данными
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Установите цвета диаграммы, используя другой DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Заполните шаблон данными и сохраните его на выходе
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Assembly"
  description: "Java-библиотека, разработанная для автоматизированного создания документов и бесшовной интеграции данных."
  features:
    # feature loop
    - title: "Объединение бизнес-данных в шаблоны с помощью Java"
      content: "Легко создавайте профессиональные отчеты, встраивая данные из JSON, XML или других источников в заранее спроектированные шаблоны с помощью GroupDocs.Assembly for Java."

    # feature loop
    - title: "Работа с встроенными объектами"
      content: "Автоматически заполняйте элементы, такие как таблицы, диаграммы и схемы, в документах, используя данные из внешних источников."

    # feature loop
    - title: "Расширенная настройка"
      content: "GroupDocs.Assembly for Java предлагает гибкие функции, такие как генерация штрих-кодов, получение онлайн-данных через URL и экспорт выходных данных в различных форматах."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформенная независимость"
  description: "GroupDocs.Assembly for Java хорошо работает с популярными операционными системами, фреймворками разработки и менеджерами пакетов."
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
    GroupDocs.Assembly for Java поддерживает широкий диапазон [форматов документов](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Ключевые возможности GroupDocs.Assembly"
  description: "Создавайте профессиональные документы и отчеты с продвинутой обработкой данных."

  items:
    # feature loop
    - icon: "preview"
      title: "Визуальные элементы данных"
      content: "Добавляйте и форматируйте такие элементы, как диаграммы, таблицы, изображения и списки непосредственно в ваших документах."

    # feature loop
    - icon: "manipulate"
      title: "Трансформация данных"
      content: "Используйте формулы, сортировку и другие инструменты для эффективной организации и представления ваших данных."

    # feature loop
    - icon: "two_pages"
      title: "Поддержка множества форматов"
      content: "Легко работайте с общими типами файлов как для шаблонов, так и для выходных файлов."

    # feature loop
    - icon: "document_settings"
      title: "Расширенное форматирование шаблонов"
      content: "Настраивайте шаблоны с числовыми, алфавитными и другими расширенными параметрами форматирования."

    # feature loop
    - icon: "text"
      title: "Динамическое создание штрих-кодов"
      content: "Быстро создавайте и вставляйте изображения штрих-кодов в документы по мере необходимости."

    # feature loop
    - icon: "add"
      title: "Гибкое форматирование текста"
      content: "Применяйте текстовые преобразования, такие как верхний регистр, нижний регистр, заглавная буква или другие стили в шаблонах."

    # feature loop
    - icon: "manipulate"
      title: "Импорт внешнего содержания"
      content: "Динамически включая содержимое из внешних файлов во время генерации документов."

    # feature loop
    - icon: "convert"
      title: "Экспорт в нескольких форматах"
      content: "Сохраняйте итоговые документы в различных форматах файлов, используя указанные расширения или конфигурации."

    # feature loop
    - icon: "update"
      title: "Динамическое встраивание медиа"
      content: "Вставляйте изображения или другие содержимое, используя данные в формате Base64 во время создания документов."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Изучите пример кода для обычных задач с GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Создать ненумерованный список в Word"
      content: |
        Узнайте, как добавлять [ненумерованные списки](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) в документы Word для организованного представления данных. Этот пример показывает, как сгенерировать список в Word с помощью GroupDocs.Assembly.
        {{< landing/code title="Создать ненумерованный список в Word">}}
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
    - title: "Создание круговых диаграмм в PPTX"
      content: |
        Используйте шаблоны и XML, чтобы добавить [круговые диаграммы](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) в ваши презентации. Сделайте ваши отчеты более увлекательными, включая круговые диаграммы для визуализации данных.
        {{< landing/code title="Создание круговых диаграмм в PPTX">}}
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