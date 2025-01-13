---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
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
head_title: "{index-content-nodejs-java.head_title}"
head_description: "{index-content-nodejs-java.head_description}"

############################# Header ############################
title: "{index-content-nodejs-java.title}"
description: "{index-content-nodejs-java.description}"
words:
  for: "برای"

actions:
  main: "{index-content-nodejs-java.actions_main}"
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
  title: "{index-content-nodejs-java.code_title}"
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
  description: "{index-content-nodejs-java.overview_description}"
  features:
    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_1.title}"
      content: "{index-content-nodejs-java.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_2.title}"
      content: "{index-content-nodejs-java.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_3.title}"
      content: "{index-content-nodejs-java.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "عدم وابستگی به پلتفرم"
  description: "{index-content-nodejs-java.platforms_description}"
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
    {index-content-nodejs-java.formats_description}
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
  title: "{index-content-nodejs-java.features.title}"
  description: "{index-content-nodejs-java.features.description}"

  items:
    # feature loop
    - icon: "preview"
      title: "{index-content-nodejs-java.features.feature_1.title}"
      content: "{index-content-nodejs-java.features.feature_1.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_2.title}"
      content: "{index-content-nodejs-java.features.feature_2.content}"

    # feature loop
    - icon: "two_pages"
      title: "{index-content-nodejs-java.features.feature_3.title}"
      content: "{index-content-nodejs-java.features.feature_3.content}"

    # feature loop
    - icon: "document_settings"
      title: "{index-content-nodejs-java.features.feature_4.title}"
      content: "{index-content-nodejs-java.features.feature_4.content}"

    # feature loop
    - icon: "text"
      title: "{index-content-nodejs-java.features.feature_5.title}"
      content: "{index-content-nodejs-java.features.feature_5.content}"

    # feature loop
    - icon: "add"
      title: "{index-content-nodejs-java.features.feature_6.title}"
      content: "{index-content-nodejs-java.features.feature_6.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_7.title}"
      content: "{index-content-nodejs-java.features.feature_7.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-nodejs-java.features.feature_8.title}"
      content: "{index-content-nodejs-java.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-nodejs-java.features.feature_9.title}"
      content: "{index-content-nodejs-java.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
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
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
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