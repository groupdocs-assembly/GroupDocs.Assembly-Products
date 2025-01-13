



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:20
draft: false
lang: fa
format: Pdf
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
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {texts_pdf.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {texts_pdf.step_4}
   
    code:
      platform: "java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "سند مثال"
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
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```java {style=abap}
        // {examples.comment_1}
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // {examples.comment_2}
        // {texts_pdf.comment_tmp}
        String template = "list_template.docx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
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
          // {texts_pdf.comment_tmp}
          String template = "numlist_template.docx";

          // {code_1.comment_3}
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // {code_1.comment_5}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "کپی"
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
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.pdf"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "آماده برای شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Assembly را رایگان آزمایش کنید یا درخواست مجوز نمایید"
  items:
    #  loop
    - title: "دانلود از NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "درباره مجوزدهی بیاموزید"
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
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "PDF"
    description: ""
    items: 
          
        # format loop 1
        - name: "ایجاد یک لیست در PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "ایجاد یک لیست در DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "ایجاد یک لیست در PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "ایجاد یک لیست در XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---