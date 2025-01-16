



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: uk
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Створення динамічних списків у PPTX за допомогою JavaScript"
head_description: "Проектуйте та вставляйте списки в шаблони PPTX за допомогою API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Вставка списків на основі даних у файли PPTX за допомогою Node.js" 
description: "GroupDocs.Assembly for Node.js via Java пропонує потужні інструменти для додавання гнучких списків, підключених до даних, у документи PPTX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Почати безкоштовно"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Про GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) спрощує створення документів, витягуючи дані з різних джерел та вбудовуючи їх у шаблони. Використовуйте його для створення списків, таблиць, діаграм та інших елементів із точним розташуванням та параметрами форматування. Підтримуючи понад 50 форматів, включаючи PDF, MS Office та електронну пошту, він допомагає автоматизувати процес генерації документів.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для вставлення списку в файл PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) спрощує додавання докладних, підключених до даних списків у ваші шаблони PPTX.
      
      1. Створіть шаблон PPTX та визначте заповнювачі для списку.
      2. Вкажіть шлях до файлу шаблону.
      3. Завантажте дані з підтримуваних джерел, таких як JSON або XML.
      4. Збережіть документ з згенерованим списком.
   
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
        // Вставте цей тег у свій шаблон, щоб позначити, куди буде вставлено список
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Вкажіть шлях до файлу вашого шаблону
        const template = "list_template.pptx";

        // Отримайте дані з бажаного джерела
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Збережіть файл з вбудованим списком
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Просто генеруйте документи з інтегрованими даними"
  description: "За допомогою GroupDocs.Assembly for Node.js via Java ви можете вбудовувати списки, таблиці, діаграми та інші елементи в шаблони, заощаджуючи час і зусилля."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Особливості GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерація звітів з кількох джерел даних"
      content: "Імпортуйте дані з JSON, XML, CSV або інших форматів для ефективного заповнення списків та інших компонентів."

    # feature loop
    - title: "Додавання списків та інших візуальних елементів"
      content: "GroupDocs.Assembly дозволяє безперешкодно впроваджувати списки, таблиці, діаграми тощо поряд із текстом, зображеннями та посиланнями для досягнення вишуканих результатів."

    # feature loop
    - title: "Точне розміщення та стилізація даних"
      content: "Шаблони на основі LINQ дають змогу контролювати, де саме з'являються списки та інші дані, використовувати цикли для повторюваних елементів і налаштовувати стилі відповідно до ваших потреб."

    # feature loop
    - title: "Підходить для кількох форматів"
      content: "Створюйте документи у форматах, таких як MS Office, PDF, OpenOffice, HTML та електронна пошта. Об'єднуйте вміст з різних джерел в один файл."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Програмне створення списку в документі"
      content: |
        Цей приклад демонструє, як динамічно додати список до документа PPTX за допомогою GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Додайте заповнювач у свій шаблон для списку
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Вкажіть шлях до файлу шаблону
          const template = "numlist_template.pptx";

          // Завантажте дані для заповнення списку
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Підготуйте джерело даних з необхідними даними
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Ініціалізуйте DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Збережіть фінальний документ з включеним списком
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "Досліджуйте можливості GroupDocs.Assembly"
    exclude: "list"
    description: "Проектуйте та генеруйте документи, насичені даними, без зусиль завдяки потужним інтеграційним інструментам."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Створення документів у різних форматах"
    exclude: "PPTX"
    description: "Node.js via Java підтримує понад 50 форматів файлів, що спрощує об'єднання шаблонів і даних у професійні результати."
    items: 
          
        # format loop 1
        - name: "Створити список у PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Створити список у DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Створити список у PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Створити список у XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---