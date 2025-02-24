



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:07
draft: false
lang: ru
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Вставьте один документ в другой в DOCX с использованием Java"
head_description: "Объединяйте файлы DOCX с помощью Java. GroupDocs.Assembly упрощает процесс объединения документов всего за несколько строк кода."

############################# Header ############################
title: "Встраивайте содержимое в файлы DOCX без усилий" 
description: "Используйте GroupDocs.Assembly for Java для бесшовной вставки одного документа DOCX в другой. Получайте точные результаты с гибкими и надежными инструментами."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Получить бесплатно"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Что такое GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) является универсальным решением для работы с документами. Оно позволяет интегрировать один документ в другой, поддерживая более 50 форматов, таких как PDF и файлы MS Office. Настройте выходные данные, объединяя, редактируя и организуя содержимое именно так, как вам нужно.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для вставки документа в файл DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) упрощает встраивание одного документа DOCX в другой и настраивается по вашему усмотрению.
      
      1. Подготовьте шаблон DOCX с заполнителями для встраиваемого содержимого.
      2. Укажите путь к файлу шаблона.
      3. Укажите путь к документу для встраивания.
      4. Сохраните выходной файл с объединенным содержимым.
   
    code:
      platform: "java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Пример документа"
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
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Используйте этот тег в своем шаблоне, чтобы отметить место для встраиваемого документа
        // <<doc [doc_expression]>>

        // Укажите путь к основному шаблону
        String template = "doc_template.docx";

        // Укажите путь к документу, который хотите вставить
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Сохраните конечный файл с встраиваемым содержимым
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные инструменты для упрощения интеграции документов"
  description: "С помощью GroupDocs.Assembly for Java встраивание документов становится простым и настраиваемым независимо от типа файла. Достигайте чистых и согласованных результатов в ваших проектах."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Основные возможности GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Создание отчетов с использованием бизнес-данных"
      content: "Заполняйте документы данными из таких источников, как JSON, XML или CSV быстро и надежно, оптимизируя ваши рабочие процессы."

    # feature loop
    - title: "Улучшение документов визуальным содержимым"
      content: "GroupDocs.Assembly позволяет вам вставлять таблицы, диаграммы и списки вместе с текстом, гиперссылками, изображениями и динамическими штрих-кодами."

    # feature loop
    - title: "Размещайте данные именно там, где это необходимо"
      content: "Шаблоны LINQ помогают точно позиционировать ваши данные, обрабатывать повторяющиеся элементы, такие как массивы, и легко применять пользовательские стили."

    # feature loop
    - title: "Совместимость с различными форматами файлов"
      content: "Объединяйте документы различных форматов, включая PDF, HTML, файлы MS Office и OpenOffice, обеспечивая гибкость для ваших проектов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как программно вставить изображение в документ"
      content: |
        Этот пример показывает, как встроить изображение в файл DOCX с помощью GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Добавьте заполнитель в файле шаблона
          // <<image [expression]>>

          // Определите путь к шаблону
          String template = "template.docx";

          // Укажите путь к изображению
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Инициализируйте экземпляр DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Сохраните файл с встраиваемым изображением
          asm.assembleDocument(template, "result.docx", data);
          ```
        platform: "java"
        copy_title: "Копировать"
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
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.docx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Изучите возможности GroupDocs.Assembly бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачать с Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Узнать о лицензировании"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ключевые возможности в одном взгляде"
    exclude: "document"
    description: "Откройте для себя широкий спектр функций, которые предлагает GroupDocs.Assembly для эффективного и беспроблемного встраивания и объединения документов."
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Объединение различных типов документов"
    exclude: "DOCX"
    description: "С помощью Java вы можете встраивать и объединять содержимое более чем в 50 форматах файлов. Добавляйте файлы без проблем для создания профессиональных результатов."
    items: 
          
        # format loop 1
        - name: "Вставить документ в PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Вставить документ в DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Вставить документ в PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Вставить документ в XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---