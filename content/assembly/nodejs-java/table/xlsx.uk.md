



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: uk
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Вставка таблиць у XLSX документи з JavaScript"
head_description: "Використовуйте GroupDocs.Assembly for Node.js via Java для швидкого вбудовування таблиць у документи або електронні листи, отримуючи дані з різних джерел."

############################# Header ############################
title: "Без зусиль додавайте таблиці до XLSX файлів за допомогою Node.js" 
description: "З GroupDocs.Assembly for Node.js via Java заповнення таблиць у XLSX документах є простим, використовуючи дані з кількох джерел."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Розпочати безкоштовний пробний період"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Вступ до GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) — це потужний інструмент для автоматизації створення документів. Він дозволяє вставляти таблиці, графіки, списки та зображення в шаблони з точною розміткою вмісту. Підтримуючи понад 50 форматів файлів, включаючи PDF, Word та електронну пошту, він спрощує створення звітів та інші завдання.

############################# Steps ############################
steps:
    enable: true
    title: "Як додати дані до таблиці в XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) дозволяє вам швидко заповнювати шаблони таблиць для файлів XLSX, використовуючи динамічні джерела даних.
      
      1. Створіть шаблон XLSX з заповнювачами для рядків і стовпців таблиці.
      2. Завантажте дані з підтримуваного джерела, наприклад JSON або CSV.
      3. Організуйте та відформатуйте дані за потреби.
      4. Згенеруйте документ з готовою таблицею.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Приклад документа"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "натисніть, щоб скопіювати"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Додайте ці теги до заповнювачів рядків таблиці у вашому шаблоні
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Вкажіть шлях до шаблону
        const template = "table_template.xlsx";

        // Завантажте свої дані з обраного джерела
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Збережіть остаточний документ з заповненою таблицею
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Легке додавання таблиць на основі даних до документів"
  description: "GroupDocs.Assembly for Node.js via Java дозволяє користувачам автоматично створювати таблиці, при цьому вбудовуючи графіки, зображення та списки за допомогою шаблонізованих робочих процесів."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Основні функції GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерація таблиць з структурованих даних"
      content: "Отримуйте дані з JSON, XML, CSV та інших форматів для автоматичного заповнення таблиць документа."

    # feature loop
    - title: "Створення естетичного вмісту"
      content: "Використовуйте GroupDocs.Assembly для проектування професійних таблиць, графіків і списків, а також для додавання посилань, зображень і тексту для вдосконаленого вигляду документа."

    # feature loop
    - title: "Динамічне розміщення вмісту таблиці"
      content: "Додавайте рядки та стовпці програмно за допомогою шаблонів на основі LINQ та налаштовуйте стилі, такі як шрифти, кольори та вирівнювання."

    # feature loop
    - title: "Безперешкодно працює з різними форматами"
      content: "Легко створюйте або редагуйте таблиці в MS Office, OpenOffice, PDF, HTML та інших форматах, об'єднуючи їх у файли за потреби."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як програмно заповнити таблицю"
      content: |
        Цей приклад демонструє заповнення таблиці в документі XLSX даними з зовнішнього джерела.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Розробіть шаблон із заповнювачами для таблиці
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Вкажіть шлях до файлу шаблону
          const template = "table_template.xlsx";

          // Завантажте необхідні дані з вашого джерела
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Організуйте дані у потрібну структуру
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Ініціалізуйте DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Збережіть вихідний документ з готовою таблицею
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Копіювати"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "натисніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.xlsx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Досліджуйте можливості GroupDocs.Assembly безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити з NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Дізнатися про ліцензування"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Основні функції в одному погляді"
    exclude: "table"
    description: "Наш API автоматизує створення таблиць і покращує генерацію документів з універсальними інструментами та шаблонами."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генерація таблиць у різних форматах"
    exclude: "XLSX"
    description: "З Node.js via Java заповнюйте шаблони та створюйте всебічні таблиці у більш ніж 50 підтримуваних форматах файлів."
    items: 
          
        # format loop 1
        - name: "Додати таблицю до PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Додати таблицю до DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Додати таблицю до PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Додати таблицю до XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---