---
############################# Static ############################
layout: "landing"
date: 2025-01-16T13:04:06
draft: false

lang: uk
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
head_title: "Node.js інструмент для створення, автоматизації та налаштування документів"
head_description: "Бібліотека Node.js для автоматизації робочих процесів документів. Генеруйте PDF, Word, Excel, PowerPoint, HTML та електронні листи з ваших шаблонів."

############################# Header ############################
title: "API Node.js для спрощеної автоматизації документів та звітів"
description: "Оптимізуйте генерацію звітів на JavaScript, об'єднуючи ваші дані з заздалегідь створеними шаблонами."
words:
  for: "для"

actions:
  main: "Розпочніть свій безкоштовний trial на NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Assembly безкоштовно або запитайте ліцензію."

release:
  title: "Версія {0} випущена"
  notes: "Дивіться, що нового"
  downloads: "Завантаження"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Створити графік у документі Word за допомогою Node.js"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Шлях до основного шаблону
    const template = "chart_template.docx";

    // Отримайте дані продуктивності менеджерів з джерела
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Створіть екземпляр DataSourceInfo з даними
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Встановіть кольори діаграми, використовуючи інший DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Заповніть шаблон даними та збережіть його вихідним
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Assembly"
  description: "Бібліотека Node.js створена для програмного створення документів з інтегрованим обробленням даних."
  features:
    # feature loop
    - title: "Інтеграція бізнес-даних у шаблони з JavaScript"
      content: "Генеруйте вишукані звіти, вбудовуючи дані JSON, XML або інші дані у шаблони за допомогою GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Управління вбудованим контентом"
      content: "Автоматично заповнюйте таблиці, графіки та інші візуальні елементи у ваших документах за допомогою зовнішніх даних."

    # feature loop
    - title: "Налаштовувані параметри"
      content: "GroupDocs.Assembly for Node.js via Java дозволяє вам додавати функції, такі як штрих-коди, отримувати дані з URL-адрес та експортувати файли у різних форматах."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформна незалежність"
  description: "GroupDocs.Assembly for Node.js via Java безперешкодно інтегрується з провідними операційними системами, фреймворками та менеджерами пакетів."
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
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Assembly for Node.js via Java підтримує широкий спектр [форматів документів](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Формати Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Зображення та інші формати
        * **Переносні:** PDF
        * **Зображення:** SVG, TIFF
        * **Інші офісні формати:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Інші формати
        * **Веб:** HTML, MHTML
        * **Електронні листи:** EML, MSG, EMLX
        * **Інше:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Основні функції GroupDocs.Assembly"
  description: "Створюйте динамічні документи та звіти з потужними інструментами управління даними."

  items:
    # feature loop
    - icon: "preview"
      title: "Багаті візуалізації даних"
      content: "Легко вставляйте графіки, таблиці, зображення та списки у свої документи з повною настройкою."

    # feature loop
    - icon: "manipulate"
      title: "Перетворення ваших даних"
      content: "Використовуйте інструменти, такі як формули та сортування, для ефективної структурування та відображення інформації."

    # feature loop
    - icon: "two_pages"
      title: "Широка сумісність форматів"
      content: "Працюйте бездоганно з популярними форматами файлів для шаблонів та виходу."

    # feature loop
    - icon: "document_settings"
      title: "Розширене налаштування шаблонів"
      content: "Форматуйте шаблони з числовими, алфавітними та іншими параметрами стилізації."

    # feature loop
    - icon: "text"
      title: "Динамічна генерація штрих-кодів"
      content: "Створюйте та вбудовуйте зображення штрих-кодів безпосередньо у свої документи на вимогу."

    # feature loop
    - icon: "add"
      title: "Гнучке стилізування тексту"
      content: "Легко застосовуйте текстові стилі, такі як застосування великих літер або заголовний регістр у ваших шаблонах."

    # feature loop
    - icon: "manipulate"
      title: "Динамічне вставлення контенту"
      content: "Включайте контент з зовнішніх файлів динамічно під час генерації документів."

    # feature loop
    - icon: "convert"
      title: "Експорт у різні формати"
      content: "Зберігайте документи у кількох форматах з вашими вказаними конфігураціями."

    # feature loop
    - icon: "update"
      title: "Динамічне вбудовування медіа"
      content: "Вставляйте зображення або інші елементи за допомогою даних Base64 під час створення документів."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Приклади коду"
  description: "Відкрийте практичні приклади використання GroupDocs.Assembly для поширених задач."
  items:
    # code sample loop
    - title: "Додати маркований список у документи Word"
      content: |
        Дізнайтеся, як створити [марковані списки](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) у документах Word для ефективної організації даних. Цей приклад демонструє, як згенерувати маркований список за допомогою GroupDocs.Assembly.
        {{< landing/code title="Додати маркований список у документи Word">}}
        ```javascript {style=abap}
        // Вставте цей шаблон на сторінку документа:
        // Показники продуктивності менеджерів
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Вкажіть шлях до шаблону
        const template = "Bulleted List Template.docx";

        // Встановіть шлях до вихідного файлу
        const result = "Result Report.docx"

        // Отримайте дані менеджерів з джерела JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Генеруйте звіт з заповненими даними
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Вставити кругові графіки у PowerPoint"
      content: |
        Дізнайтеся, як використати шаблони та XML для додавання [кругових графіків](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) до ваших презентацій. Покращте свої звіти з круговими графіками для візуального та чіткого представлення даних.
        {{< landing/code title="Вставити кругові графіки у PowerPoint">}}
        ```javascript {style=abap} 
        // Додайте шаблон заголовка діаграми до презентації:
        // Дохід клієнтів <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Також включіть шаблон даних діаграми:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Вкажіть шлях до шаблону діаграми
        const template = "Pie Chart Template.pptx";

        // Встановіть шлях до вихідного файлу
        const result = "Result Report.pptx"

        // Отримайте дані клієнтів з джерела XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Згенеруйте діаграму та збережіть результат
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---