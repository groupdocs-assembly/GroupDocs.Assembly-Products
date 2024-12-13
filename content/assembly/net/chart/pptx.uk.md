



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: uk
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Створення діаграм у файлах PPTX з C#"
head_description: "API GroupDocs.Assembly for .NET дозволяє розробникам динамічно генерувати та вставляти діаграми або графіки в документи, використовуючи дані в реальному часі."

############################# Header ############################
title: "Вбудовування діаграм у файли PPTX за допомогою API .NET" 
description: "GroupDocs.Assembly for .NET надає потужний спосіб заповнення файлів PPTX динамічними даними та бездоганної інтеграції діаграм."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Спробуйте безкоштовно"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) — це інструмент, розроблений для спрощення створення документів і звітів, що інтегрує дані з різних джерел. Генеруйте діаграми, таблиці, списки, штрих-коди та зображення динамічно. Розширені параметри форматування дозволяють точно розміщувати та налаштовувати ваш контент. Підтримує понад 50 форматів файлів, включаючи PDF, документи MS Office та електронні листи.

############################# Steps ############################
steps:
    enable: true
    title: "Як додати діаграму до документа PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) спрощує генерування та вбудовування діаграм у ваші шаблони PPTX. Підтримує різноманітні типи діаграм, такі як стовпчикові, кругові та лінійні.
      
      1. Створіть шаблон PPTX з запланованими місцями для діаграм.
      2. Отримайте свої дані з сумісного джерела.
      3. Визначте параметри діаграми, такі як тип, мітки та кольорова схема.
      4. Збережіть оновлений файл із вбудованою діаграмою.
   
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
        // Додайте цей тег до свого шаблону, щоб згенерувати діаграму
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Вкажіть шлях до файлу шаблону
        string template = "chart_template.pptx";

        // Завантажте дані з обраного джерела
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Збережіть документ із вбудованою діаграмою
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Додавайте динамічні діаграми до своїх документів без зусиль"
  description: "GroupDocs.Assembly for .NET спрощує створення документів, керованих даними, у широко використовуваних форматах. Використовуйте шаблони для вставки діаграм, таблиць, штрих-кодів, списків, гіперпосилань та зображень з розширеною інтеграцією даних."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Ключові можливості GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Перетворюйте дані на професійні діаграми"
      content: "Перетворюйте дані з JSON, XML, CSV та інших джерел на візуально привабливі діаграми всього за кілька кроків, використовуючи наш API."

    # feature loop
    - title: "Створюйте візуально привабливий контент"
      content: "GroupDocs.Assembly підтримує кілька типів діаграм, таких як графіки стовпців, кругові діаграми та лінійні графіки. Поєднуйте їх з таблицями, штрих-кодами, зображеннями та іншими елементами для створення професійних звітів."

    # feature loop
    - title: "Точно розміщуйте та налаштовуйте діаграми"
      content: "З синтаксисом LINQ ви можете динамічно генерувати та розміщувати діаграми точно там, де необхідно. Легко налаштовуйте стилі, кольори та макети відповідно до ваших вимог."

    # feature loop
    - title: "Працює з різними форматами файлів"
      content: "Створюйте документи в популярних форматах, таких як MS Office, PDF, OpenOffice та HTML. Встроюйте діаграми без зусиль у будь-який підтримуваний формат з повною сумісністю."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Створення діаграми програмно"
      content: |
        Цей приклад демонструє, як динамічно створити та вбудувати діаграму в документ PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Підготуйте шаблон із запланованим місцем для діаграми
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Надайте шлях до файлу шаблону
          string template = "table_template.pptx";

          // Отримайте дані з вашого джерела
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Сформуйте об'єкт даних з необхідною інформацією
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Встановіть властивості діаграми, такі як тип та зовнішній вигляд
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Ініціалізуйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Експортуйте документ з вбудованою діаграмою
          asm.AssembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "Відкрийте для себе ключові можливості"
    exclude: "chart"
    description: "Наша платформа допоможе вам створити привабливі, керовані даними документи, адаптовані до ваших потреб."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Створюйте візуально багаті звіти в кількох форматах"
    exclude: "PPTX"
    description: ".NET дозволяє генерувати документи з інтегрованими діаграмами в понад 50 підтримуваних форматах, поєднуючи шаблони з вашими даними без труднощів."
    items: 
          
        # format loop 1
        - name: "Діаграми у PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Діаграми у DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Діаграми у PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Діаграми у XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---