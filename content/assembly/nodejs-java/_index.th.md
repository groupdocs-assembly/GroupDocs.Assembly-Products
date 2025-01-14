---
############################# Static ############################
layout: "landing"
date: 2025-01-14T15:37:19
draft: false

lang: th
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
  for: "สำหรับ"

actions:
  main: "{index-content-nodejs-java.actions_main}"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "การจัดทำใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ลองใช้ฟีเจอร์ของ GroupDocs.Assembly ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} วางจำหน่ายแล้ว"
  notes: "ดูสิ่งที่ใหม่"
  downloads: "ดาวน์โหลด"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "{index-content-nodejs-java.code_title}"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // เส้นทางไปยังเทมเพลตหลัก
    const template = "chart_template.docx";

    // เรียกข้อมูลผลิตภาพของผู้จัดการจากแหล่งข้อมูล
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // สร้างอินสแตนซ์ของ DataSourceInfo ด้วยข้อมูล
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // ตั้งค่าสีกราฟโดยใช้อีก DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // กรอกข้อมูลลงในเทมเพลตและบันทึกไว้ที่เอาต์พุต
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "ภาพรวม GroupDocs.Assembly"
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
  title: "ความเป็นอิสระของแพลตฟอร์ม"
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
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    {index-content-nodejs-java.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### รูปแบบ Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### รูปภาพ และรูปแบบอื่นๆ
        * **พกพาได้:** PDF
        * **รูปภาพ:** SVG, TIFF
        * **รูปแบบสำนักงานอื่นๆ:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### รูปแบบอื่นๆ
        * **เว็บ:** HTML, MHTML
        * **อีเมล:** EML, MSG, EMLX
        * **อื่นๆ:** EPUB, MD

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
  title: "ตัวอย่างโค้ด"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
        ```javascript {style=abap}
        // แทรกเทมเพลตนี้บนหน้าของเอกสาร:
        // ตัวชี้วัดประสิทธิภาพของผู้จัดการ
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // ระบุเส้นทางเทมเพลต
        const template = "Bulleted List Template.docx";

        // ตั้งค่าเส้นทางไฟล์ผลลัพธ์
        const result = "Result Report.docx"

        // เรียกข้อมูลของผู้จัดการจากแหล่งข้อมูล JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // สร้างรายงานที่กรอกข้อมูล
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
        ```javascript {style=abap} 
        // เพิ่มเทมเพลตชื่อกราฟไปยังงานนำเสนอ:
        // รายได้จากลูกค้า <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // รวมเทมเพลตข้อมูลกราฟด้วย:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // ระบุเส้นทางเทมเพลตกราฟ
        const template = "Pie Chart Template.pptx";

        // ตั้งค่าเส้นทางไฟล์ผลลัพธ์
        const result = "Result Report.pptx"

        // เรียกข้อมูลของลูกค้าจากแหล่งข้อมูล XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // สร้างกราฟและบันทึกผลลัพธ์
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---