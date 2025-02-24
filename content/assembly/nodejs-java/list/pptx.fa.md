



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: fa
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ایجاد لیست‌های دینامیک در PPTX با JavaScript"
head_description: "طراحی و وارد کردن لیست‌ها به قالب‌های PPTX با استفاده از API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "گنجاندن لیست‌های مبتنی بر داده در فایل‌های PPTX با Node.js" 
description: "GroupDocs.Assembly for Node.js via Java ابزارهای قدرتمندی برای افزودن لیست‌های انعطاف‌پذیر و مبتنی بر داده به اسناد PPTX ارائه می‌دهد."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "شروع کنید به صورت رایگان"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) فرآیند ایجاد مستندات را با استخراج داده از منابع مختلف و گنجاندن آن در قالب‌ها ساده می‌کند. از آن برای ساخت لیست‌ها، جدول‌ها، نمودارها و سایر عناصر استفاده کنید، با گزینه‌های دقیق تنظیم و فرمت‌دهی. با پشتیبانی از بیش از 50 فرمت، از جمله PDF، MS Office و ایمیل‌ها، به خودکارسازی فرآیند تولید سند کمک می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل وارد کردن یک لیست به فایل PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) افزودن لیست‌های دقیق و مبتنی بر داده به قالب‌های PPTX شما را تسهیل می‌کند.
      
      1. یک قالب PPTX ایجاد کرده و جاهای خالی برای لیست تعریف کنید.
      2. مسیر فایل قالب را فراهم کنید.
      3. داده‌ها را از منابع پشتیبانی شده مانند JSON یا XML بارگذاری کنید.
      4. سند را با لیست تولید شده ذخیره کنید.
   
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
        // این تگ را در قالب خود قرار دهید تا نشان دهد لیست کجا قرار می‌گیرد
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر فایل قالب خود را تنظیم کنید
        const template = "list_template.pptx";

        // داده‌ها را از منبعی که می‌خواهید استفاده کنید دریافت کنید
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // فایل را با لیست گنجانده شده ذخیره کنید
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "تولید مستندات به سادگی با داده‌های یکپارچه"
  description: "با GroupDocs.Assembly for Node.js via Java، می‌توانید لیست‌ها، جدول‌ها، نمودارها و سایر عناصر را در قالب‌ها گنجانده و زمان و تلاش خود را صرفه‌جویی کنید."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "نکات برجسته GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تولید گزارش از منابع داده متعدد"
      content: "داده‌ها را از JSON، XML، CSV یا سایر فرمت‌ها وارد کنید تا لیست‌ها و سایر اجزا را به کارآمدی پر کنید."

    # feature loop
    - title: "افزودن لیست‌ها و سایر عناصر بصری"
      content: "GroupDocs.Assembly به شما امکان می‌دهد که به طور یکپارچه لیست‌ها، جدول‌ها، نمودارها و دیگر عناصر را در کنار متن، تصاویر و لینک‌ها برای نتایج شکیل قرار دهید."

    # feature loop
    - title: "قرار دادن و استایل‌دهی دقیق به داده‌ها"
      content: "قالب‌های مبتنی بر LINQ به شما اجازه می‌دهند که دقیقاً مشخص کنید لیست‌ها و سایر داده‌ها کجا قرار بگیرند، از حلقه‌ها برای اقلام تکراری استفاده کنید و استایل‌ها را مطابق نیازهای خود سفارشی کنید."

    # feature loop
    - title: "عملکرد در چندین فرمت"
      content: "ایجاد مستندات در فرمت‌هایی مثل MS Office، PDF، OpenOffice، HTML و ایمیل. محتوای مختلف از منابع مختلف را به یک فایل واحد ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "برنامه‌نویسی برای ایجاد یک لیست در یک سند"
      content: |
        این مثال نشان می‌دهد که چگونه به صورت دینامیک یک لیست به سند PPTX با استفاده از GroupDocs.Assembly اضافه کنید.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // یک جا خالی در قالب خود برای لیست اضافه کنید
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // مسیر فایل قالب را مشخص کنید
          const template = "numlist_template.pptx";

          // داده‌ها را برای پر کردن لیست بارگذاری کنید
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // منبع داده را با جزئیات مورد نیاز آماده کنید
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // مقداردهی اولیه به DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // سند نهایی را با لیست شامل شده ذخیره کنید
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "ویژگی‌های GroupDocs.Assembly را کشف کنید"
    exclude: "list"
    description: "طراحی و تولید مستندات غنی از داده به راحتی با استفاده از ابزارهای یکپارچه‌سازی قدرتمند."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ایجاد مستندات در چندین فرمت"
    exclude: "PPTX"
    description: "Node.js via Java از بیش از 50 فرمت فایل پشتیبانی می‌کند و ادغام قالب‌ها و داده‌ها به نتایج حرفه‌ای را تسهیل می‌کند."
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