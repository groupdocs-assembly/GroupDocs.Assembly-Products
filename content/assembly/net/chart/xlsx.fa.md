



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: fa
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ایجاد نمودارها در فایل‌های XLSX با C#"
head_description: "API GroupDocs.Assembly for .NET این امکان را برای توسعه‌دهندگان فراهم می‌کند که به‌طور پویا نمودارها یا گراف‌ها را با استفاده از داده‌های آنی در مستندات تولید و وارد کنند."

############################# Header ############################
title: "ادغام نمودارها در فایل‌های XLSX با API .NET" 
description: "GroupDocs.Assembly for .NET یک روش قدرتمند برای پر کردن فایل‌های XLSX با داده‌های پویا و ادغام نمودارها به‌راحتی فراهم می‌آورد."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آزمایش رایگان"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET چیست؟"
    link: "/assembly/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ابزاری است که برای تسهیل ایجاد مستندات و گزارش‌ها از طریق ادغام داده‌ها از منابع مختلف طراحی شده است. به‌صورت پویا نمودارها، جداول، لیست‌ها، بارکدها و تصاویر را تولید کنید. گزینه‌های قالب‌بندی پیشرفته امکان قرارگیری و سفارشی‌سازی دقیق محتوای شما را فراهم می‌کند. این ابزار از بیش از ۵۰ فرمت فایل، از جمله PDF، مستندات MS Office و ایمیل‌ها پشتیبانی می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک نمودار به مستند XLSX اضافه کنیم"
    content: |
      [GroupDocs.Assembly](/assembly/net/) فرآیند تولید و ادغام نمودارها را به مستندات XLSX شما ساده می‌کند. از انواع مختلف نمودارها مانند نمودارهای میله‌ای، دایره‌ای و خطی پشتیبانی می‌کند.
      
      1. یک الگوی XLSX طراحی کنید که مکان‌هایی برای نمودارها داشته باشد.
      2. داده‌های خود را از یک منبع سازگار بازیابی کنید.
      3. گزینه‌های نمودار مانند نوع، برچسب‌ها و رنگ‌بندی را مشخص کنید.
      4. فایل به‌روز شده را با نمودار ادغام شده ذخیره کنید.
   
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
        // این تگ را در الگوی خود قرار دهید تا یک نمودار ایجاد کنید
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // مسیر فایل الگوی خود را مشخص کنید
        string template = "chart_template.xlsx";

        // داده‌ها را از منبع مورد نظر خود بارگذاری کنید
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // مستند را با نمودار ادغام شده ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "به سادگی نمودارهای پویا را به مستندات خود اضافه کنید"
  description: "GroupDocs.Assembly for .NET فرآیند خلق مستندات مبتنی بر داده را در فرمت‌های پرکاربرد ساده می‌کند. از الگوها برای وارد کردن نمودارها، جداول، بارکدها، لیست‌ها، هایپرلینک‌ها و تصاویر با ادغام داده‌های پیشرفته و پویا استفاده کنید."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "تبدیل داده‌ها به نمودارهای حرفه‌ای"
      content: "داده‌ها را از JSON، XML، CSV و منابع دیگر به نمودارهای بصری جذاب با چند مرحله ساده تبدیل کنید."

    # feature loop
    - title: "ایجاد محتوای بصری جذاب"
      content: "GroupDocs.Assembly از انواع مختلف نمودارها مانند نمودارهای میله‌ای، دایره‌ای و خطی پشتیبانی می‌کند. این‌ها را با جداول، بارکدها، تصاویر و عناصر دیگر ترکیب کنید تا گزارش‌های حرفه‌ای ایجاد کنید."

    # feature loop
    - title: "قرارگیری و سفارشی‌سازی دقیق نمودارها"
      content: "با استفاده از نحوی LINQ، می‌توانید نمودارها را به‌طور پویا تولید و دقیقاً در مکان‌های مورد نیاز قرار دهید. به‌راحتی سبک‌ها، رنگ‌ها و طرح‌بندی را به‌منظور تطابق با نیازهای خود سفارشی کنید."

    # feature loop
    - title: "کار با انواع فرمت‌های فایل"
      content: "مستندات را در فرمت‌های محبوب مانند MS Office، PDF، OpenOffice و HTML تولید کنید. نمودارها را بدون مشکل در هر فرمت پشتیبانی شده به‌طور کامل ادغام کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ایجاد یک نمودار به‌صورت برنامه‌نویسی"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید به‌صورت پویا یک نمودار را ایجاد و آن را در یک مستند XLSX ادغام کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // یک الگو با یک مکان‌نما برای نمودار آماده کنید
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // مسیر فایل الگو را ارائه دهید
          string template = "table_template.xlsx";

          // داده‌ها را از منبع خود بازیابی کنید
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // یک شی داده با اطلاعات موردنیاز بسازید
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // ویژگی‌های نمودار مانند نوع و ظاهر را تنظیم کنید
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // هسته DocumentAssembler را راه‌اندازی کنید
          DocumentAssembler asm = new DocumentAssembler();

          // مستند را با نمودار شامل شده صادر کنید
          asm.AssembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    exclude: "chart"
    description: "پلتفرم ما به شما کمک می‌کند تا مستندات جذاب و مبتنی بر داده را بر اساس نیازهای خود ایجاد کنید."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ایجاد گزارش‌های بصری غنی در چندین فرمت"
    exclude: "XLSX"
    description: ".NET به شما این امکان را می‌دهد که مستندات با نمودارهای ادغام شده را در بیش از ۵۰ فرمت پشتیبانی شده تولید کنید و الگوها را به‌طور یکپارچه با داده‌های خود ترکیب کنید."
    items: 
          
        # format loop 1
        - name: "نمودارها در PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "نمودارها در DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "نمودارها در PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "نمودارها در XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---