



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:20
draft: false
lang: ru
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: ""
head_description: ""

############################# Header ############################
title: "" 
description: ""
subtitle: "" 

header_actions:
  enable: true
  items:
    #  loop
    - title: ""
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: ""
    link: "/assembly/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {steps.content.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {steps.content.step_4}
   
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
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```java {style=abap}
        // {examples.comment_1}
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // {examples.comment_2}
        String template = "list_template.pptx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "{more_features.image_description}"
  features:
    # feature loop
    - title: "{more_features.feature_1.title}"
      content: "{more_features.feature_1.content}"

    # feature loop
    - title: "{more_features.feature_2.title}"
      content: "{more_features.feature_2.content}"

    # feature loop
    - title: "{more_features.feature_3.title}"
      content: "{more_features.feature_3.content}"

    # feature loop
    - title: "{more_features.feature_4.title}"
      content: "{more_features.feature_4.content}"
      
  code_samples_ext:
    # code sample ext loop
    - title: "{code_1.title}"
      content: |
        {code_1.content}
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // {code_1.comment_1}
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // {code_1.comment_2}
          String template = "numlist_template.pptx";

          // {code_1.comment_3}
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // {code_1.comment_5}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Изучите возможности GroupDocs.Assembly бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачать с NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Узнать о лицензировании"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "list"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Генерация штрих-кодов"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Динамически создавайте и добавляйте штрих-коды в документы"

        # operation loop 2
        - name: "Визуализация данных с помощью диаграмм"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Заполняйте различные типы диаграмм данными"

        # operation loop 3
        - name: "Слияние документов"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Объединяйте содержимое одного документа с другим"

        # operation loop 4
        - name: "Отображение данных с помощью списков"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Генерируйте списки в документах с использованием определенных данных"

        # operation loop 5
        - name: "Организация данных в таблицах"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Извлекайте данные из любых источников и заполняйте таблицы"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "PPTX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Создать список в PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Формат документа Adobe Portable"
          
        # format loop 2
        - name: "Создать список в DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Создать список в PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Создать список в XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---