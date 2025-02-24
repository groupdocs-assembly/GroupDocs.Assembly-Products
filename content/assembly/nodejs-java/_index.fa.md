---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: fa
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "ابزار Node.js برای ساخت، اتوماسیون و سفارشی‌سازی اسناد"
head_description: "کتابخانه Node.js برای اتوماسیون گردش کار اسنادی. ایجاد فایل‌های PDF، ورد، اکسل، پاورپوینت، HTML و ایمیل از قالب‌های خود."

############################# Header ############################
title: "API Node.js برای اتوماسیون ساده اسناد و گزارش‌ها"
description: "تولید گزارش‌های JavaScript را با ترکیب داده‌های خود با قالب‌های از پیش ساخته شده تسهیل کنید."
words:
  for: "برای"

actions:
  main: "آزمایش خود را در NPM آغاز کنید"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "مجوزدهی"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Assembly را به‌صورت رایگان امتحان کنید یا درخواست مجوز دهید."

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیزی جدید است"
  downloads: "دانلودها"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "ایجاد نمودار در یک سند ورد با استفاده از Node.js"
  more: "نمونه‌های بیشتر"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // مسیر به الگوی اصلی
    const template = "chart_template.docx";

    // داده‌های تولید بازدهی مدیران را از منبع بازیابی کنید
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // یک نمونه از DataSourceInfo با داده‌ها ایجاد کنید
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // رنگ‌های نمودار را با استفاده از DataSourceInfo دیگر تنظیم کنید
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // الگو را با داده‌ها پر کنید و آن را در خروجی ذخیره کنید
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نگاهی به GroupDocs.Assembly"
  description: "کتابخانه Node.js برای ایجاد اسناد به صورت برنامه‌نویسی با مدیریت داده‌های یکپارچه ساخته شده است."
  features:
    # feature loop
    - title: "ترکیب داده‌های کسب‌وکار با قالب‌ها با JavaScript"
      content: "گزارش‌های حرفه‌ای با گنجاندن داده‌های JSON، XML یا سایر داده‌ها در قالب‌ها با کمک GroupDocs.Assembly for Node.js via Java تولید کنید."

    # feature loop
    - title: "مدیریت محتوای گنجانده شده"
      content: "به‌طور خودکار جداول، نمودارها و سایر عناصر بصری را در اسناد خود با استفاده از داده‌های خارجی پر کنید."

    # feature loop
    - title: "گزینه‌های سفارشی‌سازی"
      content: "GroupDocs.Assembly for Node.js via Java به شما این امکان را می‌دهد که ویژگی‌هایی مانند بارکدها را اضافه کنید، داده‌ها را از URLها استخراج کنید و فایل‌ها را در فرمت‌های مختلف صادر کنید."

############################# Platforms ############################
platforms:
  enable: true
  title: "عدم وابستگی به پلتفرم"
  description: "GroupDocs.Assembly for Node.js via Java به‌طور روان با سیستم‌عامل‌ها، چارچوب‌ها و مدیران بسته‌ی پیشرو ادغام می‌شود."
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
    GroupDocs.Assembly for Node.js via Java از مجموعه‌ی وسیعی از [فرمت‌های اسناد](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/) پشتیبانی می‌کند.
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
  title: "ویژگی‌های اصلی GroupDocs.Assembly"
  description: "ایجاد اسناد و گزارش‌های پویا با ابزارهای مدیریت داده قدرتمند."

  items:
    # feature loop
    - icon: "preview"
      title: "نمایش‌های غنی داده"
      content: "به سادگی نمودارها، جداول، تصاویر و لیست‌ها را با سفارشی‌سازی کامل به اسناد خود اضافه کنید."

    # feature loop
    - icon: "manipulate"
      title: "تبدیل داده‌های شما"
      content: "از ابزارهایی مانند فرمول‌ها و مرتب‌سازی برای ساختاردهی و نمایش مؤثر اطلاعات استفاده کنید."

    # feature loop
    - icon: "two_pages"
      title: "سازگاری با فرمت‌های وسیع"
      content: "به‌طور همزمان با فرمت‌های رایج فایل برای قالب‌ها و خروجی‌ها کار کنید."

    # feature loop
    - icon: "document_settings"
      title: "سفارشی‌سازی پیشرفته قالب‌ها"
      content: "قالب‌ها را با گزینه‌های فرمت‌دهی عددی، الفبایی و سایر گزینه‌های استایل فرمت کنید."

    # feature loop
    - icon: "text"
      title: "ایجاد بارکدها به‌طور پویا"
      content: "تصاویر بارکد را به‌طور مستقیم و طبق درخواست در اسناد خود ایجاد و درج کنید."

    # feature loop
    - icon: "add"
      title: "استایل متن انعطاف‌پذیر"
      content: "به سادگی استایل‌های متنی مانند حروف بزرگ یا عنوان را در قالب‌های خود اعمال کنید."

    # feature loop
    - icon: "manipulate"
      title: "درج محتوای پویا"
      content: "در حین تولید اسناد، به‌طور پویا محتوای فایل‌های خارجی را شامل کنید."

    # feature loop
    - icon: "convert"
      title: "صادرات به فرمت‌های مختلف"
      content: "اسناد را با پیکربندی‌های مشخص شده خود در چندین فرمت ذخیره کنید."

    # feature loop
    - icon: "update"
      title: "گنجاندن رسانه به‌طور پویا"
      content: "در زمان ایجاد اسناد، تصاویر یا عناصر دیگر را با استفاده از داده‌های Base64 درج کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "نمونه‌های عملی از نحوه استفاده از GroupDocs.Assembly برای وظایف رایج را کشف کنید."
  items:
    # code sample loop
    - title: "اضافه کردن یک لیست گلوله‌ای در اسناد ورد"
      content: |
        چگونگی ایجاد [لیست‌های گلوله‌ای](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) در اسناد ورد برای سازماندهی مؤثر داده‌ها را ببینید. این مثال نحوه تولید یک لیست گلوله‌ای با استفاده از GroupDocs.Assembly را نشان می‌دهد.
        {{< landing/code title="اضافه کردن یک لیست گلوله‌ای در اسناد ورد">}}
        ```javascript {style=abap}
        // این الگو را در یک صفحه مستند وارد کنید:
        // شاخص‌های عملکرد مدیران
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر الگو را مشخص کنید
        const template = "Bulleted List Template.docx";

        // مسیر فایل خروجی را تنظیم کنید
        const result = "Result Report.docx"

        // داده‌های مدیران را از یک منبع JSON بازیابی کنید
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // گزارش را با داده‌های پر شده تولید کنید
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "درج نمودارهای دایره‌ای در پاورپوینت"
      content: |
        یاد بگیرید چگونه از قالب‌ها و XML برای افزودن [نمودارهای دایره‌ای](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) در ارائه‌های خود استفاده کنید. گزارش‌های خود را با نمودارهای دایره‌ای برای ارائه بصری و شفاف داده‌ها تقویت کنید.
        {{< landing/code title="درج نمودارهای دایره‌ای در پاورپوینت">}}
        ```javascript {style=abap} 
        // الگوی عنوان نمودار را به ارائه اضافه کنید:
        // درآمد مشتریان <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // همچنین الگوی داده‌های نمودار را شامل کنید:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // مسیر الگوی نمودار را مشخص کنید
        const template = "Pie Chart Template.pptx";

        // مسیر فایل خروجی را تنظیم کنید
        const result = "Result Report.pptx"

        // داده‌های مشتریان را از یک منبع XML بازیابی کنید
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // نمودار را تولید کرده و نتیجه را ذخیره کنید
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---