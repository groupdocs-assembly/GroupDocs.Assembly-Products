



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: fa
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "گنجاندن بارکدها در فایل‌های XLSX با Java"
head_description: "API GroupDocs.Assembly for Java ساخت و درج تصاویر بارکد را در اسناد و ایمیل‌های شما به‌طور زنده ساده می‌کند."

############################# Header ############################
title: "تولید بارکد برای فایل‌های XLSX با API Java ما" 
description: "GroupDocs.Assembly for Java ابزارهای جامع برای ایجاد، سفارشی‌سازی و گنجاندن بارکدها در فایل‌های XLSX به‌صورت داینامیک فراهم می‌کند."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "هم‌اکنون دانلود کنید"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "چیست GroupDocs.Assembly for Java؟"
    link: "/assembly/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) به شما کمک می‌کند با افزودن داده‌ها از منابع متعدد، اسناد را ایجاد و سفارشی کنید. متن، اعداد، نمودارها، جداول، لیست‌ها، تصاویر و بارکدها را به‌سادگی درج کنید. از الگوهای پیشرفته استفاده کنید تا اطمینان حاصل کنید داده‌ها دقیقاً در جایی که می‌خواهید ظاهر می‌شوند. از بیش از ۵۰ فرمت، از جمله PDF، فایل‌های Office و ایمیل‌ها پشتیبانی می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک بارکد را در سند XLSX گنجانده‌ام"
    content: |
      [GroupDocs.Assembly](/assembly/java/) به شما اجازه می‌دهد بارکدها را در فرمت‌های محبوب مانند الگوهای XLSX درج کنید. از بیش از ۶۰ نوع پشتیبانی می‌کند، از جمله بارکدهای ۱ بعدی و ۲ بعدی.
      
      1. یک الگوی XLSX با نشانگرهای بارکد تنظیم کنید.
      2. داده‌ها را از یک منبع پشتیبانی شده دریافت کنید.
      3. تنظیمات بارکد همچون اندازه و وضوح را تنظیم کنید.
      4. سند حاوی بارکد را ذخیره کنید.
   
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
        // از این تگ در الگوی خود برای ایجاد بارکد در سند خروجی استفاده کنید
        // <<barcode [barcode_expression] -barcode_type>>

        // مسیر فایل برای الگو را تعیین کنید
        String template = "barcode_template.xlsx";

        // داده‌ها را از منبع خود دریافت کنید
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // سند به‌روز شده با بارکد را ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ایجاد اسناد با استفاده از الگوهای مبتنی بر داده"
  description: "GroupDocs.Assembly for Java ایجاد اسناد را در انواع فایل‌های محبوب ساده می‌کند. از الگوها برای افزودن نمودارها، جداول، لیست‌ها، لینک‌ها، تصاویر و بارکدها به‌طور یکپارچه استفاده کنید."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تولید گزارش با استفاده از داده‌های کسب‌وکار"
      content: "این API اسناد را با داده‌هایی از فرمت‌هایی مانند JSON، XML و CSV به‌طور کارآمد و دقیق پر می‌کند."

    # feature loop
    - title: "تصویرسازی داده‌ها با عناصر داخلی"
      content: "GroupDocs.Assembly از عناصر داخلی مانند جداول، نمودارها و لیست‌ها، همراه با متن، لینک‌ها، تصاویر و تولید بارکد به‌صورت زنده پشتیبانی می‌کند."

    # feature loop
    - title: "درج داده‌ها در مکان مورد نیاز"
      content: "با الگوهای مبتنی بر LINQ، می‌توانید داده‌ها را به‌طور دقیق قرار دهید، از حلقه‌ها برای افزودن آرایه‌ها استفاده کنید و فرمت‌بندی‌هایی مانند رنگ را به‌طور برنامه‌نویسی سفارشی کنید."

    # feature loop
    - title: "سازگاری گسترده با انواع فایل‌ها"
      content: "فایل‌هایی مانند اسناد MS Office، PDF، HTML، OpenOffice و ایمیل‌ها را مدیریت کنید. همچنین می‌توانید یک سند را با دیگری ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک بارکد به‌طور دینامیک ایجاد کنید"
      content: |
        این مثال نشان می‌دهد که چگونه به طور دینامیک یک بارکد تولید و به سند XLSX اضافه کنید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک الگو با یک جایگزین بارکد آماده کنید
          // <<barcode [barcode_expression] -barcode_type>>

          // مسیر فایل الگوی خود را تنظیم کنید
          String template = "barcode_template.xlsx";

          // داده‌ها را از یک منبع خاص بارگذاری کنید
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // یک شی منبع داده با داده‌های لازم بسازید
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // یک نمونه از DocumentAssembler ایجاد کنید
          DocumentAssembler asm = new DocumentAssembler();

          // تنظیمات بارکد را سفارشی کنید
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // سند به‌روز شده را با بارکد ذخیره کنید
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: "کشف ویژگی‌های کلیدی"
    exclude: "barcode"
    description: "پلتفرم ما مدیریت اسناد تجاری را با ابزارها و اتوماسیون قدرتمند ساده می‌کند."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "تولید گزارش در فرمت‌های مختلف"
    exclude: "XLSX"
    description: "Java از بیش از ۵۰ نوع فایل پشتیبانی می‌کند و ادغام داده و پردازش الگوها را برای نتایج حرفه‌ای تسهیل می‌کند."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/assembly/java/barcode/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/assembly/java/barcode/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/assembly/java/barcode/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/assembly/java/barcode/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---