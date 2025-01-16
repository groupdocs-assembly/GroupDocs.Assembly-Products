



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:00
draft: false
lang: fa
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "اضافه کردن نمودارها به فایل‌های DOCX با JavaScript"
head_description: "با GroupDocs.Assembly for Node.js via Java، توسعه‌دهندگان می‌توانند به‌سرعت نمودارهای دینامیک را با استفاده از منابع داده زنده در اسناد ایجاد و درج کنند."

############################# Header ############################
title: "نمودارها را به فایل‌های DOCX با استفاده از Node.js اضافه کنید" 
description: "GroupDocs.Assembly for Node.js via Java روند ادغام نمودارها به اسناد DOCX با ورودی داده‌های بلادرنگ را تسهیل می‌کند."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "هم‌اکنون رایگان شروع کنید"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) یک راه‌حل قوی برای ایجاد اسناد و گزارشات خودکار است. می‌توانید به‌دقت نمودارها، جداول، تصاویر، بارکدها و لیست‌ها را به فایل‌ها اضافه کنید. این پلتفرم چندمنظوره از بیش از ۵۰ فرمت، از جمله PDF، اسناد آفیس و ایمیل‌ها پشتیبانی می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل افزودن یک نمودار به سند DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) افزودن نمودارها به فایل‌های DOCX را ساده می‌کند. از انواع نمودار مانند میله‌ای، خطی یا دایره‌ای انتخاب کنید.
      
      1. یک الگوی DOCX با جایگاه‌های خالی برای نمودارها طراحی کنید.
      2. داده‌ها را از یک منبع پشتیبانی شده بارگذاری کنید.
      3. گزینه‌های نمودار شامل نوع، رنگ‌ها و برچسب‌ها را پیکربندی کنید.
      4. سند را با نمودار درج‌شده صادر کنید.
   
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
        // این تگ را در الگوی خود قرار دهید تا یک نمودار تولید شود
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر فایل الگو را مشخص کنید
        const template = "chart_template.docx";

        // داده‌ها را از سیستم منبع خود استخراج نمایید
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // سند نهایی را با نمودار درج‌شده ذخیره کنید
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "به‌راحتی نمودارها را در اسناد خود ادغام کنید"
  description: "GroupDocs.Assembly for Node.js via Java ایجاد اسناد غنی از ویژگی را در انواع فایل‌های معروف آسان می‌کند. از الگوها برای افزودن نمودارها، جداول، بارکدها، لیست‌ها، تصاویر و بیشتر با به‌روزرسانی‌های داده بلادرنگ استفاده کنید."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "ویژگی‌های برتر GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تبدیل داده‌ها به نمودارهای حرفه‌ای"
      content: "داده‌ها را از منابعی مانند JSON، XML یا CSV به نمودارهای باکیفیت تبدیل کنید که می‌توانند به‌طور مستقیم در اسناد درج شوند."

    # feature loop
    - title: "ایجاد جلوه‌های بصری خیره‌کننده"
      content: "نمودارهای میله‌ای، نمودارهای دایره‌ای و نمودارهای خطی تولید کنید که به‌طور یکپارچه با دیگر عناصر سند مانند تصاویر، جداول و بارکدها کار می‌کنند."

    # feature loop
    - title: "قابلیت‌های انعطاف‌پذیر در طراحی و جایگذاری نمودار"
      content: "از الگوهای LINQ برای کنترل موقعیت و طراحی نمودار، از جمله رنگ‌ها، طرح‌ها و برچسب‌ها استفاده کنید تا ارائه‌ای زیبا داشته باشید."

    # feature loop
    - title: "پشتیبانی از فرمت‌های مختلف فایل"
      content: "اسناد را در فرمت‌هایی مانند MS Office، PDF، OpenOffice و HTML تولید کنید، با نمودارهایی که به‌طور کامل ادغام شده‌اند برای یک نتیجه حرفه‌ای."
      
  code_samples_ext:
    # code sample ext loop
    - title: "تولید و درج نمودارها به‌صورت دینامیک"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید به‌صورت برنامه‌نویسی نمودارها را در فایل‌های DOCX ایجاد و درج کنید.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // یک الگو با یک جایگاه برای نمودار آماده کنید
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // مسیر فایل الگو را تعیین کنید
          const template = "table_template.docx";

          // داده‌ها را از یک منبع انتخاب شده دریافت کنید
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // یک شی داده شامل اطلاعات نمودار آماده کنید
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // نوع نمودار را انتخاب کنید و ظاهر آن را سفارشی کنید
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // DocumentAssembler را راه‌اندازی کنید
          const asm = new assemblyLib.DocumentAssembler();

          // سند به‌روز شده را با نمودار درج شده ذخیره کنید
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "کشف ویژگی‌های پیشرفته"
    exclude: "chart"
    description: "این پلتفرم ایجاد اسناد را با ابزارهایی که برای تجزیه و تحلیل داده‌ها و ادغام یکپارچه طراحی شده‌اند، تسهیل می‌کند."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "تولید گزارش‌ها در فرمت‌های مختلف فایل"
    exclude: "DOCX"
    description: "Node.js via Java از بیش از ۵۰ فرمت پشتیبانی می‌کند، و این امکان را می‌دهد که الگوها را با داده‌ها ترکیب کنید تا اسناد شکیل تولید نمایید."
    items: 
          
        # format loop 1
        - name: "نمودارها در PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "نمودارها در DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "نمودارها در PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "نمودارها در XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---