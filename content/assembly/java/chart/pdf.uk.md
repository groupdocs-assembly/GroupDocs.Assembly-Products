



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: uk
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Генеруйте діаграми у документах PDF за допомогою Java"
head_description: "API GroupDocs.Assembly for Java дозволяє розробникам створювати та вставляти динамічні діаграми або графіки у документи без труднощів, підживлюючись даними в реальному часі."

############################# Header ############################
title: "Додавайте діаграми до документів PDF з API Java" 
description: "GroupDocs.Assembly for Java спрощує процес вбудовування діаграм у документи PDF, використовуючи дані в реальному часі."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Розпочати безкоштовно"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Вступ до GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Дізнатися більше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) є універсальним рішенням для автоматизації створення документів та звітів. Він дозволяє вам додавати діаграми, таблиці, списки, штрихкоди та зображення безпосередньо у ваші файли, з просунутими інструментами для точного форматування та інтеграції даних. Платформа підтримує понад 50 форматів, включаючи PDF, файли Microsoft Office та електронні листи.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для вбудовування діаграми у документ PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) спрощує процес вставлення діаграм у шаблони PDF. Виберіть один з різних стилів діаграм, включаючи стовпчикові, кругові та лінійні діаграми.
      
      1. Створіть шаблон з місцями для діаграми (шаблони PDF наразі не підтримуються).
      2. Завантажте ваші дані з сумісного джерела.
      3. Встановіть параметри діаграми, такі як тип, мітки та кольори.
      4. Збережіть документ з діаграмою у форматі PDF.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Приклад документа"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "натисніть, щоб скопіювати"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Додайте цей тег до вашого шаблону, щоб включити діаграму.
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Вкажіть шлях до файлу вашого шаблону.
        // Шаблони PDF наразі не підтримуються.
        String template = "chart_template.docx";

        // Отримайте необхідні дані з вашого джерела.
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Збережіть фінальний документ із вбудованою діаграмою.
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Без зусиль вбудовуйте динамічні діаграми у ваші документи"
  description: "GroupDocs.Assembly for Java надає простий спосіб створення документів з багатими даними у популярних форматах. Використовуйте шаблони, щоб вставити діаграми, таблиці, штрихкоди, списки, посилання та зображення з динамічними оновленнями з ваших даних."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Перетворюйте дані на діаграми"
      content: "Використовуйте API, щоб перетворити дані з JSON, XML, CSV або інших джерел у чисті, професійні діаграми для ваших документів."

    # feature loop
    - title: "Створюйте візуально вражаючий контент"
      content: "GroupDocs.Assembly підтримує різноманітні візуальні формати, включаючи стовпчикові графіки, кругові діаграми та лінійні графіки, які можна комбінувати з таблицями, штрихкодами, зображеннями та іншим для покращених звітів."

    # feature loop
    - title: "Налаштовуване розташування та стилізація діаграм"
      content: "З синтаксисом на основі LINQ ви можете динамічно генерувати та розташовувати діаграми в документі, при цьому легко налаштовуючи стилі, кольори та макети відповідно до ваших дизайнерських потреб."

    # feature loop
    - title: "Підтримує кілька форматів документів"
      content: "Генеруйте документи у форматах MS Office, PDF, OpenOffice та HTML. Діаграми безперешкодно інтегруються у будь-який підтримуваний формат для професійних результатів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Програмно генеруйте та вбудовуйте діаграми"
      content: |
        Цей приклад демонструє, як програмно створити та вбудувати діаграму в документ PDF.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Підготуйте шаблон із місцем для діаграми.
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Вкажіть шлях до файлу шаблону.
          // Шаблони PDF наразі не підтримуються.
          String template = "table_template.docx";

          // Завантажте дані з вибраного джерела.
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Створіть об'єкт даних з відповідною інформацією.
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Налаштуйте тип та зовнішній вигляд діаграми.
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Ініціалізуйте DocumentAssembler.
          DocumentAssembler asm = new DocumentAssembler();

          // Збережіть готовий документ із вбудованою діаграмою.
          asm.assembleDocument(template, "result.pdf", data, design);
          ```
        platform: "java"
        copy_title: "Копіювати"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "натисніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.pdf"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Досліджуйте можливості GroupDocs.Assembly безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити з Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Дізнатися про ліцензування"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Досліджуйте потужні можливості"
    exclude: "chart"
    description: "Ця платформа спрощує процес проектування документів, орієнтованих на дані, з візуально привабливим оформленням, які відповідають вашим потребам."
    items: 
          
        # operation loop 1
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "Динамічно створювати та додавати штрих-коди до документів"

        # operation loop 2
        - name: "Візуалізувати дані за допомогою діаграм"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "Заповнити різні типи діаграм даними"

        # operation loop 3
        - name: "Об'єднувати документи"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "Об'єднати вміст одного документа в інший"

        # operation loop 4
        - name: "Відображати дані за допомогою списків"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "Генерувати списки в документах, використовуючи специфічні дані"

        # operation loop 5
        - name: "Організовувати дані в таблицях"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "Витягувати дані з будь-якого джерела та заповнювати таблиці"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генеруйте комплексні звіти в різноманітних форматах"
    exclude: "PDF"
    description: "Java дозволяє вам створювати документи з інтегрованими діаграмами у понад 50 форматах файлів, забезпечуючи безшовне злиття шаблонів і даних."
    items: 
          
        # format loop 1
        - name: "Діаграми у PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Діаграми у DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Діаграми у PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Діаграми у XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---