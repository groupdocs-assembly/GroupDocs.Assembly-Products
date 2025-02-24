



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: fa
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ترکیب اسناد در XLSX با JavaScript"
head_description: "با استفاده از JavaScript فایل‌های XLSX را ترکیب کنید. GroupDocs.Assembly ادغام اسناد را در چند مرحله ساده تسریع می‌بخشد."

############################# Header ############################
title: "ادغام محتوای فایل‌های XLSX بدون دردسر" 
description: "با GroupDocs.Assembly for Node.js via Java، ادغام یک فایل XLSX به دیگری سریع و دقیق است. از ابزارهای قابل اعتماد و منعطف برای ادغام روان لذت ببرید."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آزمایش رایگان"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) یک روش قوی برای مدیریت اسناد ارائه می‌دهد. یک فایل را به دیگری بدون زحمت ادغام کنید و از بیش از ۵۰ فرمت، از جمله PDF و MS Office پشتیبانی کنید. طرح‌ها را شخصی‌سازی کنید، محتوا را ویرایش کنید و اسناد را دقیقاً به شیوه‌ای که نیاز دارید سازماندهی کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک سند را به یک فایل XLSX ادغام کنیم"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) به شما امکان می‌دهد یک فایل XLSX را به دیگری با گزینه‌های قابل سفارشی‌سازی اضافه کنید.
      
      1. یک الگوی XLSX با جای‌گذاری برای محتوا طراحی کنید.
      2. مسیر فایل را برای الگو مشخص کنید.
      3. مسیر فایل را برای سندی که می‌خواهید ادغام کنید، ارائه دهید.
      4. فایل نهایی را با محتوای ترکیب شده صادر کنید.
   
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
        // این برچسب را به الگوی خود اضافه کنید تا مشخص کنید کجا سند درج خواهد شد.
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر فایل را برای قالب اصلی تنظیم کنید.
        const template = "doc_template.xlsx";

        // مسیر سندی را که می‌خواهید ادغام کنید، ارائه دهید.
        const data 
            = new assemblyLib.DataSourceInfo("insert.xlsx", "doc_expression");

        // خروجی نهایی را با سند ادغام شده ذخیره کنید.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ابزارهای قدرتمند برای ادغام اسناد"
  description: "GroupDocs.Assembly for Node.js via Java ادغام فایل‌ها را در قالب‌های مختلف آسان و کاملاً قابل سفارشی‌سازی می‌کند. نتایج حرفه‌ای و یکپارچه را هر بار ارائه می‌دهد."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تولید گزارش‌ها با داده‌های تجاری"
      content: "داده‌ها را از منابع JSON، XML یا CSV استخراج کنید تا گزارش‌ها و اسناد جامع را به سرعت و دقت ایجاد کنید."

    # feature loop
    - title: "اضافه کردن عناصر بصری غنی"
      content: "GroupDocs.Assembly به شما امکان می‌دهد جداول، نمودارها، لیست‌ها، تصاویر و بارکدها را در کنار متن و هایپرلینک‌ها درج کنید."

    # feature loop
    - title: "قرارگیری دقیق داده‌ها"
      content: "از الگوهای LINQ برای قرار دادن داده‌ها در مکان دقیق خود استفاده کنید، اشیای تکراری مانند آرایه‌ها را مدیریت کنید و به راحتی سبک‌ها را سفارشی‌سازی کنید."

    # feature loop
    - title: "کار با انواع فرمت‌ها"
      content: "محتوا را در بین فرمت‌هایی مانند PDF، فایل‌های MS Office، HTML و OpenOffice به‌طور یکپارچه ادغام کنید و انعطاف‌پذیری برای تمام پروژه‌ها ارائه دهید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "برنامه‌نویسی برای درج یک تصویر در یک سند"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان یک تصویر را در یک فایل XLSX با استفاده از GroupDocs.Assembly درج کرد.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // یک جای‌گذاری در الگو برای تصویر اضافه کنید.
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // مسیر فایل الگو را مشخص کنید.
          const template = "template.xlsx";

          // مسیر تصویر مورد نظر برای درج را تنظیم کنید.
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // شیء DocumentAssembler را مقداردهی اولیه کنید.
          const asm = new assemblyLib.DocumentAssembler();

          // سند را با تصویر درون‌گریزی ذخیره کنید.
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    exclude: "document"
    description: "ابزارهای جامع را که GroupDocs.Assembly برای ادغام کارآمد و یکپارچه اسناد ارائه می‌دهد، کشف کنید."
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
    title: "ترکیب اسناد در فرمت‌های متعدد"
    exclude: "XLSX"
    description: "با استفاده از Node.js via Java محتوای خود را در بیش از ۵۰ فرمت فایل ادغام کنید و نتایج حرفه‌ای و بی‌نقصی را تضمین کنید."
    items: 
          
        # format loop 1
        - name: "گنجاندن یک سند در PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "گنجاندن یک سند در DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "گنجاندن یک سند در PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "گنجاندن یک سند در XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---