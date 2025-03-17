---
############################# Static ############################
layout: "landing"
date: 2025-03-17T13:11:12
draft: false

lang: ru
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: ".NET API для автоматизации документов, сборки и генерации отчетов"
head_description: "C# .NET API для автоматизации документов, сборки и генерации отчетов. Создавайте документы PDF, Word, Excel, PPTX, HTML и электронные письма из пользовательских шаблонов."

############################# Header ############################
title: ".NET API для автоматизации документов и отчетности"
description: "Генерируйте отчеты в приложениях .NET, определяя шаблоны и объединяя данные."
words:
  for: "для"

actions:
  main: "Скачать пробную версию через Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Assembly бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Смотрите, что нового"
  downloads: "Загрузки"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Заполнение диаграммы в DOCX с помощью C#"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Путь к основному шаблону
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Assembly"
  description: ".NET решение для автоматизации создания документов с передовой интеграцией данных."
  features:
    # feature loop
    - title: "Добавление бизнес-данных в шаблоны документов с помощью C#"
      content: "Генерация отчетов стала проще: с GroupDocs.Assembly for .NET вы можете без усилий вставить данные из источников, таких как JSON или XML, в предопределенные шаблоны."

    # feature loop
    - title: "Обработка нативных объектов данных"
      content: "Поддерживаемые типы документов включают встраиваемые объекты, такие как диаграммы, графики, таблицы и списки, которые могут быть автоматически заполнены данными."

    # feature loop
    - title: "Дополнительные функции"
      content: "GroupDocs.Assembly for .NET предоставляет широкие возможности настройки. Программно создавайте объекты данных, генерируйте штрих-коды, используйте онлайн-источники данных через URL и сохраняйте выходные данные в различных форматах."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформенная независимость"
  description: "GroupDocs.Assembly for .NET совместим с следующими операционными системами, фреймворками и менеджерами пакетов."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Assembly for .NET может обрабатывать следующие [форматы файлов](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "Функции GroupDocs.Assembly"
  description: "Создавайте документы и отчеты с использованием передовых моделей данных."

  items:
    # feature loop
    - icon: "preview"
      title: "Расширенное представление данных"
      content: "Поддерживает широкий спектр объектов данных, таких как графики, списки, таблицы, изображения и прочее."

    # feature loop
    - icon: "manipulate"
      title: "Манипуляция данными"
      content: "Применяйте формулы и последовательные операции для форматирования и эффективного отображения данных."

    # feature loop
    - icon: "two_pages"
      title: "Широкий спектр поддерживаемых форматов"
      content: "Беспрепятственно работайте со всеми обычными форматами документов для шаблонов или выходных файлов."

    # feature loop
    - icon: "document_settings"
      title: "Богатая разметка шаблона"
      content: "Используйте порядковое, кардинальное и алфавитное числовое форматирование в шаблонах."

    # feature loop
    - icon: "text"
      title: "Встраивание штрих-кодов"
      content: "Динамически генерируйте изображения штрих-кодов и вставляйте их в ваши документы."

    # feature loop
    - icon: "add"
      title: "Форматирование данных"
      content: "Форматируйте строки в шаблонах в верхнем регистре, нижнем регистре, с заглавной буквой или в других стилях."

    # feature loop
    - icon: "manipulate"
      title: "Манипуляция содержимым документа"
      content: "Динамически вставляйте содержимое из внешних документов в ваши отчеты."

    # feature loop
    - icon: "convert"
      title: "Сохранение в нескольких форматах"
      content: "Укажите формат выходного файла, используя расширения файла или подробные конфигурации."

    # feature loop
    - icon: "update"
      title: "Гибкая обработка данных"
      content: "Динамически вставляйте изображения и документы, используя байты, закодированные в Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Примеры кода для типичных операций GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "С ненумерованным списком в документе Microsoft Word"
      content: |
        [Ненумерованные списки](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) являются распространенным способом представления бизнес-данных. Вот пример добавления списка в документ Word с использованием GroupDocs.Assembly.
        {{< landing/code title="Как заполнить список в документах">}}
        ```csharp {style=abap}
        // Вставьте этот шаблон на страницу документа:
        // Индикаторы производительности менеджеров
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Укажите путь к шаблону
        string template = "Bulleted List Template.docx";

        // Установите путь к выходному файлу
        string result = "Result Report.docx"

        // Получите данные менеджеров из источника JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Сгенерируйте отчет с заполненными данными
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Круговые диаграммы в презентациях PPTX"
      content: |
        Вы можете создавать [круговые диаграммы](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) с помощью шаблонов и данных XML. Улучшите свои отчеты с помощью визуально привлекательных представлений данных.
        {{< landing/code title="Как представить данные в круговой диаграмме">}}
        ```csharp {style=abap}
        // Добавьте шаблон заголовка диаграммы в презентацию:
        // Доходы клиентов <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Также включите шаблон данных диаграммы:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Укажите путь к шаблону диаграммы
        string template = "Pie Chart Template.pptx";

        // Установите путь к выходному файлу
        string result = "Result Report.pptx"

        // Получите данные клиентов из источника XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Сгенерируйте диаграмму и сохраните результат
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---