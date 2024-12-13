



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: fa
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ایجاد لیست‌ها در اسناد XLSX با استفاده از Java"
head_description: "طراحی و گنجاندن لیست‌های پویا را به راحتی در قالب‌های XLSX با API GroupDocs.Assembly for Java انجام دهید."

############################# Header ############################
title: "لیست‌های پویا را به فایل‌های XLSX با API Java ما اضافه کنید" 
description: "GroupDocs.Assembly for Java ابزارهای انعطاف‌پذیری برای تولید و درج لیست‌های پرمحتوا به طور مستقیم در اسناد XLSX ارائه می‌دهد."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "همین حالا امتحان کنید"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "چیست GroupDocs.Assembly for Java؟"
    link: "/assembly/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) امکان طراحی اسناد حرفه‌ای را با کشیدن داده‌ها از منابع مختلف فراهم می‌کند. از آن برای ایجاد لیست‌ها، جداول، نمودارها یا متون استفاده کنید و این عناصر را با استفاده از قابلیت‌های پیشرفته قالب در مکان‌های دقیق قرار دهید. با پشتیبانی از بیش از ۵۰ فرمت، از جمله PDF، فایل‌های MS Office و اسناد ایمیلی، به شما کمک می‌کند تا گردش کار خود را اتوماسیون و بهینه‌سازی کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک لیست مبتنی بر داده را به سند XLSX اضافه کنیم"
    content: |
      [GroupDocs.Assembly](/assembly/java/) به شما این امکان را می‌دهد تا به سرعت لیست‌های غنی از داده را به قالب‌های XLSX وارد کنید. محتوای خود را بدون زحمت سفارشی و سازماندهی کنید.
      
      1. یک قالب XLSX ایجاد کرده و مکان‌های نشانه‌گذاری برای لیست را مشخص کنید.
      2. مسیر فایل را به قالب تنظیم کنید.
      3. داده‌ها را از فرمت‌های پشتیبانی شده مانند JSON یا XML بکشید.
      4. سند نهایی را با لیست اضافه شده ذخیره کنید.
   
    code:
      platform: "java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "سند مثال"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // این برچسب را در قالب خود در جایی که لیست باید ظاهر شود قرار دهید
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // مسیر فایل قالب را تعریف کنید
        String template = "list_template.xlsx";

        // داده‌ها را از منبع انتخابی خود بکشید
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // سند را با لیست درج شده ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ایجاد اسناد از قالب‌ها با ادغامی داده"
  description: "GroupDocs.Assembly for Java افزودن لیست‌ها، جداول، نمودارها و سایر اجزا به قالب‌های سند را ساده می‌کند."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Assembly"
  features:
    # feature loop
    - title: "ایجاد گزارش‌ها با داده از منابع مختلف"
      content: "از داده‌های فرمت‌هایی مانند JSON، XML و CSV برای پر کردن لیست‌ها و سایر اجزا به طور مؤثر استفاده کنید."

    # feature loop
    - title: "اضافه کردن لیست‌ها و سایر عناصر داده به طور یکپارچه"
      content: "GroupDocs.Assembly امکان گنجاندن لیست‌ها، نمودارها، جداول و بیشتر، به همراه متن، تصاویر و لینک‌ها را برای ایجاد اسناد شیک فراهم می‌کند."

    # feature loop
    - title: "کنترل دقیق بر روی مکان نصب داده‌ها"
      content: "قالب‌های مبتنی بر LINQ به شما این امکان را می‌دهند که مکان‌های دقیقی برای لیست‌ها و داده‌های خود تعریف کنید. از حلقه‌ها برای ایجاد لیست‌های دقیق به طور خودکار و اعمال قالب‌بندی‌های سفارشی استفاده کنید."

    # feature loop
    - title: "پشتیبانی از فرمت‌های مختلف سند"
      content: "ایجاد یا ویرایش فایل‌ها در فرمت‌هایی مانند MS Office، PDF، OpenOffice، HTML و ایمیل. ادغام محتوا از چندین سند به میزان لازم."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک لیست را به صورت برنامه‌نویسی ایجاد کنید"
      content: |
        این مثال نشان می‌دهد که چگونه به صورت پویا یک لیست را به یک فایل XLSX با استفاده از GroupDocs.Assembly اضافه کنید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک برچسب جایگزین در قالب خود برای لیست اضافه کنید
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // مسیر فایل به قالب خود را فراهم کنید
          String template = "numlist_template.xlsx";

          // داده‌های لازم برای پر کردن لیست را بکشید
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // منبع داده را با جزئیات لازم آماده کنید
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // مقداردهی اولیه DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // سند خروجی را با لیست کامل ذخیره کنید
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "کپی"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.xlsx"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "آماده برای شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Assembly را رایگان آزمایش کنید یا درخواست مجوز نمایید"
  items:
    #  loop
    - title: "دانلود از Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "درباره مجوزدهی بیاموزید"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "کشف کنید که GroupDocs.Assembly چه کارهایی می‌تواند انجام دهد"
    exclude: "list"
    description: "به سادگی اسناد غنی از محتوا را با ابزارهای پیشرفته ادغام داده طراحی و تولید کنید."
    items: 
          
        # operation loop 1
        - name: "تولید بارکدها"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "بارکدهایی به صورت دینامیکی ایجاد و به اسناد اضافه کنید"

        # operation loop 2
        - name: "تصویرسازی داده‌ها با نمودارها"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "انواع مختلف نمودارها را با داده‌ها پر کنید"

        # operation loop 3
        - name: "ادغام اسناد"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "محتوای یک سند را به سند دیگر ترکیب کنید"

        # operation loop 4
        - name: "نمایش داده‌ها با لیست‌ها"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "با استفاده از داده‌های خاص، لیست‌ها را در اسناد تولید کنید"

        # operation loop 5
        - name: "سازماندهی داده‌ها در جداول"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "داده‌ها را از هر منبعی بازیابی کرده و جداول را پر کنید"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "تولید اسناد در فرمت‌های مختلف"
    exclude: "XLSX"
    description: "Java از بیش از ۵۰ فرمت پشتیبانی می‌کند، که به شما این امکان را می‌دهد تا با ترکیب داده‌ها و قالب‌ها اسناد ساختاری ایجاد کنید."
    items: 
          
        # format loop 1
        - name: "ایجاد یک لیست در PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "ایجاد یک لیست در DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "ایجاد یک لیست در PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "ایجاد یک لیست در XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---