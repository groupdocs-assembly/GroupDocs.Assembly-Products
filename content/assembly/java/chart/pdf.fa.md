



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: fa
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "تولید نمودارها در اسناد PDF با استفاده از Java"
head_description: "API GroupDocs.Assembly for Java به توسعه‌دهندگان این امکان را می‌دهد که به‌صورت یکپارچه نمودارها یا گراف‌های دینامیک را در اسناد قرار دهند که از داده‌های زنده بهره می‌برند."

############################# Header ############################
title: "اضافه کردن نمودارها به اسناد PDF با API Java" 
description: "GroupDocs.Assembly for Java روند قرار دادن نمودارها در اسناد PDF را با استفاده از داده‌های زنده ساده می‌کند."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "برای شروع رایگان ثبت‌نام کنید"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "معرفی GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) یک راه‌حل چندمنظوره برای اتوماسیون ایجاد مستندات و گزارش‌ها است. این ابزار به شما اجازه می‌دهد که نمودارها، جداول، لیست‌ها، بارکدها و تصاویر را مستقیماً به فایل‌های خود اضافه کنید و ابزارهای پیشرفته‌ای برای فرمت‌بندی دقیق و یکپارچه‌سازی داده‌ها در اختیار دارید. این پلتفرم از بیش از ۵۰ فرمت، از جمله PDF، فایل‌های مایکروسافت آفیس و ایمیل‌ها پشتیبانی می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل قرار دادن یک نمودار در سند PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) روند قرار دادن نمودارها در الگوهای PDF را ساده می‌کند. از سبک‌های مختلف نمودار، از جمله نمودارهای میله‌ای، دایره‌ای و خطی انتخاب کنید.
      
      1. یک الگو با جایگاه‌هایی برای نمودار ایجاد کنید (الگوهای PDF پشتیبانی نمی‌شوند).
      2. داده‌های خود را از یک منبع سازگار بارگذاری کنید.
      3. گزینه‌های نمودار، از جمله نوع، برچسب‌ها و رنگ‌ها را تعیین کنید.
      4. سند حاوی نمودار را به عنوان یک فایل PDF ذخیره کنید.
   
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
        // این تگ را به الگوی خود اضافه کنید تا یک نمودار شامل شود
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // مسیر فایل الگوی خود را مشخص کنید
        // در حال حاضر الگوهای PDF پشتیبانی نمی‌شوند.
        String template = "chart_template.docx";

        // داده‌های لازم را از منبع خود استخراج کنید
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // سند نهایی را با نمودار جاسازی شده ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "به‌سادگی نمودارهای دینامیک را در اسناد خود جاسازی کنید"
  description: "GroupDocs.Assembly for Java راهی آسان برای ایجاد اسناد غنی از داده در فرمت‌های محبوب ارائه می‌دهد. از الگوها برای وارد کردن نمودارها، جداول، بارکدها، لیست‌ها، لینک‌ها و تصاویر با به‌روزرسانی‌های دینامیک از داده‌های خود استفاده کنید."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "به‌راحتی داده‌ها را به نمودارها تبدیل کنید"
      content: "از API برای تبدیل داده‌ها از JSON، XML، CSV یا دیگر منابع به نمودارهای حرفه‌ای و جلوه‌دار برای اسناد خود استفاده کنید."

    # feature loop
    - title: "محتوای بصری تأثیرگذار ایجاد کنید"
      content: "GroupDocs.Assembly از فرمت‌های بصری مختلفی پشتیبانی می‌کند، از جمله نمودارهای میله‌ای، نمودارهای دایره‌ای و نمودارهای خطی که می‌توانند با جداول، بارکدها، تصاویر و غیره ترکیب شوند تا گزارش‌های بهتری ایجاد کنند."

    # feature loop
    - title: "تعیین موقعیت و سبک نمودار قابل تنظیم"
      content: "با استفاده از سینتکس مبتنی بر LINQ، می‌توانید نمودارها را به‌صورت دینامیک در سند تولید و موقعیت‌یابی کنید و در عین حال به‌راحتی سبک‌ها، رنگ‌ها و چیدمان‌ها را برای دستیابی به نیازهای طراحی خود تنظیم کنید."

    # feature loop
    - title: "پشتیبانی از چندین فرمت سند"
      content: "اسناد را در فرمت‌هایی نظیر MS Office، PDF، OpenOffice و HTML تولید کنید. نمودارها به‌طور روان در هر فرمت پشتیبانی‌شده قرار می‌گیرند و نتایج حرفه‌ای را ارائه می‌دهند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "نمودارها را به‌صورت برنامه‌نویسی تولید و قرار دهید"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان به‌صورت برنامه‌نویسی یک نمودار را به سند PDF اضافه کرد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک الگو با یک جایگاه برای نمودار آماده کنید
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // مسیر فایل الگو را مشخص کنید
          // در حال حاضر الگوهای PDF پشتیبانی نمی‌شوند.
          String template = "table_template.docx";

          // داده‌ها را از منبع انتخابی خود بارگذاری کنید
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // یک شیء داده با اطلاعات مربوطه ایجاد کنید
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // نوع و ظاهر نمودار را تنظیم کنید
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // DocumentAssembler را راه‌اندازی کنید
          DocumentAssembler asm = new DocumentAssembler();

          // سند کامل شده را با نمودار جاسازی شده ذخیره کنید
          asm.assembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "کشف قابلیت‌های قدرتمند"
    exclude: "chart"
    description: "این پلتفرم روند طراحی اسناد متمرکز بر داده و بصری را که به نیازهای شما متناسب است، آسان می‌کند."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "تولید گزارش‌های جامع در فرمت‌های متنوع"
    exclude: "PDF"
    description: "Java به شما اجازه می‌دهد اسنادی با نمودارهای یکپارچه در بیش از ۵۰ فرمت فایل ایجاد کنید و اطمینان حاصل می‌کند که ادغام الگوها و داده‌ها به‌راحتی انجام می‌شود."
    items: 
          
        # format loop 1
        - name: "نمودارها در PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "نمودارها در DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "نمودارها در PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "نمودارها در XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---