---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: fa
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

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
head_title: "API .NET برای اتوماسیون مستندات، تجمیع و تولید گزارش"
head_description: "API C# .NET برای اتوماسیون مستندات، تجمیع و تولید گزارش. ایجاد PDF، Word، Excel، PPTX، HTML و مستندات ایمیلی از الگوهای سفارشی."

############################# Header ############################
title: "API اتوماسیون مستندات و گزارش‌دهی .NET"
description: "گزارش‌ها را در برنامه‌های .NET با تعریف الگوها و ادغام داده‌ها تولید کنید."
words:
  for: "برای"

actions:
  main: "دانلود آزمایشی از طریق NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "مجوزدهی"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Assembly را به‌صورت رایگان امتحان کنید یا درخواست مجوز دهید."

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیزی جدید است"
  downloads: "دانلودها"

code:
  title: "پر کردن یک نمودار در DOCX با C#"
  more: "نمونه‌های بیشتر"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // مسیر به الگوی اصلی
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نگاهی به GroupDocs.Assembly"
  description: "راه حل .NET برای اتوماسیون ایجاد مستندات با یکپارچگی داده پیشرفته."
  features:
    # feature loop
    - title: "افزودن داده‌های تجاری به الگوهای مستندات با C#"
      content: "تولید گزارش به‌طور آسان: با GroupDocs.Assembly for .NET می‌توانید به راحتی داده‌ها را از منابعی مانند JSON یا XML به الگوهای از پیش تعریف شده وارد کنید."

    # feature loop
    - title: "پردازش اشیاء داده بومی"
      content: "فرمت‌های مستند پشتیبانی شده شامل اشیاء تعبیه شده‌ای همچون نمودارها، جداول و لیست‌ها هستند که می‌توانند به‌طور خودکار با داده‌ها پر شوند."

    # feature loop
    - title: "ویژگی‌های اضافی"
      content: "GroupDocs.Assembly for .NET گزینه‌های سفارشی‌سازی وسیعی را فراهم می‌کند. اشیاء داده را به‌صورت برنامه‌نویسی طراحی کنید، بارکدها را تولید کنید، از منابع داده آنلاین از طریق URL استفاده کنید و خروجی را در فرمت‌های مختلف ذخیره کنید."

############################# Platforms ############################
platforms:
  enable: true
  title: "عدم وابستگی به پلتفرم"
  description: "GroupDocs.Assembly for .NET با سیستم‌عامل‌ها، فریم‌ورک‌ها و مدیران بسته‌های زیر سازگار است."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت‌های پشتیبانی شده"
  description: |
    GroupDocs.Assembly for .NET می‌تواند فرمت‌های زیر را پردازش کند [فرمت‌های مستند](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "ویژگی‌های GroupDocs.Assembly"
  description: "ایجاد مستندات و گزارش‌ها با استفاده از مدل‌های داده پیشرفته."

  items:
    # feature loop
    - icon: "preview"
      title: "نمایش داده پیشرفته"
      content: "پشتیبانی از دامنه وسیعی از اشیاء داده مانند نمودارها، لیست‌ها، جداول، تصاویر و غیره."

    # feature loop
    - icon: "manipulate"
      title: "دستکاری داده"
      content: "فرمول‌ها و عملیات خودکار را برای فرمت و نمایش مؤثر داده‌ها اعمال کنید."

    # feature loop
    - icon: "two_pages"
      title: "دامنه وسیعی از فرمت‌های پشتیبانی شده"
      content: "بدون مشکل با تمامی فرمت‌های معمول مستندات برای الگوها یا فایل‌های خروجی کار کنید."

    # feature loop
    - icon: "document_settings"
      title: "نشانه‌گذاری غنی در الگوها"
      content: "در الگوها از فرمت‌بندی عددی، الفبایی و سازمانی سود ببرید."

    # feature loop
    - icon: "text"
      title: "اضافه کردن بارکدها"
      content: "تصاویر بارکد را به‌صورت دینامیکی ایجاد کرده و آن‌ها را در مستندات خود وارد کنید."

    # feature loop
    - icon: "add"
      title: "فرمت‌بندی داده"
      content: "رشته‌ها را در الگوها به‌صورت بزرگ، کوچک، با حرف بزرگ اول یا به سبک‌های دیگر فرمت کنید."

    # feature loop
    - icon: "manipulate"
      title: "دستکاری محتوای مستند"
      content: "به‌طور دینامیکی محتوا را از مستندات خارجی در گزارش‌های خود وارد کنید."

    # feature loop
    - icon: "convert"
      title: "ذخیره‌سازی در چندین فرمت"
      content: "فرمت فایل خروجی را با استفاده از پسوندهای فایل یا تنظیمات دقیق مشخص کنید."

    # feature loop
    - icon: "update"
      title: "پردازش داده انعطاف‌پذیر"
      content: "تصاویر و مستندات را به‌طور دینامیکی با استفاده از بایت‌های کدگذاری‌شده با Base64 وارد کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "نمونه‌های کد برای عملیات رایج GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "لیست شماره‌گذاری شده در یک سند Microsoft Word"
      content: |
        [لیست‌های شماره گذاری شده](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) یک روش معمول برای ارائه داده‌های تجاری هستند. این یک نمونه از افزودن یک لیست به مستند Word با استفاده از GroupDocs.Assembly است.
        {{< landing/code title="چگونه یک لیست را در مستندات پر کنیم">}}
        ```csharp {style=abap}
        // این الگو را در یک صفحه مستند وارد کنید:
        // شاخص‌های عملکرد مدیران
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // مسیر الگو را مشخص کنید
        string template = "Bulleted List Template.docx";

        // مسیر فایل خروجی را تنظیم کنید
        string result = "Result Report.docx"

        // داده‌های مدیران را از یک منبع JSON بازیابی کنید
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // گزارش را با داده‌های پر شده تولید کنید
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "نمودارهای دایره‌ای در ارائه PPTX"
      content: |
        شما می‌توانید [نمودارهای دایره‌ای](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) را با استفاده از الگوها و داده‌های XML ایجاد کنید. گزارش‌های خود را با نمایش‌های بصری جذاب بهبود دهید.
        {{< landing/code title="چگونه داده‌ها را در یک نمودار دایره‌ای نمایش دهیم">}}
        ```csharp {style=abap}
        // الگوی عنوان نمودار را به ارائه اضافه کنید:
        // درآمد مشتریان <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // همچنین الگوی داده‌های نمودار را شامل کنید:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // مسیر الگوی نمودار را مشخص کنید
        string template = "Pie Chart Template.pptx";

        // مسیر فایل خروجی را تنظیم کنید
        string result = "Result Report.pptx"

        // داده‌های مشتریان را از یک منبع XML بازیابی کنید
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // نمودار را تولید کرده و نتیجه را ذخیره کنید
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---