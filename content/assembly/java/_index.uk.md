---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: uk
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

############################# Head ############################
head_title: "Java бібліотека для створення документів, автоматизації та звітності"
head_description: "Java бібліотека для автоматизації створення документів та генерування звітів. Створюйте PDF, Word, Excel, PPTX, HTML та електронні документи за допомогою настраюваних шаблонів."

############################# Header ############################
title: "Java API для автоматизації звітів і документів"
description: "Спростіть генерацію звітів у Java, об'днуючи дані з шаблонами."
words:
  for: "для"

actions:
  main: "Отримати пробну версію через NuGet"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Assembly безкоштовно або запитайте ліцензію."

release:
  title: "Версія {0} випущена"
  notes: "Дивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Генерувати діаграму у DOCX за допомогою Java"
  more: "Більше прикладів"
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
    // Шлях до основного шаблону
    String template = "chart_template.docx";

    // Отримайте дані продуктивності менеджерів з джерела
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Створіть екземпляр DataSourceInfo з даними
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Встановіть кольори діаграми, використовуючи інший DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Заповніть шаблон даними та збережіть його вихідним
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Assembly"
  description: "Java бібліотека, розроблена для автоматизованого створення документів і безшовної інтеграції даних."
  features:
    # feature loop
    - title: "Об'єднуйте бізнес-дані в шаблони за допомогою Java"
      content: "Легко створюйте професійні звіти, вбудовуючи дані з JSON, XML або інших джерел у заздалегідь розроблені шаблони за допомогою GroupDocs.Assembly for Java."

    # feature loop
    - title: "Працюйте з вбудованими об'єктами"
      content: "Автоматично заповнюйте елементи, такі як таблиці, діаграми та схеми в документах, використовуючи дані з зовнішніх джерел."

    # feature loop
    - title: "Розширене налаштування"
      content: "GroupDocs.Assembly for Java пропонує гнучкі функції, такі як генерація штрих-кодів, витягування онлайн-даних через URL-адреси та експорт виходу в різних форматах."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформна незалежність"
  description: "GroupDocs.Assembly for Java безперешкодно працює з популярними операційними системами, фреймворками розробки та менеджерами пакетів."
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
    GroupDocs.Assembly for Java підтримує широкий спектр [форматів документів](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Ключові можливості GroupDocs.Assembly"
  description: "Створюйте професійні документи та звіти з розширеними можливостями обробки даних."

  items:
    # feature loop
    - icon: "preview"
      title: "Візуальні елементи даних"
      content: "Додавайте та форматуйте елементи, такі як діаграми, таблиці, зображення та списки безпосередньо у ваших документах."

    # feature loop
    - icon: "manipulate"
      title: "Трансформація даних"
      content: "Використовуйте формули, сортування та інші інструменти для організації та ефективного представлення ваших даних."

    # feature loop
    - icon: "two_pages"
      title: "Підтримка кількох форматів"
      content: "Легко працюйте з загальними типами файлів як для шаблонів, так і для вихідних файлів."

    # feature loop
    - icon: "document_settings"
      title: "Покращене форматування шаблонів"
      content: "Налаштуйте шаблони з числовими, алфавітними та іншими розширеними опціями форматування."

    # feature loop
    - icon: "text"
      title: "Динамічна генерація штрих-кодів"
      content: "Швидко створюйте та вставляйте зображення штрих-кодів у документи за потреби."

    # feature loop
    - icon: "add"
      title: "Гнучке стилювання тексту"
      content: "Застосовуйте трансформації тексту, такі як прописні, малописні, заголовні стилі або інші стилі в шаблонах."

    # feature loop
    - icon: "manipulate"
      title: "Імпорт зовнішнього вмісту"
      content: "Динамічно вбудовуйте вміст з зовнішніх файлів під час створення документів."

    # feature loop
    - icon: "convert"
      title: "Експорт у кількох форматах"
      content: "Зберігайте остаточні документи у різних форматах файлів, використовуючи вказані розширення або конфігурації."

    # feature loop
    - icon: "update"
      title: "Динамічне вбудовування мультимедіа"
      content: "Вставляйте зображення або інший вміст, використовуючи дані, закодовані в Base64, під час створення документів."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Приклади коду"
  description: "Досліджуйте зразки коду для загальних завдань з GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Створення маркірованого списку у Word"
      content: |
        Дізнайтеся, як додати [маркіровані списки](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) до документів Word для організованого представлення даних. Цей приклад демонструє, як згенерувати список у Word за допомогою GroupDocs.Assembly.
        {{< landing/code title="Створення маркірованого списку у Word">}}
        ```java {style=abap}
        // Вставте цей шаблон на сторінку документа:
        // Показники продуктивності менеджерів
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Вкажіть шлях до шаблону
        String template = "Bulleted List Template.docx";

        // Встановіть шлях до вихідного файлу
        String result = "Result Report.docx"

        // Отримайте дані менеджерів з джерела JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Генеруйте звіт з заповненими даними
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Створення кругових діаграм у PPTX"
      content: |
        Використовуйте шаблони та XML, щоб додати [кругові діаграми](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) до своїх презентацій. Зробіть свої звіти більш захопливими, включивши кругові діаграми для візуалізації даних.
        {{< landing/code title="Створення кругових діаграм у PPTX">}}
        ```java {style=abap}   
        // Додайте шаблон заголовка діаграми до презентації:
        // Дохід клієнтів <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Також включіть шаблон даних діаграми:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Вкажіть шлях до шаблону діаграми
        String template = "Pie Chart Template.pptx";

        // Встановіть шлях до вихідного файлу
        String result = "Result Report.pptx"

        // Отримайте дані клієнтів з джерела XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Згенеруйте діаграму та збережіть результат
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---