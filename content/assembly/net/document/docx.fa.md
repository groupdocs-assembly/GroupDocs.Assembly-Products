



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: fa
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ادغام یک سند در سند دیگر در DOCX با API C#"
head_description: "مدیریت اسناد DOCX را با استفاده از C# تسهیل کنید. با GroupDocs.Assembly، فایل‌ها را به طور یکپارچه در چند مرحله ترکیب کنید."

############################# Header ############################
title: "ترکیب اسناد با فرمت DOCX" 
description: "با GroupDocs.Assembly for .NET، می‌توانید به سرعت یک سند DOCX را در سند دیگر قرار دهید. این API ابزارهای قوی برای ادغام دقیق اسناد ارائه می‌دهد."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET چیست؟"
    link: "/assembly/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ابزاری قدرتمند برای ترکیب و مدیریت اسناد است. به کاربران این امکان را می‌دهد که یک سند را در سند دیگر قرار دهند و به آسانی محتوای آن را ادغام کنند. با پشتیبانی از بیش از 50 فرمت—از جمله PDF، فایل‌های MS Office و بیشتر—می‌توانید خروجی نهایی را به گونه‌ای سازماندهی، ویرایش و سفارشی کنید که نیازهای شما را برآورده سازد.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک سند را به یک فایل DOCX ادغام کنیم"
    content: |
      [GroupDocs.Assembly](/assembly/net/) به شما این امکان را می‌دهد که به سادگی یک سند را در یک فایل DOCX دیگر قرار دهید. محتوا را ادغام و سفارشی کنید.
      
      1. یک الگوی DOCX با جاهای خالی برای سند گنجانده شده طراحی کنید.
      2. مسیر فایل الگو را تعیین کنید.
      3. مسیر فایل سند را که باید گنجانده شود مشخص کنید.
      4. فایل نهایی را با محتوای گنجانده شده ذخیره کنید.
   
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
        // این برچسب را به الگوی خود اضافه کنید تا نقطه درج را علامت‌گذاری کنید
        // <<doc [doc_expression]>>

        // مسیر فایل الگو را مشخص کنید
        string template = "doc_template.docx";

        // مسیر سندی که باید در آن گنجانده شود را فراهم کنید
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // سند ادغام شده را ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ادغام اسناد را با ابزارهای پیشرفته تسهیل کنید"
  description: "کتابخانه GroupDocs.Assembly for .NET embedding یک سند در سند دیگری را ساده می‌کند و از فرمت‌های مختلف پشتیبانی کرده و سفارشی‌سازی برای ادغام بدون درز را فراهم می‌آورد."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "گزارش‌هایی از داده‌های تجاری خود تولید کنید"
      content: "به‌طور خودکار اسناد را با داده‌ها از JSON، XML، CSV یا دیگر منابع پر کنید و اطمینان حاصل کنید که کارها به طور دقیق و مؤثر انجام می‌شود."

    # feature loop
    - title: "اسناد را با عناصر بصری غنی کنید"
      content: "GroupDocs.Assembly به شما امکان می‌دهد جداول، نمودارها و لیست‌ها را شامل کنید و همچنین متن، پیوندها، تصاویر و بارکدهای تولید شده به‌صورت پویا را بیفزایید."

    # feature loop
    - title: "داده‌ها را با دقت قرار دهید و فرمت کنید"
      content: "الگوهای مبتنی بر LINQ به شما کنترل بر روی قرار گرفتن داده‌ها می‌دهند، اجازه می‌دهند حلقه‌ها را برای آرایه‌ها مدیریت کنید و امکان تنظیمات بصری مانند شخصی‌سازی رنگ‌ها را فراهم می‌آورند."

    # feature loop
    - title: "با چندین فرمت فایل کار می‌کند"
      content: "به سادگی اسناد را در فرمت‌هایی مانند MS Office، PDF، HTML، OpenOffice و بیشتر در یکدیگر ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه به‌طور برنامه‌نویسی یک تصویر را به یک سند اضافه کنیم"
      content: |
        این مثال نشان می‌دهد چگونه می‌توان یک تصویر را به یک سند DOCX با استفاده از GroupDocs.Assembly وارد کرد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // یک برچسب جایگزین در الگوی خود اضافه کنید
          // <<image [expression]>>

          // مسیر فایل را برای الگو مشخص کنید
          string template = "template.docx";

          // مسیر فایل تصویر را تعیین کنید
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // یک نمونه از DocumentAssembler را اولیه‌سازی کنید
          DocumentAssembler asm = new DocumentAssembler();

          // سند را با تصویر گنجانده شده ذخیره کنید
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "ابزارهای قدرتمند ما را کشف کنید"
    exclude: "document"
    description: "ویژگی‌هایی را که GroupDocs.Assembly برای ویرایش و ادغام اسناد با دقت ارائه می‌دهد، کاوش کنید."
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
    title: "اسناد را در فرمت‌های مختلف ادغام کنید"
    exclude: "DOCX"
    description: "با API .NET، می‌توانید اسناد را در بیش از 50 فرمت پشتیبانی شده ترکیب کنید. به‌راحتی فایل‌ها یا بخش‌ها را به سند نهایی خود بیفزایید."
    items: 
          
        # format loop 1
        - name: "گنجاندن یک سند در PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "گنجاندن یک سند در DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "گنجاندن یک سند در PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "گنجاندن یک سند در XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---