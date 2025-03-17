---
############################# Static ############################
layout: "landing"
date: 2025-03-17T13:11:11
draft: false

lang: fa
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "کتابخانه Java برای ایجاد، اتوماسیون و گزارش‌دهی مستندات"
head_description: "کتابخانه Java برای اتوماسیون ایجاد مستندات و تولید گزارش. ایجاد PDF، Word، Excel، PPTX، HTML و مستندات ایمیلی با استفاده از الگوهای سفارشی."

############################# Header ############################
title: "API Java برای اتوماسیون گزارش‌ها و مستندات"
description: "تولید گزارش‌ها در Java با ادغام داده‌ها با الگوها را ساده کنید."
words:
  for: "برای"

actions:
  main: "دریافت آزمایشی از طریق Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "مجوزدهی"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Assembly را به‌صورت رایگان امتحان کنید یا درخواست مجوز دهید."

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیزی جدید است"
  downloads: "دانلودها"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "ایجاد نموداری در DOCX با Java"
  more: "نمونه‌های بیشتر"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // مسیر به الگوی اصلی
    String template = "chart_template.docx";

    // داده‌های تولید بازدهی مدیران را از منبع بازیابی کنید
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // یک نمونه از DataSourceInfo با داده‌ها ایجاد کنید
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // رنگ‌های نمودار را با استفاده از DataSourceInfo دیگر تنظیم کنید
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // الگو را با داده‌ها پر کنید و آن را در خروجی ذخیره کنید
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نگاهی به GroupDocs.Assembly"
  description: "کتابخانه Java طراحی‌شده برای ایجاد اتوماتیک مستندات و یکپارچگی داده بدون مشکل."
  features:
    # feature loop
    - title: "ادغام داده‌های تجاری در الگوها با Java"
      content: "به سادگی گزارش‌های حرفه‌ای با وارد کردن داده‌ها از JSON، XML یا منابع دیگر به الگوهای از پیش طراحی شده با استفاده از GroupDocs.Assembly for Java ایجاد کنید."

    # feature loop
    - title: "کار با اشیاء تعبیه‌شده"
      content: "به‌طور خودکار عناصر مانند جداول، نمودارها و دیاگرام‌ها را با استفاده از داده‌ها از منابع خارجی پر کنید."

    # feature loop
    - title: "سفارشی‌سازی پیشرفته"
      content: "GroupDocs.Assembly for Java امکانات انعطاف‌پذیری را مانند تولید بارکد، کشیدن داده‌های آنلاین از طریق URL و صادرات خروجی در فرمت‌های مختلف ارائه می‌دهد."

############################# Platforms ############################
platforms:
  enable: true
  title: "عدم وابستگی به پلتفرم"
  description: "GroupDocs.Assembly for Java به‌صورت بی‌دردسر با سیستم‌عامل‌ها، فریم‌ورک‌های توسعه و مدیران بسته‌های محبوب کار می‌کند."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت‌های پشتیبانی شده"
  description: |
    GroupDocs.Assembly for Java از یک دامنه وسیع [فرمت‌های مستند](https://docs.groupdocs.com/assembly/java/supported-document-formats/) پشتیبانی می‌کند.
  groups:
    # group loop
    - color: "green"
      content: |
        ### فرمت‌های Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### تصاویر و سایر فرمت‌ها
        * **قابل حمل:** PDF
        * **تصاویر:** SVG, TIFF
        * **سایر فرمت‌های اداری:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### سایر فرمت‌ها
        * **وب:** HTML, MHTML
        * **ایمیل‌ها:** EML, MSG, EMLX
        * **سایر:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "قابلیت‌های کلیدی GroupDocs.Assembly"
  description: "ایجاد مستندات و گزارش‌های حرفه‌ای با مدیریت داده پیشرفته."

  items:
    # feature loop
    - icon: "preview"
      title: "عناصر داده بصری"
      content: "عناصر مانند نمودارها، جداول، تصاویر و لیست‌ها را به‌طور مستقیم در مستندات خود اضافه و فرمت کنید."

    # feature loop
    - icon: "manipulate"
      title: "تبدیل داده"
      content: "از فرمول‌ها، مرتب‌سازی و ابزارهای دیگر برای سازماندهی و ارائه مؤثر داده‌های خود استفاده کنید."

    # feature loop
    - icon: "two_pages"
      title: "پشتیبانی از فرمت‌های متعدد"
      content: "با سهولت کار با انواع فایل‌های معمول برای الگوها و فایل‌های خروجی."

    # feature loop
    - icon: "document_settings"
      title: "فرمت‌بندی الگوهای پیشرفته"
      content: "الگوها را با گزینه‌های تنظیم درست عددی، الفبایی و دیگر فرمت‌های پیشرفته سفارشی کنید."

    # feature loop
    - icon: "text"
      title: "تولید دینامیک بارکد"
      content: "به سرعت بارکدها را تولید کرده و در مستندات به آن‌ها اضافه کنید."

    # feature loop
    - icon: "add"
      title: "استایل بندی متنی انعطاف‌پذیر"
      content: "تبدیلات متنی از جمله حالت بزرگ، حالت کوچک، حالت عنوان یا سبک‌های دیگر را در الگوها اعمال کنید."

    # feature loop
    - icon: "manipulate"
      title: "وارد کردن محتوای خارجی"
      content: "به‌طور دینامیک محتوا را از فایل‌های خارجی هنگام ایجاد مستندات وارد کنید."

    # feature loop
    - icon: "convert"
      title: "صادرات در فرمت‌های مختلف"
      content: "مستندات نهایی را با استفاده از پسوندها یا تنظیمات مشخص شده در فرمت‌های مختلف ذخیره کنید."

    # feature loop
    - icon: "update"
      title: "مدیاهای دینامیک"
      content: "تصاویر یا محتوای دیگر را با استفاده از داده‌های کدگذاری شده با Base64 هنگام ایجاد مستندات وارد کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "نمونه کد برای وظایف رایج با GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "ایجاد یک لیست شماره‌گذاری شده در Word"
      content: |
        یاد بگیرید چگونه [لیست‌های شماره‌گذاری شده](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) را به مستندات Word برای نمایندگی سازمان یافته داده اضافه کنید. این مثال نشان می‌دهد چگونه با استفاده از GroupDocs.Assembly یک لیست در Word تولید کنید.
        {{< landing/code title="ایجاد یک لیست شماره‌گذاری شده در Word">}}
        ```java {style=abap}
        // این الگو را در یک صفحه مستند وارد کنید:
        // شاخص‌های عملکرد مدیران
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // مسیر الگو را مشخص کنید
        String template = "Bulleted List Template.docx";

        // مسیر فایل خروجی را تنظیم کنید
        String result = "Result Report.docx"

        // داده‌های مدیران را از یک منبع JSON بازیابی کنید
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // گزارش را با داده‌های پر شده تولید کنید
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ایجاد نمودارهای دایره‌ای در PPTX"
      content: |
        از الگوها و XML برای افزودن [نمودارهای دایره‌ای](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) به ارائه‌های خود استفاده کنید. گزارش‌های خود را با گنجاندن نمودارهای دایره‌ای برای تجسم داده‌ها بیشتر جذاب کنید.
        {{< landing/code title="ایجاد نمودارهای دایره‌ای در PPTX">}}
        ```java {style=abap}   
        // الگوی عنوان نمودار را به ارائه اضافه کنید:
        // درآمد مشتریان <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // همچنین الگوی داده‌های نمودار را شامل کنید:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // مسیر الگوی نمودار را مشخص کنید
        String template = "Pie Chart Template.pptx";

        // مسیر فایل خروجی را تنظیم کنید
        String result = "Result Report.pptx"

        // داده‌های مشتریان را از یک منبع XML بازیابی کنید
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // نمودار را تولید کرده و نتیجه را ذخیره کنید
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---