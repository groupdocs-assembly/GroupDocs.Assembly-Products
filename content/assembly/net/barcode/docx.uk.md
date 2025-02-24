



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: uk
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Генеруйте штрих-коди в документах DOCX за допомогою C#"
head_description: "API GroupDocs.Assembly for .NET дозволяє розробникам динамічно генерувати та вбудовувати зображення штрих-кодів у документи та електронні листи."

############################# Header ############################
title: "Додайте штрих-коди до документів DOCX за допомогою нашого API .NET" 
description: "GroupDocs.Assembly for .NET надає повну підтримку для динамічного створення та вбудовування штрих-кодів у документи DOCX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачати безкоштовну версію"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Огляд GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) створено для допомоги у генерації документів та звітів шляхом інтеграції даних з різних джерел. Наповнюйте документи текстом або числовими даними, створюйте графіки, таблиці, списки або вставляйте зображення та штрих-коди на льот. Використовуйте розширений розмітку для точного розміщення даних. Підтримує більш ніж 50 форматів, включаючи PDF, файли MS Office та електронні листи.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для додавання згенерованого штрих-коду до документа DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) дозволяє вставляти штрих-коди в шаблони у форматах, таких як DOCX. Підтримує понад 60 типів штрих-кодів, включаючи одновимірні та двовимірні формати.
      
      1. Підготуйте шаблон DOCX з місцями для штрих-кодів.
      2. Отримайте дані з будь-якого підтримуваного джерела даних.
      3. Налаштуйте додаткові параметри, такі як розмір або роздільна здатність штрих-коду.
      4. Збережіть шаблон зі штрих-кодом як новий документ.
   
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
        // Вставте цей тег у свій шаблон для генерації штрих-коду в фінальному документі
        // <<barcode [barcode_expression] -barcode_type>>

        // Вкажіть шлях до файлу шаблону
        string template = "barcode_template.docx";

        // Отримайте дані з вашого джерела
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Збережіть документ з згенерованим штрих-кодом
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Генерація документів шляхом заповнення шаблонів даними"
  description: "GroupDocs.Assembly for .NET розроблений для спрощення створення документів у популярних форматах. Додавайте графіки, списки, таблиці, гіперпосилання, зображення та штрих-коди, використовуючи розширені шаблони та розмітку."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Особливості GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Створення звітів з бізнес-даних"
      content: "Наш API ефективно заповнює документи в популярних офісних форматах, використовуючи дані з таких джерел, як JSON, XML та CSV."

    # feature loop
    - title: "Використовуйте візуальні елементи для відображення даних"
      content: "GroupDocs.Assembly підтримує вбудовування нативних елементів, таких як списки, таблиці та графіки, а також текст, гіперпосилання, зображення та динамічно генеровані штрих-коди."

    # feature loop
    - title: "Вставляйте дані будь-де в документі"
      content: "Використовуйте синтаксис на базі LINQ для точного розташування даних. Масиви можна вставляти за допомогою циклів для-each, а форматування (наприклад, колір) можна налаштувати програмно."

    # feature loop
    - title: "Підтримує широкий спектр форматів"
      content: "Обробляйте популярні формати файлів, такі як MS Office, OpenOffice, PDF, HTML та різні формати електронної пошти. Вбудовуйте один документ в інший за потреби."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як динамічно генерувати штрих-код"
      content: |
        Цей приклад демонструє вбудовування динамічно згенерованого штрих-коду в документ DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Використовуйте цей шаблон для вставки штрих-коду в документ
          // <<barcode [barcode_expression] -barcode_type>>

          // Вкажіть шлях до файлу шаблону
          string template = "barcode_template.docx";

          // Отримайте дані з вибраного джерела
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Створіть об'єкт джерела даних лише з потрібними даними
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Ініціалізуйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Встановіть додаткові властивості штрих-коду
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // Збережіть фінальний документ з вбудованим штрих-кодом
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    title: "Ознайомтесь з ключовими функціями"
    exclude: "barcode"
    description: "Наше рішення розроблене для оптимізації ваших потреб у обробці бізнес-документів."
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
    title: "Створення звітів в популярних форматах"
    exclude: "DOCX"
    description: ".NET підтримує генерацію звітів у більш ніж 50 форматах, що дозволяє безперешкодно об'єднувати дані та шаблони для видатних результатів."
    items: 
          
        # format loop 1
        - name: "Додати штрих-код до PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Додати штрих-код до DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Додати штрих-код до PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Додати штрих-код до XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---