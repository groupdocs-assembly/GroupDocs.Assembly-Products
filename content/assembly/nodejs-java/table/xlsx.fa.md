



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:04
draft: false
lang: fa
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "XLSX: جدول‌ها را با JavaScript وارد کنید"
head_description: "از GroupDocs.Assembly for Node.js via Java برای درج سریع جدول‌ها در مستندات یا ایمیل‌ها استفاده کنید و داده‌ها را از منابع مختلف استخراج کنید."

############################# Header ############################
title: "به راحتی جدول‌ها را به فایل‌های XLSX با Node.js اضافه کنید" 
description: "با GroupDocs.Assembly for Node.js via Java، پر کردن جدول‌ها در مستندات XLSX ساده است و از داده‌های متعدد استفاده می‌کند."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آغاز آزمایش رایگان شما"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "آشنایی با GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ابزاری قدرتمند برای خودکارسازی ایجاد مستندات است. این ابزار به شما امکان می‌دهد به راحتی جدول‌ها، نمودارها، لیست‌ها و تصاویر را به الگوها اضافه کنید و محتوا را به طور دقیق قرار دهید. با پشتیبانی از بیش از ۵۰ فرمت فایل، از جمله PDF، Word و ایمیل، فرآیند ایجاد گزارش و سایر وظایف را تسهیل می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه داده‌ها را به جدول در XLSX اضافه کنیم"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) به شما این امکان را می‌دهد که به سرعت الگوهای جدول را برای فایل‌های XLSX با استفاده از منابع داده داینامیک پر کنید.
      
      1. یک الگوی XLSX با جاهای خالی برای ردیف‌ها و ستون‌های جدول ایجاد کنید.
      2. داده‌ها را از یک منبع پشتیبانی‌شده مانند JSON یا CSV بارگذاری کنید.
      3. داده‌ها را به شکل مطلوب سازماندهی و فرمت دهید.
      4. مستند را با جدول تکمیل‌شده ایجاد کنید.
   
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
        // این تگ‌ها را در جاهای خالی ردیف جدول الگوی خود قرار دهید.
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر فایل الگو را مشخص کنید.
        const template = "table_template.xlsx";

        // داده‌های خود را از منبع انتخابی بارگذاری کنید.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // مستند نهایی را با جدول تکمیل‌شده ذخیره کنید.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "به راحتی جدول‌های مبتنی بر داده را به مستندات اضافه کنید"
  description: "GroupDocs.Assembly for Node.js via Java به کاربران این امکان را می‌دهد که جدول‌ها را به طور خودکار ایجاد کنند و در عین حال نمودارها، تصاویر و لیست‌ها را با استفاده از کارکردهای مبتنی بر الگو ادغام کنند."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "ویژگی‌های برتر GroupDocs.Assembly"
  features:
    # feature loop
    - title: "ایجاد جدول از داده‌های ساختاریافته"
      content: "داده‌ها را از JSON، XML، CSV و سایر فرمت‌ها استخراج کنید تا به طور خودکار جدول‌های مستندات را پر کنید."

    # feature loop
    - title: "ایجاد محتوای بصری حرفه‌ای"
      content: "از GroupDocs.Assembly برای طراحی جدول‌ها، نمودارها و لیست‌های حرفه‌ای استفاده کنید و لینک‌ها، تصاویر و متن را برای ظاهری شیک به مستند اضافه کنید."

    # feature loop
    - title: "قرار دادن محتوای جدول به صورت داینامیک"
      content: "برای افزودن ردیف‌ها و ستون‌ها به صورت برنامه‌نویسی از الگوهای مبتنی بر LINQ استفاده کنید و سبک‌هایی مانند قلم، رنگ‌ها و تراز را سفارشی کنید."

    # feature loop
    - title: "عملکرد بی‌نقص در تمام فرمت‌ها"
      content: "به راحتی جدول‌ها را در فرمت‌های MS Office، OpenOffice، PDF، HTML و دیگر فرمت‌ها ایجاد یا ویرایش کنید و آن‌ها را به فایل‌ها ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه به صورت برنامه‌نویسی یک جدول را پر کنیم"
      content: |
        این مثال پر کردن یک جدول در مستند XLSX را با داده‌هایی از یک منبع خارجی نشان می‌دهد.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // یک الگو طراحی کنید که جاهای خالی برای جدول داشته باشد.
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // مسیر فایل الگو را مشخص کنید.
          const template = "table_template.xlsx";

          // داده‌های مورد نیاز را از منبع خود بارگذاری کنید.
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // داده‌ها را به ساختار مورد نیاز سازماندهی کنید.
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // اقدام به راه‌اندازی DocumentAssembler کنید.
          const asm = new assemblyLib.DocumentAssembler();

          // مستند خروجی را با جدول تکمیل‌شده ذخیره کنید.
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_table.xlsx"
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
    title: "ویژگی‌های اصلی در یک نگاه"
    exclude: "table"
    description: "API ما ایجاد جدول را خودکار می‌کند و فرآیند تولید مستند را با ابزارها و الگوهای چندمنظوره بهبود می‌بخشد."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ایجاد جدول در انواع فرمت‌ها"
    exclude: "XLSX"
    description: "با Node.js via Java، الگوها را پر کنید و جدول‌های جامع ایجاد کنید که شامل بیش از ۵۰ نوع فایل پشتیبانی‌شده است."
    items: 
          
        # format loop 1
        - name: "اضافه کردن جدول به PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن جدول به DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "اضافه کردن جدول به PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "اضافه کردن جدول به XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---