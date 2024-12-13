



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: fa
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ایجاد جداول در اسناد PPTX با C#"
head_description: "API GroupDocs.Assembly for .NET به توسعه‌دهندگان این امکان را می‌دهد که به راحتی جداول را در اسناد و ایمیل‌ها با داده‌های منابع پویا اضافه و پر کنند."

############################# Header ############################
title: "تولید جداول داده‌ای در اسناد PPTX با استفاده از API .NET ما" 
description: "GroupDocs.Assembly for .NET به شما این امکان را می‌دهد که به‌طور پویا جداول را در اسناد PPTX با داده‌های منابع مختلف پر کنید."
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
    title: "بررسی اجمالی GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) برای ایجاد اسناد و گزارش‌ها با پر کردن الگوها با داده‌های منابع متعدد ساخته شده است. به راحتی می‌توان داده‌های ساختاریافته را در جداول، فهرست‌ها و نمودارها درج کرد یا تصاویر را به‌طور پویا وارد کرد. نحو پیشرفته اطمینان می‌دهد که داده‌ها به درستی قرار داده شوند. پشتیبانی از بیش از 50 فرمت، از جمله PDF، اسناد MS Office و فایل‌های ایمیل.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک جدول را در سند PPTX پر کنیم"
    content: |
      [GroupDocs.Assembly](/assembly/net/) به شما این امکان را می‌دهد که جداول را به‌طور پویا در الگوهای فرمت‌های PPTX پر کنید. داده‌ها را از منابع مختلف به جداول خود وارد کنید.
      
      1. یک الگوی PPTX با جای‌گذاری‌های جدول ایجاد کنید.
      2. داده‌ها را از هر منبع پشتیبانی‌شده استخراج کنید.
      3. داده‌ها را فیلتر کنید تا فقط اطلاعات مورد نیاز را شامل شود.
      4. سند را با جدول پر شده ذخیره کنید.
   
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
        // این تگ‌ها را به یک ردیف جدول الگو اضافه کنید
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // مسیر فایل را برای قالب تعیین کنید
        string template = "table_template.pptx";

        // داده‌ها را از یک منبع پشتیبانی‌شده استخراج کنید
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // سند را با جدول پر شده با داده‌ها ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ایجاد اسناد با جداول پویا"
  description: "GroupDocs.Assembly for .NET روند ایجاد سند را با اتوماسیون پر کردن جداول و پشتیبانی از عناصر اضافی مانند نمودارها، فهرست‌ها و تصاویر از طریق الگوها و نشانه‌گذاری پیشرفته ساده می‌کند."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "ایجاد گزارش از داده‌های ساختار یافته"
      content: "API داده‌ها را از منابعی مانند JSON، XML و CSV پردازش می‌کند تا جداول را به‌طور کارآمد و دقیق در اسناد اداری پر کند."

    # feature loop
    - title: "نمایش بصری داده‌ها"
      content: "GroupDocs.Assembly امکان ایجاد جداول، فهرست‌ها و نمودارها را فراهم می‌کند و همچنین متن، لینک‌ها و تصاویر را برای طراحی حرفه‌ای اسناد درج می‌کند."

    # feature loop
    - title: "موقعیت دقیق داده‌های جدول"
      content: "از نحو مبتنی بر LINQ برای افزودن به‌طور پویا سطرها و ستون‌های جدول استفاده کنید. سبک‌ها، از جمله رنگ‌ها و فرمت‌ها را به‌طور برنامه‌نویسی سفارشی کنید."

    # feature loop
    - title: "پشتیبانی از طیف وسیعی از فرمت‌ها"
      content: "به راحتی فرمت‌های محبوبی مانند MS Office، OpenOffice، PDF و HTML را مدیریت کنید. جداول پرشده را به طور یکپارچه در انواع سندهای پشتیبانی‌شده وارد کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک جدول داده را به‌طور پویا پر کنیم"
      content: |
        این مثال نشان می‌دهد که چگونه یک جدول در سند PPTX را با استفاده از داده‌های پویا پر کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // یک الگو با یک جای‌گذاری برای جدول آماده کنید
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // مسیر فایل را به الگو مشخص کنید
          string template = "table_template.pptx";

          // داده‌ها را از منبع انتخابی خود بازیابی کنید
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // یک شیء منبع داده با داده‌های لازم ایجاد کنید
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // مقداردهی DocumentAssembler را انجام دهید
          DocumentAssembler asm = new DocumentAssembler();

          // سند کامل شده با جدول پر شده را ذخیره کنید
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    exclude: "table"
    description: "راه‌حل ما فرآیند ایجاد اسناد حرفه‌ای را با جداول پرشده به‌طور پویا و عناصر اضافی ساده می‌کند."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ایجاد گزارش‌ها با جداول تفصیلی"
    exclude: "PPTX"
    description: ".NET امکان ایجاد گزارش‌های جامع را با پر کردن الگوها با جداول و سایر عناصر داده در بیش از 50 فرمت پشتیبانی‌شده فراهم می‌آورد."
    items: 
          
        # format loop 1
        - name: "اضافه کردن جدول به PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن جدول به DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "اضافه کردن جدول به PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "اضافه کردن جدول به XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---