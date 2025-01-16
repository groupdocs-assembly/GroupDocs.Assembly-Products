



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:03:59
draft: false
lang: fa
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "اضافه کردن بارکد به فایل‌های PDF با استفاده از JavaScript"
head_description: "بارکدها را به سرعت در اسناد و ایمیل‌های خود با استفاده از API GroupDocs.Assembly for Node.js via Java تولید و درج کنید."

############################# Header ############################
title: "ایجاد بارکد برای فایل‌های PDF با استفاده از Node.js" 
description: "با GroupDocs.Assembly for Node.js via Java، می‌توانید بارکدها را به‌طور پویا تولید، سفارشی کرده و در اسناد PDF درج کنید."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "شروع کنید"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "مقدمه‌ای بر GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) به شما این امکان را می‌دهد که اسناد حرفه‌ای را با ترکیب داده‌ها از منابع مختلف ایجاد کنید. نمودارها، جداول، لیست‌ها، تصاویر و بارکدها را به فایل‌های خود اضافه کنید. از قالب‌ها برای سازماندهی محتوا در جای مناسب استفاده کنید. با بیش از 50 فرمت، از جمله PDF، اسناد Office و ایمیل‌ها کار می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل اضافه کردن بارکد در فایل‌های PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) این امکان را به شما می‌دهد تا بارکدها را در اسناد PDF درج کنید. این ابزار از بیش از 60 نوع بارکد شامل فرمت‌های 1D و 2D پشتیبانی می‌کند.
      
      1. یک قالب با مکان‌نگهدارهای بارکد طراحی کنید (قالب‌های PDF پشتیبانی نمی‌شوند).
      2. داده‌ها را از یک منبع سازگار استخراج کنید.
      3. گزینه‌های بارکد مانند اندازه و وضوح را تنظیم کنید.
      4. سند را با بارکد به صورت یک فایل PDF صادر کنید.
   
    code:
      platform: "java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "سند مثال"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
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
        ```javascript {style=abap}
        // از این برچسب در قالب استفاده کنید تا یک بارکد در سند خروجی درج شود.
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر فایل قالب را مشخص کنید.
        // توجه: قالب‌های PDF در حال حاضر پشتیبانی نمی‌شوند.
        const template = "barcode_template.docx";

        // داده‌های مورد نیاز را از منبع خود بارگذاری کنید.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // سند را با بارکد به صورت یک فایل PDF صادر کنید.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ایجاد اسناد با قالب‌های مبتنی بر داده"
  description: "با GroupDocs.Assembly for Node.js via Java، شما می‌توانید فایل‌های حرفه‌ای را در فرمت‌های محبوب با درج بی‌وقفه نمودارها، جداول، لیست‌ها، لینک‌ها، تصاویر و بارکدها ایجاد کنید."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "ایجاد گزارش با داده‌های تجاری"
      content: "از API برای پر کردن قالب‌ها با داده‌ها از فرمت‌هایی مانند JSON، XML و CSV به‌سرعت و دقت استفاده کنید."

    # feature loop
    - title: "اضافه کردن عناصر تصویری"
      content: "GroupDocs.Assembly امکان درج عناصری مانند نمودارها، جداول، لیست‌ها، متن، لینک‌ها، تصاویر و بارکدها را به‌صورت بلادرنگ پشتیبانی می‌کند."

    # feature loop
    - title: "کنترل مکان‌گذاری داده‌ها"
      content: "با استفاده از قالب‌های مبتنی بر LINQ، می‌توانید داده‌ها را به‌دقت قرار دهید، در آرایه‌ها حلقه بزنید و فرمتی سفارشی را به‌صورت برنامه‌نویسی اعمال کنید."

    # feature loop
    - title: "سازگار با بسیاری از فرمت‌ها"
      content: "با فایل‌هایی مانند اسناد MS Office، PDF، HTML، فایل‌های OpenOffice و ایمیل‌ها کار کنید. در صورت نیاز، چندین سند را ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "مثال: تولید بارکد به‌صورت برنامه‌نویسی"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید به‌صورت برنامه‌نویسی یک بارکد را ایجاد و در یک سند PDF درج کنید.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // قالبی با مکان‌نگهدار بارکد طراحی کنید.
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // مسیر فایل قالب را مشخص کنید.
          // توجه: قالب‌های PDF در حال حاضر پشتیبانی نمی‌شوند.
          const template = "barcode_template.docx";

          // داده‌ها را از منبع خود بارگذاری کنید.
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // یک شیء منبع داده با جزئیات لازم ایجاد کنید.
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // یک نمونه از DocumentAssembler را راه‌اندازی کنید.
          const asm = new assemblyLib.DocumentAssembler();

          // پیکربندی بارکد را تنظیم کنید.
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // سند را با بارکد درج شده ذخیره کنید.
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "کپی"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "بررسی ویژگی‌های کلیدی"
    exclude: "barcode"
    description: "پردازش اسناد را با ابزارهای پیشرفته و قابلیت‌های اتوماسیون ساده کنید."
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
    title: "فرمت‌های فایل پشتیبانی‌شده برای ایجاد گزارش"
    exclude: "PDF"
    description: "Node.js via Java بیش از 50 نوع فایل را مدیریت می‌کند، که ادغام داده‌ها و پردازش قالب‌ها را برای نتایج با کیفیت بالا آسان می‌سازد."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---