---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: uk
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
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "API .NET для автоматизації документів, складання та генерування звітів"
head_description: "C# .NET API для автоматизації документів, складання та генерування звітів. Створюйте PDF, Word, Excel, PPTX, HTML і електронні документи з настраюваних шаблонів."

############################# Header ############################
title: "API автоматизації документів та звітності .NET"
description: "Генеруйте звіти в додатках .NET, визначаючи шаблони та об'єднуючи дані."
words:
  for: "для"

actions:
  main: "Завантажити пробну версію через Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Assembly безкоштовно або запитайте ліцензію."

release:
  title: "Версія {0} випущена"
  notes: "Дивіться, що нового"
  downloads: "Завантаження"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Заповнити діаграму у DOCX за допомогою C#"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Шлях до основного шаблону
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Assembly"
  description: ".NET рішення для автоматизації створення документів з просунутим інтеграцією даних."
  features:
    # feature loop
    - title: "Додайте бізнес-дані до шаблонів документів за допомогою C#"
      content: "Генерація звітів спрощена: За допомогою GroupDocs.Assembly for .NET ви можете без зусиль вставляти дані з таких джерел, як JSON або XML, у заздалегідь визначені шаблони."

    # feature loop
    - title: "Обробляйте вбудовані об'єкти даних"
      content: "Підтримувані типи документів включають вбудовані об'єкти, такі як діаграми, таблиці та списки, які можуть автоматично заповнюватися даними."

    # feature loop
    - title: "Додаткові можливості"
      content: "GroupDocs.Assembly for .NET надає широкі можливості налаштування. Програмно проектуйте об'єкти даних, генеруйте штрих-коди, використовуйте онлайн-джерела даних через URL-адреси та зберігайте вихід у різних форматах."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформна незалежність"
  description: "GroupDocs.Assembly for .NET сумісний з наступними операційними системами, фреймворками та менеджерами пакетів."
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
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Assembly for .NET може обробляти наступні [формати файлів](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "Особливості GroupDocs.Assembly"
  description: "Створюйте документи та звіти, використовуючи розширені моделі даних."

  items:
    # feature loop
    - icon: "preview"
      title: "Розширене представлення даних"
      content: "Підтримує широкий спектр об'єктів даних, таких як діаграми, списки, таблиці, зображення та багато іншого."

    # feature loop
    - icon: "manipulate"
      title: "Маніпуляція даними"
      content: "Застосовуйте формули та послідовні операції для ефективного форматування та відображення даних."

    # feature loop
    - icon: "two_pages"
      title: "Широкий спектр підтримуваних форматів"
      content: "Безперешкодно працюйте з усіма звичайними форматами документів для шаблонів або вихідних файлів."

    # feature loop
    - icon: "document_settings"
      title: "Багатий шаблонний розмітка"
      content: "Використовуйте порядкове, кардинальне та алфавітне числове форматування в шаблонах."

    # feature loop
    - icon: "text"
      title: "Вбудовування штрих-кодів"
      content: "Динамічно генеруйте зображення штрих-кодів та вставляйте їх у документи."

    # feature loop
    - icon: "add"
      title: "Форматування даних"
      content: "Форматуйте рядки в шаблонах у верхньому, нижньому, з великої букви або стилях з великою першою літерою."

    # feature loop
    - icon: "manipulate"
      title: "Маніпуляція вмістом документа"
      content: "Динамічно вставляйте вміст з зовнішніх документів у ваші звіти."

    # feature loop
    - icon: "convert"
      title: "Збереження у кількох форматах"
      content: "Вкажіть формат виходу, використовуючи розширення файлів або детальні конфігурації."

    # feature loop
    - icon: "update"
      title: "Гнучка обробка даних"
      content: "Динамічно вставляйте зображення та документи, використовуючи байти, закодовані в Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Приклади коду"
  description: "Приклади коду для типових операцій GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Маркірований список у документі Microsoft Word"
      content: |
        [Маркіровані списки](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) є звичайним способом представлення бізнес-даних. Ось приклад додавання списку до документа Word за допомогою GroupDocs.Assembly.
        {{< landing/code title="Як заповнити список у документах">}}
        ```csharp {style=abap}
        // Вставте цей шаблон на сторінку документа:
        // Показники продуктивності менеджерів
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Вкажіть шлях до шаблону
        string template = "Bulleted List Template.docx";

        // Встановіть шлях до вихідного файлу
        string result = "Result Report.docx"

        // Отримайте дані менеджерів з джерела JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Генеруйте звіт з заповненими даними
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Кругові діаграми в презентаціях PPTX"
      content: |
        Ви можете створити [кругові діаграми](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) за допомогою шаблонів та XML-даних. Покращте ваші звіти візуально привабливими представленнями даних.
        {{< landing/code title="Як відобразити дані в круговій діаграмі">}}
        ```csharp {style=abap}
        // Додайте шаблон заголовка діаграми до презентації:
        // Дохід клієнтів <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Також включіть шаблон даних діаграми:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Вкажіть шлях до шаблону діаграми
        string template = "Pie Chart Template.pptx";

        // Встановіть шлях до вихідного файлу
        string result = "Result Report.pptx"

        // Отримайте дані клієнтів з джерела XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Згенеруйте діаграму та збережіть результат
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---