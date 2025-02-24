



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: uk
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Вставка діаграм у файли XLSX за допомогою JavaScript"
head_description: "З допомогою GroupDocs.Assembly for Node.js via Java розробники можуть швидко створювати та вбудовувати динамічні діаграми у документи, використовуючи живі джерела даних."

############################# Header ############################
title: "Додавайте діаграми до файлів XLSX за допомогою Node.js" 
description: "GroupDocs.Assembly for Node.js via Java спрощує процес інтеграції діаграм у документи XLSX з введенням даних у реальному часі."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Почати безкоштовно сьогодні"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Огляд GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) – це потужне рішення для створення автоматизованих документів і звітів. Додавайте діаграми, таблиці, зображення, штрих-коди та списки до файлів з точністю та безпосередністю. Ця універсальна платформа підтримує понад 50 форматів, включаючи PDF, документи Office та електронні листи.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для додавання діаграми до документа XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) дозволяє додавати діаграми до файлів XLSX. Виберіть з типів діаграм, таких як стовпчикові, лінійні або кругові.
      
      1. Розробіть шаблон XLSX з заповнювачами для діаграм.
      2. Завантажте дані з підтримуваного джерела.
      3. Налаштуйте параметри діаграми, включаючи тип, кольори та ярлики.
      4. Експортуйте документ з вбудованою діаграмою.
   
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
        // Додайте цей тег до свого шаблону для генерації діаграми.
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Вкажіть шлях до файлу шаблону.
        const template = "chart_template.xlsx";

        // Отримайте дані з вашої системи-джерела.
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Збережіть остаточний документ із вбудованою діагрою.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Без зусиль вбудовуйте діаграми у свої документи"
  description: "GroupDocs.Assembly for Node.js via Java дозволяє просто генерувати документи з багатим функціоналом у популярних файлових типах. Використовуйте шаблони для додавання діаграм, таблиць, штрих-кодів, списків, зображень та багато іншого з оновленням даних у реальному часі."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Основні функції GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Перетворюйте дані на професійні діаграми"
      content: "Перетворюйте дані з джерел, таких як JSON, XML або CSV, у високоякісні діаграми, які можна безпосередньо вбудовувати в документи."

    # feature loop
    - title: "Створюйте вражаючі візуалізації"
      content: "Генеруйте стовпчикові, кругові та лінійні діаграми, які бездоганно працюють з іншими елементами документа, такими як зображення, таблиці та штрих-коди."

    # feature loop
    - title: "Гнучке оформлення і розміщення діаграм"
      content: "Використовуйте шаблони LINQ для контролю за позиціонуванням і стилем діаграм, включаючи кольори, макети та ярлики, для естетичного представлення."

    # feature loop
    - title: "Підтримка багатьох файлових форматів"
      content: "Генеруйте документи у форматах, таких як MS Office, PDF, OpenOffice та HTML, з діаграмами, які ідеально інтегровані для професійного вигляду."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Динамічно створюйте та вставляйте діаграми"
      content: |
        Цей приклад ілюструє, як програмно створювати та вбудовувати діаграми у файли XLSX.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Налаштуйте шаблон з заповнювачем для діаграми.
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Визначте шлях до файлу шаблону.
          const template = "table_template.xlsx";

          // Отримайте дані з вибраного джерела.
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Підготуйте об'єкт даних, що містить інформацію про діаграму.
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Виберіть тип діаграми та налаштуйте її зовнішній вигляд.
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Ініціалізуйте DocumentAssembler.
          const asm = new assemblyLib.DocumentAssembler();

          // Збережіть оновлений документ із вбудованою діаграмою.
          asm.assembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Відкрийте для себе розширені функції"
    exclude: "chart"
    description: "Ця платформа спростила створення документів із інструментами, розробленими для візуалізації даних та безперебійної інтеграції."
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
    title: "Генерація звітів у кількох файлових форматах"
    exclude: "XLSX"
    description: "Node.js via Java підтримує понад 50 форматів, що дозволяє зручно поєднувати шаблони з даними для створення вишуканих документів."
    items: 
          
        # format loop 1
        - name: "Діаграми у PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Діаграми у DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Діаграми у PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Діаграми у XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---