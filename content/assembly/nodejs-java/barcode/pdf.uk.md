



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: uk
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Додавання штрих-кодів до файлів PDF за допомогою JavaScript"
head_description: "Генеруйте та вбудовуйте штрих-коди у ваші документи та електронні листи з API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Створення штрих-кодів для файлів PDF за допомогою Node.js" 
description: "За допомогою GroupDocs.Assembly for Node.js via Java ви можете динамічно генерувати, налаштовувати та вбудовувати штрих-коди у документи PDF."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Почати"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Вступ до GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) дозволяє створювати професійні документи, поєднуючи дані з кількох джерел. Додавайте графіки, таблиці, списки, зображення та штрих-коди до ваших файлів. Використовуйте шаблони для впорядкування вмісту у відповідні місця. Підтримує більше 50 форматів, включаючи PDF, документи Office та електронні листи.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для додавання штрих-коду у файли PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) дозволяє вбудовувати штрих-коди в документи PDF. Він підтримує понад 60 типів штрих-кодів, включаючи 1D та 2D формати.
      
      1. Створіть шаблон зі заповнювачами для штрих-кодів (шаблони PDF не підтримуються).
      2. Отримайте дані з сумісного джерела.
      3. Встановіть параметри штрих-коду, такі як розмір та роздільна здатність.
      4. Експортуйте документ зі штрих-кодом у файл PDF.
   
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
        // Використовуйте цей тег у шаблоні, щоб включити штрих-код у вихідний документ
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Вкажіть шлях до файлу шаблону
        // Примітка: Шаблони PDF наразі не підтримуються.
        const template = "barcode_template.docx";

        // Завантажте необхідні дані з вашого джерела
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Експортуйте документ зі штрих-кодом у файл PDF.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Генеруйте документи з шаблонами, заснованими на даних"
  description: "За допомогою GroupDocs.Assembly for Node.js via Java ви можете створювати професійні файли в популярних форматах, безперешкодно вбудовуючи графіки, таблиці, списки, посилання, зображення та штрих-коди."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Основні функції GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Створення звітів з бізнес-даних"
      content: "Використовуйте API для швидкого та точного заповнення шаблонів даними з форматів, таких як JSON, XML та CSV."

    # feature loop
    - title: "Додавання візуальних елементів"
      content: "GroupDocs.Assembly підтримує вставлення елементів, таких як графіки, таблиці, списки, текст, посилання, зображення та штрих-коди в реальному часі."

    # feature loop
    - title: "Контроль розташування даних"
      content: "З шаблонами на основі LINQ ви можете точно розміщувати дані, проходити через масиви та застосовувати користувацьке форматування програмно."

    # feature loop
    - title: "Сумісність з багатьма форматами"
      content: "Працюйте з файлами, такими як документи MS Office, PDF, HTML, файли OpenOffice та електронні листи. Об'єднуйте кілька документів за потреби."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Приклад: Генерація штрих-коду програмно"
      content: |
        Цей приклад демонструє, як програмно згенерувати та вставити штрих-код у документ PDF.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Створіть шаблон із заповнювачем для штрих-коду
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Вкажіть шлях до файлу шаблону
          // Примітка: Шаблони PDF наразі не підтримуються.
          const template = "barcode_template.docx";

          // Отримайте дані з вашого джерела
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Створіть об'єкт джерела даних з необхідними деталями
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Ініціалізуйте екземпляр DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Налаштуйте конфігурацію штрих-коду
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Збережіть документ із включеним штрих-кодом
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "Досліджуйте ключові функції"
    exclude: "barcode"
    description: "Спростіть обробку документів з допомогою розширених інструментів та можливостей автоматизації."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Підтримувані формати файлів для створення звітів"
    exclude: "PDF"
    description: "Node.js via Java обробляє понад 50 типів файлів, спрощуючи злиття даних та обробку шаблонів для отримання якісних результатів."
    items: 
          
        # format loop 1
        - name: "Додати штрих-код до PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Додати штрих-код до DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Додати штрих-код до PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Додати штрих-код до XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---