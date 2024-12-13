



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: uk
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Генеруйте списки в документах DOCX за допомогою C#"
head_description: "API GroupDocs.Assembly for .NET дозволяє розробникам динамічно створювати та вбудовувати заповнені даними списки у документи та шаблони."

############################# Header ############################
title: "Додавайте списки на основі даних до документів DOCX за допомогою нашого API .NET" 
description: "GroupDocs.Assembly for .NET пропонує потужні інструменти для динамічного генерування та вбудовування списків у документи DOCX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачати безкоштовну пробну версію"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Огляд GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) призначений для оптимізації створення документів та звітів через безперешкодну інтеграцію даних з різних джерел. Заповнюйте шаблони списками, діаграмами, таблицями, штрих-кодами або текстом, і точно розміщуйте контент за допомогою розширеного набору розмітки. З підтримкою понад 50 форматів, включаючи PDF, файли MS Office та електронні листи, це ідеальне рішення для автоматизації документних робочих процесів.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для додавання заповненого даними списку до документа DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) спрощує вставлення списків на основі даних у шаблони DOCX. Створюйте та налаштовуйте списки без зайвих зусиль.
      
      1. Підготуйте шаблон DOCX з заповнювальниками для списку.
      2. Встановіть шлях до шаблону.
      3. Отримайте дані з підтримуваних джерел, таких як JSON або XML.
      4. Збережіть остаточний документ із вбудованим списком.
   
    code:
      platform: "net"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Приклад документа"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "натисніть, щоб скопіювати"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Додайте цей тег до вашого шаблону, щоб позначити місце, де з'явиться список
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Вкажіть шлях до файл-шаблона
        string template = "list_template.docx";

        // Отримайте дані з обраного джерела
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Збережіть документ з згенерованим списком
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Створюйте документи, заповнюючи шаблони структурованими даними"
  description: "GroupDocs.Assembly for .NET спрощує створення документів на основі даних. Додавайте списки, таблиці, штрих-коди, діаграми, зображення та інші елементи динамічно за допомогою розширених шаблонів."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Особливості GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генеруйте звіти на основі бізнес-даних"
      content: "API заповнює документи в популярних форматах, використовуючи дані з джерел, таких як JSON, XML, CSV тощо, з точністю та ефективністю."

    # feature loop
    - title: "Використовуйте списки та інші елементи для представлення даних"
      content: "GroupDocs.Assembly дозволяє вбудовувати списки, таблиці та діаграми разом з текстом, штрих-кодами, гіперпосиланнями та зображеннями для створення добре структурованих документів."

    # feature loop
    - title: "Вставляйте дані точно у потрібних місцях"
      content: "Використовуйте синтаксис на основі LINQ для точного позиціонування списків та інших елементів даних. Використовуйте цикли для динамічного заповнення списків і застосовуйте індивідуальне форматування програмно."

    # feature loop
    - title: "Підтримує багаторазові формати документів"
      content: "Генеруйте та керуйте документами у різних форматах, таких як MS Office, OpenOffice, PDF, HTML та електронні листи. Легко інтегруйте кілька документів в один."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як динамічно генерувати список"
      content: |
        Цей приклад демонструє, як вбудувати динамічно згенерований список у документ DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Додайте тег заповнювача до вашого шаблону для списку
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Вкажіть шлях до файл-шаблона
          string template = "numlist_template.docx";

          // Отримайте дані для заповнення списку
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Створіть об'єкт джерела даних з необхідною інформацією
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Ініціалізуйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Збережіть остаточний документ із згенерованим списком
          asm.AssembleDocument(template, "result.docx", data);
          ```
        platform: "net"
        copy_title: "Копіювати"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "натисніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.docx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Досліджуйте можливості GroupDocs.Assembly безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити з Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Дізнатися про ліцензування"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Досліджуйте основні можливості"
    exclude: "list"
    description: "Наша платформа створена для спрощення створення та інтеграції контенту документів на основі даних."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Створюйте структуровані документи в популярних форматах"
    exclude: "DOCX"
    description: ".NET підтримує понад 50 форматів, що дозволяє безперешкодно об'єднувати дані та шаблони для отримання відполірованих і структурованих результатів."
    items: 
          
        # format loop 1
        - name: "Створити список у PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Створити список у DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Створити список у PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Створити список у XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---