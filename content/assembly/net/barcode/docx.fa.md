



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: fa
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "تولید بارکد در اسناد DOCX با استفاده از C#"
head_description: "API GroupDocs.Assembly for .NET به توسعه‌دهندگان امکان می‌دهد تا بارکدهای تصویری را به‌صورت دینامیک در اسناد و ایمیل‌ها تولید و درج کنند."

############################# Header ############################
title: "افزودن بارکد به اسناد DOCX با استفاده از API .NET ما" 
description: "GroupDocs.Assembly for .NET پشتیبانی کامل از ایجاد و درج بارکدها به‌صورت دینامیک در اسناد DOCX را ارائه می‌دهد."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود نسخه آزمایشی رایگان"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) برای کمک به شما در تولید اسناد و گزارش‌ها از طریق یکپارچه‌سازی داده‌ها از منابع متنوع طراحی شده‌است. اسناد را با داده‌های متنی یا عددی پر کنید، نمودارها، جداول و لیست‌ها را ایجاد کنید، یا به‌صورت آنی تصاویر و بارکدها را درج کنید. از نشانه‌گذاری پیشرفته برای قرار دادن دقیق داده‌ها در مکان‌های مورد نیاز استفاده کنید. از بیش از ۵۰ فرمت پشتیبانی می‌کند، از جمله PDF، فایل‌های مایکروسافت آفیس و ایمیل‌ها.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل افزودن یک بارکد تولید شده به سند DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) به شما امکان می‌دهد بارکدها را در الگوها در فرمت‌هایی مانند DOCX درج کنید. از بیش از ۶۰ نوع بارکد، از جمله فرمت‌های یک‌بعدی و دو‌بعدی پشتیبانی می‌کند.
      
      1. یک الگوی DOCX با جاهای خالی بارکد آماده کنید.
      2. داده‌ها را از هر منبع داده پشتیبانی‌شده بازیابی کنید.
      3. خصوصیات اضافی مانند اندازه یا وضوح بارکد را پیکربندی کنید.
      4. الگوی بارکد را به‌عنوان یک سند جدید ذخیره کنید.
   
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
        // این تگ را به الگوی خود اضافه کنید تا بارکدی در سند نهایی تولید شود.
        // <<barcode [barcode_expression] -barcode_type>>

        // مسیر فایل الگو را مشخص کنید.
        string template = "barcode_template.docx";

        // داده‌ها را از منبع خود بازیابی کنید.
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // سند را با بارکد تولید شده ذخیره کنید.
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "تولید اسناد با پر کردن الگوها با داده‌ها"
  description: "GroupDocs.Assembly for .NET برای ساده‌سازی ایجاد اسناد در فرمت‌های محبوب طراحی شده‌است. نمودارها، لیست‌ها، جداول، پیوندهای اینترنتی، تصاویر و بارکدها را با استفاده از الگوها و نشانه‌گذاری پیشرفته اضافه کنید."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Assembly"
  features:
    # feature loop
    - title: "ایجاد گزارش‌ها از داده‌های تجاری"
      content: "API ما به‌طور کارآمد اسناد را در فرمت‌های محبوب اداری با استفاده از داده‌های منابعی مانند JSON، XML و CSV پر می‌کند."

    # feature loop
    - title: "استفاده از عناصر بصری برای نمایش داده‌ها"
      content: "GroupDocs.Assembly از درج عناصر بومی مانند لیست‌ها، جداول و نمودارها، به همراه متن، پیوندهای اینترنتی، تصاویر و بارکدهای تولید شده به‌صورت دینامیک پشتیبانی می‌کند."

    # feature loop
    - title: "درج داده در هر نقطه از سند"
      content: "از سینتکس مبتنی بر LINQ برای قرار دادن داده‌ها دقیقاً در مکان‌های مورد نیاز استفاده کنید. آرایه‌ها را می‌توان با استفاده از حلقه‌های for-each درج کرد و فرمت‌دهی (مانند رنگ) را می‌توان به‌صورت برنامه‌نویسی سفارشی‌سازی کرد."

    # feature loop
    - title: "پشتیبانی از طیف وسیعی از فرمت‌ها"
      content: "فرمت‌های محبوب فایل مانند مایکروسافت آفیس، OpenOffice، PDF، HTML و فرمت‌های مختلف ایمیل را پردازش کنید. به‌صورت نیاز یک سند را داخل سند دیگر جای‌گذاری کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه بارکد را به‌صورت دینامیک تولید کنیم"
      content: |
        این مثال فرایند درج یک بارکد تولید شده به‌صورت دینامیک را در یک سند DOCX نشان می‌دهد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // از این الگو برای درج بارکد در سند استفاده کنید.
          // <<barcode [barcode_expression] -barcode_type>>

          // مسیر فایل الگو را مشخص کنید.
          string template = "barcode_template.docx";

          // داده‌ها را از منبع انتخابی خود بازیابی کنید.
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // یک شیء منبع داده را با تنها داده‌های مورد نیاز ایجاد کنید.
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // مقداردهی اولیه DocumentAssembler.
          DocumentAssembler asm = new DocumentAssembler();

          // خصوصیات اضافی بارکد را تنظیم کنید.
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // سند نهایی را با بارکد درج‌شده ذخیره کنید.
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    title: "اکتشاف ویژگی‌های کلیدی"
    exclude: "barcode"
    description: "راه‌حل ما برای ساده‌سازی نیازهای پردازش اسناد تجاری شما طراحی شده است."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ایجاد گزارش‌ها در فرمت‌های محبوب"
    exclude: "DOCX"
    description: ".NET از تولید گزارش‌ها در بیش از ۵۰ فرمت پشتیبانی می‌کند و به شما امکان می‌دهد داده‌ها و الگوها را به‌صورت یکپارچه ترکیب کنید و نتایج فوق‌العاده‌ای به دست آورید."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---