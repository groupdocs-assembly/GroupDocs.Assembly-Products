



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: uk
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Об'єднайте документи у DOCX за допомогою JavaScript"
head_description: "Об'єднуйте файли DOCX за допомогою JavaScript. GroupDocs.Assembly спрощує злиття документів всього за кілька простих кроків."

############################# Header ############################
title: "Просто об'єднуйте вміст у файли DOCX" 
description: "За допомогою GroupDocs.Assembly for Node.js via Java інтеграція одного файлу DOCX в інший є швидкою і точною. Насолоджуйтесь гнучкими, надійними інструментами для безперешкодного злиття."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Спробуйте безкоштовно"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Огляд GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) пропонує потужний спосіб управління документами. Об'єднуйте один файл в інший, підтримуючи більше 50 форматів, таких як PDF та MS Office. Налаштовуйте макети, редагуйте вміст та організовуйте документи саме так, як вам потрібно.

############################# Steps ############################
steps:
    enable: true
    title: "Як об'єднати документ у файл DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) спрощує вставлення одного файлу DOCX в інший з налаштовуваними варіантами.
      
      1. Розробіть шаблон DOCX з місцезнаками для вмісту.
      2. Встановіть шлях до шаблону.
      3. Надайте шлях до документа для об'єднання.
      4. Експортуйте фінальний файл з об'єднаним вмістом.
   
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
        // Вставте цей тег у свій шаблон, щоб визначити, де буде вставлено документ
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Встановіть шлях до основного шаблону
        const template = "doc_template.docx";

        // Надайте шлях до документа, який ви хочете об'єднати
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // Збережіть фінальний вихід із вбудованим документом
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Потужні інструменти для інтеграції документів"
  description: "GroupDocs.Assembly for Node.js via Java спрощує вставку файлів в різноманітні формати, які можна повністю налаштувати. Забезпечте послідовні, професійні результати щоразу."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Ключові можливості GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерація звітів з діловими даними"
      content: "Отримуйте дані з JSON, XML або CSV джерел для швидкого та точного створення всебічних звітів і документів."

    # feature loop
    - title: "Додавання елементів збагаченого візуального оформлення"
      content: "GroupDocs.Assembly дозволяє включати таблиці, графіки, списки, зображення та штрих-коди поряд із текстом і гіперпосиланнями."

    # feature loop
    - title: "Точне розташування даних"
      content: "Використовуйте шаблони LINQ, щоб розташувати дані точно там, де потрібно, обробляйте повторювані елементи, такі як масиви, та налаштовуйте стилі без зусиль."

    # feature loop
    - title: "Працює з різними форматами"
      content: "Об'єднуйте вміст безперешкодно в таких форматах, як PDF, файли MS Office, HTML та OpenOffice, пропонуючи гнучкість для всіх проектів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Вбудування зображення в документ програмно"
      content: |
        Цей приклад демонструє, як вставити зображення у файл DOCX за допомогою GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Додайте місцезнак у шаблон для зображення
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Вкажіть шлях до файлу шаблону
          const template = "template.docx";

          // Встановіть шлях до зображення, яке потрібно вбудувати
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Ініціалізуйте об'єкт DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Збережіть документ з включеним зображенням
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    exclude: "document"
    description: "Досліджуйте всебічні інструменти, які пропонує GroupDocs.Assembly для ефективного та безперешкодного злиття документів."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Об'єднуйте документи у багатьох форматах"
    exclude: "DOCX"
    description: "Використовуйте Node.js via Java, щоб об'єднувати вміст у більше ніж 50 файлових форматах, забезпечуючи професійні та відшліфовані результати."
    items: 
          
        # format loop 1
        - name: "Вставити документ у PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Вставити документ у DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Вставити документ у PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Вставити документ у XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---