



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: uk
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Вставити один документ в інший у DOCX за допомогою API C#"
head_description: "Зливайте документи DOCX за допомогою C#. З GroupDocs.Assembly комбінуйте файли без зусиль у всього кілька кроків."

############################# Header ############################
title: "Об'єднати документи у форматі DOCX" 
description: "З GroupDocs.Assembly for .NET ви можете швидко вставити один документ DOCX в інший. Цей API пропонує потужні інструменти для точного злиття документів."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) — це потужний інструмент для складання та маніпуляції документами. Він дозволяє користувачам вставляти один документ в інший, забезпечуючи безшовне злиття контенту. Підтримуючи понад 50 форматів, включаючи PDF, файли MS Office та інші, ви можете організовувати, редагувати та налаштовувати фінальний результат відповідно до ваших вимог.

############################# Steps ############################
steps:
    enable: true
    title: "Як з'єднати документ з файлом DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) дозволяє легко вставити один документ в інший файл DOCX. Об’єднуйте та налаштовуйте зміст з комфортом.
      
      1. Створіть шаблон DOCX з заповнювачами для вбудованого документа.
      2. Визначте шлях до файлу шаблону.
      3. Вкажіть шлях до документа, який слід вставити.
      4. Збережіть фінальний файл з вбудованим контентом.
   
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
        // Додайте цей тег до вашого шаблону, щоб позначити точку вставки
        // <<doc [doc_expression]>>

        // Вкажіть шлях файлу для шаблону
        string template = "doc_template.docx";

        // Надайте шлях до документа, який потрібно вставити
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Зберігайте злитий документ
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Упростіть злиття документів з допомогою розширених інструментів"
  description: "Бібліотека GroupDocs.Assembly for .NET спрощує вставку одного документа в інший, підтримує різні формати файлів та пропонує можливості налаштування для бездоганної інтеграції."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Генерація звітів з ваших бізнес-даних"
      content: "Автоматично заповнюйте документи даними з JSON, XML, CSV або інших джерел, забезпечуючи точність та ефективність процесів."

    # feature loop
    - title: "Додавання візуальних елементів до документів"
      content: "GroupDocs.Assembly дозволяє включати таблиці, графіки та списки, а також текст, посилання, зображення та динамічно згенеровані штрих-коди."

    # feature loop
    - title: "Точна позиція та форматування даних"
      content: "Шаблони на основі LINQ дають вам контроль над розміщенням даних, дозволяють опрацьовувати цикли для масивів і дозволяють стилізацію, наприклад, налаштування кольору."

    # feature loop
    - title: "Підтримка декількох форматів файлів"
      content: "Легко вставляйте документи один в один на різних форматах, таких як MS Office, PDF, HTML, OpenOffice та інші."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як програмно вставити зображення в документ"
      content: |
        Цей приклад демонструє, як вставити зображення в документ DOCX за допомогою GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Додайте тег заповнювача у вашому шаблоні
          // <<image [expression]>>

          // Вкажіть шлях файлу для шаблону
          string template = "template.docx";

          // Встановіть шлях до файлу зображення
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Ініціалізуйте екземпляр DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Збережіть документ з вбудованим зображенням
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "Відкрийте потужні інструменти"
    exclude: "document"
    description: "Вивчіть можливості, які пропонує GroupDocs.Assembly для вставки та злиття документів з точністю."
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
    title: "Зливайте документи в різних форматах"
    exclude: "DOCX"
    description: "За допомогою API .NET ви можете з'єднувати документи в більш ніж 50 підтримуваних форматах. Без зусиль вставляйте файли або їх частини у ваші фінальні документи."
    items: 
          
        # format loop 1
        - name: "Вставити документ у PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Вставити документ у DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Вставити документ у PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Вставити документ у XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---