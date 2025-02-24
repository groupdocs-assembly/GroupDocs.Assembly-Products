



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: fa
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "اضافه کردن جداول به مدارک DOCX با استفاده از Java"
head_description: "با استفاده از GroupDocs.Assembly for Java، توسعه‌دهندگان می‌توانند به سرعت جداول را در مدارک و ایمیل‌ها وارد کرده و داده‌ها را از منابع پویا استخراج کنند."

############################# Header ############################
title: "جداول را در فایل‌های DOCX با API Java ما پر کنید" 
description: "GroupDocs.Assembly for Java فرآیند پر کردن جداول در مدارک DOCX را با داده‌هایی از ورودی‌های مختلف ساده می‌کند."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دریافت نسخه آزمایشی رایگان"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java چیست؟"
    link: "/assembly/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) ابزاری برای تولید مدارک و گزارشات با وارد کردن خودکار داده‌ها به الگوهای از پیش طراحی شده است. شما می‌توانید به راحتی جداول، لیست‌ها، نمودارها و تصاویر را اضافه کنید. ویژگی‌های پیشرفته آن به شما این امکان را می‌دهد که محتوا را به دقت در مدارک خود قرار دهید. این ابزار با بیش از 50 نوع فایل، شامل PDF، MS Office و فرمت‌های ایمیل سازگاری دارد.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل برای وارد کردن داده‌ها به جدول DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) به شما در پر کردن الگوهای جدول برای DOCX و سایر فرمت‌ها کمک می‌کند. از داده‌های دینامیک منابع خود استفاده کنید تا به آسانی اجزا را بسازید.
      
      1. یک الگوی DOCX با جاگزاری برای ردیف‌ها و ستون‌های جدول تنظیم کنید.
      2. داده‌ها را از هر منبع ورودی پشتیبانی شده استخراج کنید.
      3. داده‌ها را فیلتر یا پردازش پیش از ورود کنید تا با نیازهای شما مطابقت داشته باشد.
      4. مدرک نهایی را با جدول کامل تولید کنید.
   
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
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // از این تگ‌ها در یک جاگزاری ردیف جدول در الگوی خود استفاده کنید
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // مسیر فایل الگو را تعریف کنید
        String template = "table_template.docx";

        // داده‌ها را از منبع انتخابی خود بارگذاری کنید
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // فایل خروجی را با جدول پر شده ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ایجاد مدارک با جداول پر شده با داده‌ها"
  description: "GroupDocs.Assembly for Java ایجاد جداول را در مدارک شما ساده می‌کند. همچنین از افزودن عناصر مانند نمودارها، لیست‌ها و تصاویر با استفاده از الگوها پشتیبانی می‌کند."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "ویژگی‌های اصلی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تولید گزارش‌ها از چند فرمت داده"
      content: "API به طور یکپارچه با JSON، XML، CSV و سایر فرمت‌ها کار می‌کند تا جداول را با داده‌های منظم در مدارک شما پر کند."

    # feature loop
    - title: "ارائه اطلاعات به صورت بصری"
      content: "GroupDocs.Assembly به شما کمک می‌کند تا جداول، لیست‌ها و نمودارهای حرفه‌ای بسازید و همچنین لینک‌ها، متن و تصاویر را برای ظاهری شیک درج کنید."

    # feature loop
    - title: "قرار دادن محتوای جدول با دقت"
      content: "از نحو LINQ با انعطاف‌پذیری استفاده کنید تا ردیف‌ها و ستون‌ها را به صورت دینامیک اضافه کنید. ظاهر، از جمله سبک‌ها و رنگ‌های قلم را به صورت برنامه‌نویسی سفارشی کنید."

    # feature loop
    - title: "سازگار با چندین فرمت"
      content: "با MS Office، OpenOffice، PDF، HTML و غیره کار کنید. جداول را به هر فرمت فایل پشتیبانی شده به راحتی ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ایجاد دینامیک یک جدول پر شده با داده‌ها"
      content: |
        این مثال نشان می‌دهد چگونه یک جدول را در یک مدارک DOCX با استفاده از داده‌های ورودی دینامیک پر کنید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک الگو با یک جاگزاری برای جدول طراحی کنید
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // محل فایل الگو را تعیین کنید
          String template = "table_template.docx";

          // داده‌ها را از منبع دلخواه خود بارگذاری کنید
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // یک شیء داده شامل فیلدهای ضروری آماده کنید
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // یک نمونه از DocumentAssembler ایجاد کنید
          DocumentAssembler asm = new DocumentAssembler();

          // مدرک را با جدول پر شده ذخیره کنید
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "آماده برای شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Assembly را رایگان آزمایش کنید یا درخواست مجوز نمایید"
  items:
    #  loop
    - title: "دانلود از Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "درباره مجوزدهی بیاموزید"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ویژگی‌های کلیدی در یک نگاه"
    exclude: "table"
    description: "API ما ایجاد مدارک حرفه‌ای را با اتوماسیون پر کردن جداول در کنار سایر اجزای قدرتمند آسان می‌کند."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "تولید جداول دقیق در فرمت‌های مختلف"
    exclude: "DOCX"
    description: "با Java، می‌توانید الگوها را با داده‌ها پر کرده و گزارش‌های دقیقی در بیش از 50 نوع فایل تولید کنید."
    items: 
          
        # format loop 1
        - name: "اضافه کردن جدول به PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن جدول به DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "اضافه کردن جدول به PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "اضافه کردن جدول به XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---