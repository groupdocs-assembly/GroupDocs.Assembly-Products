



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: fa
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ایجاد لیست‌ها در اسناد PDF با C#"
head_description: "API GroupDocs.Assembly for .NET به توسعه‌دهندگان این امکان را می‌دهد که لیست‌های پرشده با داده‌ها را به طور دینامیک در اسناد و الگوها ایجاد و جاسازی کنند."

############################# Header ############################
title: "اضافه کردن لیست‌های داده‌محور به اسناد PDF با استفاده از API .NET ما" 
description: "GroupDocs.Assembly for .NET ابزارهای قدرتمندی برای تولید و جاسازی لیست‌ها به طور دینامیک در اسناد PDF ارائه می‌دهد."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "نسخه‌ی آزمایشی رایگان را دانلود کنید"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) به منظور ساده‌سازی ایجاد اسناد و گزارش‌ها طراحی شده است و به‌طور یکپارچه داده‌ها را از منابع مختلف ادغام می‌کند. الگوها را با لیست‌ها، نمودارها، جداول، بارکدها یا متن پر کنید و محتوا را به‌طور دقیق با استفاده از نشانه‌گذاری پیشرفته قرار دهید. با پشتیبانی از بیش از 50 فرمت—از جمله PDF، فایل‌های MS Office و ایمیل‌ها—این ابزار برای اتوماسیون جریان‌های کاری اسناد ایده‌آل است.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل افزودن لیست پر شده با داده به سند PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) این امکان را فراهم می‌کند تا به‌راحتی لیست‌های داده‌محور را به الگوهای PDF وارد کنید. لیست‌ها را ایجاد و سفارشی کنید.
      
      1. یک الگو با نقاط تعیین‌شده برای لیست ایجاد کنید (در حال حاضر الگوهای PDF پشتیبانی نمی‌شوند).
      2. مسیر الگو را تنظیم کنید.
      3. داده‌ها را از منابع پشتیبانی‌شده مانند JSON یا XML بازیابی کنید.
      4. سند تکمیل‌شده با لیست را به‌عنوان یک فایل PDF صادر کنید.
   
    code:
      platform: "net"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "سند مثال"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // این برچسب را به الگوی خود اضافه کنید تا مکانی که لیست ظاهر می‌شود، مشخص کنید
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // مسیر فایل الگو را مشخص کنید
        // پشتیبانی از الگوهای PDF در حال حاضر در دسترس نیست.
        string template = "list_template.docx";

        // داده‌ها را از منبع انتخابی خود بازیابی کنید
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // سند را با لیست تولید شده ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ایجاد اسناد با پر کردن الگوها با داده‌های ساختارمند"
  description: "GroupDocs.Assembly for .NET ساخت اسناد داده‌محور را ساده می‌کند. به‌طور دینامیک لیست‌ها، جداول، بارکدها، نمودارها، تصاویر و عناصر دیگر را با الگوهای پیشرفته اضافه کنید."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تولید گزارش‌ها از داده‌های تجاری"
      content: "این API اسناد را در فرمت‌های محبوب با استفاده از داده‌های منابعی مانند JSON، XML، CSV و غیره با دقت و کارایی پر می‌کند."

    # feature loop
    - title: "استفاده از لیست‌ها و عناصر دیگر برای ارائه داده‌ها"
      content: "GroupDocs.Assembly به شما این امکان را می‌دهد که لیست‌ها، جداول و نمودارها را به همراه متن، بارکدها، لینک‌های وب و تصاویر برای ایجاد اسناد ساختارمند خوب جاسازی کنید."

    # feature loop
    - title: "جایگذاری دقیق داده‌ها در مکان‌های مورد نیاز"
      content: "از نحو مبتنی بر LINQ برای قرار دادن لیست‌ها و دیگر عناصر داده‌ای با دقت استفاده کنید. از حلقه‌ها برای پر کردن دینامیک لیست‌ها استفاده کنید و قالب‌بندی سفارشی را به‌طور برنامه‌نویسی اعمال کنید."

    # feature loop
    - title: "پشتیبانی از چندین فرمت سند"
      content: "اسناد را در فرمت‌های مختلفی مانند MS Office، OpenOffice، PDF، HTML و فایل‌های ایمیل تولید و مدیریت کنید. به‌راحتی چندین سند را به یک فایل واحد ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه به‌طور دینامیک یک لیست تولید کنیم"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید یک لیست تولید شده به‌طور دینامیک را در یک سند PDF جاسازی کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // یک برچسب نشانه‌گذاری به الگوی خود برای لیست اضافه کنید
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // مسیر فایل الگو را مشخص کنید
          // پشتیبانی از الگوهای PDF در حال حاضر در دسترس نیست.
          string template = "numlist_template.docx";

          // داده‌ها را برای پر کردن لیست بازیابی کنید
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // یک شیء منبع داده با اطلاعات لازم ایجاد کنید
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // DocumentAssembler را مقداردهی اولیه کنید
          DocumentAssembler asm = new DocumentAssembler();

          // سند نهایی را با لیست تولید شده ذخیره کنید
          asm.AssembleDocument(template, "result.pdf", data);
          ```
        platform: "net"
        copy_title: "کپی"
        install:
          command: "dotnet add package GroupDocs.Assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "آماده برای شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Assembly را رایگان آزمایش کنید یا درخواست مجوز نمایید"
  items:
    #  loop
    - title: "دانلود از Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "درباره مجوزدهی بیاموزید"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "کشف قابلیت‌های کلیدی"
    exclude: "list"
    description: "پلتفرم ما برای ساده‌سازی ایجاد و ادغام محتوای داده‌محور سند طراحی شده است."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ایجاد اسناد ساختارمند در فرمت‌های محبوب"
    exclude: "PDF"
    description: ".NET از بیش از 50 فرمت پشتیبانی می‌کند و به شما امکان می‌دهد که داده‌ها و الگوها را به‌صورت یکپارچه ادغام کرده و نتایج ساختار یافته و کامل تولید کنید."
    items: 
          
        # format loop 1
        - name: "ایجاد یک لیست در PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "ایجاد یک لیست در DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "ایجاد یک لیست در PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "ایجاد یک لیست در XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---