



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:07
draft: false
lang: fa
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "یک سند را در XLSX با استفاده از Java وارد کنید"
head_description: "فایل‌های XLSX را به راحتی با Java ترکیب کنید. GroupDocs.Assembly فرآیند ادغام اسناد را تنها با چند خط کد ساده می‌کند."

############################# Header ############################
title: "به راحتی محتوای خود را در فایل‌های XLSX جاسازی کنید" 
description: "از GroupDocs.Assembly for Java برای ادغام بدون دردسر یک سند XLSX به سند دیگر استفاده کنید. با ابزارهای قابل اعتماد و انعطاف‌پذیر نتایج دقیق‌تری به دست آورید."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "به صورت رایگان دریافت کن"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java چیست؟"
    link: "/assembly/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) راه‌حلی چندمنظوره برای مدیریت اسناد است. این امکان را به شما می‌دهد تا به راحتی یک سند را به سند دیگر ادغام کنید و از بیش از ۵۰ فرمت، از جمله PDF و فایل‌های MS Office پشتیبانی کند. خروجی خود را با ترکیب، ویرایش و سازماندهی محتوا به دقیقا همان شکلی که می‌خواهید، شخصی‌سازی کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل وارد کردن یک سند به یک فایل XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) جاسازی یک سند XLSX به سند دیگر را ساده و قابل تنظیم می‌کند.
      
      1. یک الگوی XLSX با مکان‌نگاشت‌هایی برای محتوای جاسازی شده آماده کنید.
      2. مسیر فایل برای الگو را مشخص کنید.
      3. مسیر فایل سندی که می‌خواهید جاسازی کنید را ارائه دهید.
      4. فایل خروجی را با محتوای ادغام شده ذخیره کنید.
   
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
        // از این تگ در الگوی خود برای علامت‌گذاری محل سند جاسازی شده استفاده کنید
        // <<doc [doc_expression]>>

        // مسیر فایل برای الگوی اصلی را تنظیم کنید
        String template = "doc_template.xlsx";

        // مسیر سندی که می‌خواهید وارد کنید را ارائه دهید
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // فایل نهایی را با محتوای جاسازی شده ذخیره کنید
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ابزارهای پیشرفته برای ساده‌سازی ادغام اسناد"
  description: "با GroupDocs.Assembly for Java، جاسازی اسناد ساده و قابل تنظیم است، بدون در نظر گرفتن نوع فایل. در پروژه‌های خود نتایج مرتب و یکنواختی را به دست آورید."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "نکات برجسته GroupDocs.Assembly"
  features:
    # feature loop
    - title: "ایجاد گزارش با استفاده از داده‌های تجاری"
      content: "مستندات را به سرعت و به طور قابل اعتماد با داده‌هایی از منابعی مانند JSON، XML یا CSV پر کنید و جریان‌های کاری خود را بهینه‌سازی کنید."

    # feature loop
    - title: "تقویت اسناد با محتوای بصری"
      content: "GroupDocs.Assembly به شما این امکان را می‌دهد که جداول، نمودارها و لیست‌ها را در کنار متن، پیوندهای هایپر، تصاویر و حتی بارکدهای پویا وارد کنید."

    # feature loop
    - title: "قرار دادن داده‌ها در مکان مناسب"
      content: "الگوهای LINQ کمک می‌کنند تا داده‌های خود را با دقت قرار دهید، عناصر تکراری مانند آرایه‌ها را مدیریت کرده و به راحتی استایل‌های سفارشی را اعمال کنید."

    # feature loop
    - title: "سازگاری با انواع مختلف فایل‌ها"
      content: "اسناد را در میان فرمت‌های مختلف، از جمله PDF، HTML، فایل‌های MS Office و OpenOffice ادغام کنید و از انعطاف‌پذیری برای پروژه‌های خود اطمینان حاصل کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه به طور برنامه‌نویسی یک تصویر را به یک سند وارد کنیم"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان یک تصویر را به یک فایل XLSX با استفاده از GroupDocs.Assembly جاسازی کرد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک تگ مکان‌نگاشت در فایل الگو اضافه کنید
          // <<image [expression]>>

          // مسیر الگو را تعریف کنید
          String template = "template.xlsx";

          // مسیر تصویر را مشخص کنید
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // نمونه DocumentAssembler را مقداردهی اولیه کنید
          DocumentAssembler asm = new DocumentAssembler();

          // فایل را با تصویر جاسازی شده ذخیره کنید
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "قابلیت‌های کلیدی در یک نگاه"
    exclude: "document"
    description: "ویژگی‌های گسترده‌ای که GroupDocs.Assembly برای ساده‌سازی و بهینه‌سازی ادغام و ترکیب اسناد ارائه می‌دهد را کشف کنید."
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
    title: "ادغام در انواع مختلف اسناد"
    exclude: "XLSX"
    description: "با Java، می‌توانید محتوا را در میان بیش از ۵۰ فرمت فایل جاسازی و ترکیب کنید. فایل‌ها را به صورت روان اضافه کنید تا نتایج حرفه‌ای ایجاد کنید."
    items: 
          
        # format loop 1
        - name: "گنجاندن یک سند در PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 2
        - name: "گنجاندن یک سند در DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "سند Open XML مایکروسافت ورد"
          
        # format loop 3
        - name: "گنجاندن یک سند در PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "ارائه Open XML پاورپوینت"
          
        # format loop 4
        - name: "گنجاندن یک سند در XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "صفحه‌گسترده Open XML مایکروسافت اکسل"


          

---