



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: ru
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Генерируйте диаграммы в PPTX документах, используя Java"
head_description: "API GroupDocs.Assembly for Java позволяет разработчикам создавать и вставлять динамические диаграммы или графики в документы без усилий, используя актуальные данные."

############################# Header ############################
title: "Добавьте диаграммы в PPTX документы с помощью API Java" 
description: "GroupDocs.Assembly for Java упрощает процесс встраивания диаграмм в PPTX документы, используя данные в реальном времени."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Начать бесплатно"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Введение в GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) — это универсальное решение для автоматизации создания документов и отчетов. Он позволяет вам добавлять диаграммы, таблицы, списки, штрих-коды и изображения прямо в ваши файлы, с передовыми инструментами для точного форматирования и интеграции данных. Платформа поддерживает более 50 форматов, включая PDF, файлы Microsoft Office и электронные письма.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для встраивания диаграммы в документ PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) упрощает процесс вставки диаграмм в шаблоны PPTX. Выбирайте из различных стилей диаграмм, включая столбчатые, круговые и линейные.
      
      1. Создайте шаблон PPTX с заполнительными местами для диаграммы.
      2. Загрузите ваши данные из совместимого источника.
      3. Установите параметры диаграммы, такие как тип, метки и цвета.
      4. Сохраните документ с включенной диаграммой.
   
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
        // Добавьте этот тег в ваш шаблон для включения диаграммы
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Укажите путь к вашему шаблону
        String template = "chart_template.pptx";

        // Извлеките необходимые данные из вашего источника
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Сохраните финальный документ с встраиваемой диаграммой
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Легко встраивайте динамические диаграммы в ваши документы"
  description: "GroupDocs.Assembly for Java предлагает простой способ создания насыщенных данными документов в популярных форматах. Используйте шаблоны для вставки диаграмм, таблиц, штрих-кодов, списков, ссылок и изображений с динамическим обновлением из ваших данных."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Превращайте данные в диаграммы"
      content: "Используйте API, чтобы преобразовать данные из JSON, XML, CSV или других источников в чистые, профессиональные диаграммы для ваших документов."

    # feature loop
    - title: "Создавайте визуально привлекательное содержимое"
      content: "GroupDocs.Assembly поддерживает различные визуальные форматы, включая столбчатые графики, круговые диаграммы и линейные графики, которые могут быть объединены с таблицами, штрих-кодами, изображениями и другими элементами для улучшенных отчетов."

    # feature loop
    - title: "Настраиваемое размещение и стилизация диаграмм"
      content: "С помощью синтаксиса на основе LINQ вы можете динамически генерировать и размещать диаграммы в документе, легко настраивая стили, цвета и макеты в соответствии с вашими потребностями в дизайне."

    # feature loop
    - title: "Поддержка нескольких форматов документов"
      content: "Генерируйте документы в таких форматах, как MS Office, PDF, OpenOffice и HTML. Диаграммы плавно интегрируются в любой поддерживаемый формат для профессиональных результатов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Программно создавайте и встраивайте диаграммы"
      content: |
        Этот пример демонстрирует, как программно создать и встроить диаграмму в документ PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Подготовьте шаблон с заполнительным местом для диаграммы
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Укажите путь к файлу шаблона
          String template = "table_template.pptx";

          // Загрузите данные из выбранного источника
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Создайте объект данных с соответствующей информацией
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Настройте тип и внешний вид диаграммы
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Инициализируйте DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Сохраните завершенный документ с встроенной диаграммой
          asm.assembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "Изучите мощные возможности"
    exclude: "chart"
    description: "Эта платформа упрощает процесс проектирования ориентированных на данные, визуально привлекательных документов, адаптированных к вашим потребностям."
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генерируйте комплексные отчеты в разных форматах"
    exclude: "PPTX"
    description: "Java позволяет создавать документы с интегрированными диаграммами в более чем 50 файловых форматах, обеспечивая бесшовное объединение шаблонов и данных."
    items: 
          
        # format loop 1
        - name: "Диаграммы в PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Диаграммы в DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Диаграммы в PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Диаграммы в XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---