---
############################# Static ############################
layout: "landing"
date: 2025-01-16T13:04:06
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
head_title: "เครื่องมือ Node.js สำหรับการสร้าง อัตโนมัติ และปรับแต่งเอกสาร"
head_description: "ไลบรารี Node.js สำหรับการทำงานอัตโนมัติของเอกสาร สร้างไฟล์ PDF, Word, Excel, PowerPoint, HTML, และอีเมลจากเทมเพลตของคุณ."

############################# Header ############################
title: "API Node.js สำหรับการจัดทำเอกสารและรายงานอย่างง่าย"
description: "ปรับปรุงการสร้างรายงานใน JavaScript โดยการรวมข้อมูลของคุณกับเทมเพลตที่สร้างไว้ล่วงหน้า."
words:
  for: "สำหรับ"

actions:
  main: "เริ่มทดลองใช้งานบน NPM"
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
  title: "สร้างแผนภูมิในเอกสาร Word โดยใช้ Node.js"
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
  description: "ไลบรารี Node.js ที่ออกแบบมาเพื่อสร้างเอกสารโปรแกรมmatically พร้อมการจัดการข้อมูลที่รวมไว้."
  features:
    # feature loop
    - title: "รวมข้อมูลธุรกิจเข้ากับเทมเพลตด้วย JavaScript"
      content: "สร้างรายงานที่ดูดีโดยการฝัง JSON, XML, หรือข้อมูลอื่น ๆ ในเทมเพลตด้วย GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "จัดการเนื้อหาที่ฝัง"
      content: "ทำให้ตาราง แผนภูมิ และวิชวลอื่น ๆ ในเอกสารของคุณถูกกรอกโดยอัตโนมัติด้วยข้อมูลภายนอก."

    # feature loop
    - title: "ตัวเลือกที่ปรับแต่งได้"
      content: "GroupDocs.Assembly for Node.js via Java อนุญาตให้คุณเพิ่มฟีเจอร์ต่าง ๆ เช่น บาร์โค้ด ดึงข้อมูลจาก URL และส่งออกไฟล์ในรูปแบบต่าง ๆ."

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Assembly for Node.js via Java เข้ากันได้อย่างราบรื่นกับระบบปฏิบัติการ เฟรมเวิร์ก และการจัดการแพ็คเกจชั้นนำ."
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
    GroupDocs.Assembly for Node.js via Java รองรับรายการที่กว้างขวางของ [รูปแบบเอกสาร](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "คุณสมบัติหลักของ GroupDocs.Assembly"
  description: "สร้างเอกสารและรายงานที่มีพลศาสตร์ด้วยเครื่องมือการจัดการข้อมูลที่ทรงพลัง."

  items:
    # feature loop
    - icon: "preview"
      title: "วิชวลข้อมูลที่หลากหลาย"
      content: "แทรกแผนภูมิ ตาราง รูปภาพ และรายการต่าง ๆ ลงในเอกสารของคุณได้อย่างเต็มที่."

    # feature loop
    - icon: "manipulate"
      title: "แปลงข้อมูลของคุณ"
      content: "ใช้เครื่องมืออย่างสูตรและการจัดเรียงเพื่อจัดโครงสร้างและแสดงข้อมูลอย่างมีประสิทธิภาพ."

    # feature loop
    - icon: "two_pages"
      title: "รองรับรูปแบบที่หลากหลาย"
      content: "ทำงานร่วมกับรูปแบบไฟล์ยอดนิยมสำหรับเทมเพลตและผลลัพธ์ได้อย่างไร้รอยต่อ."

    # feature loop
    - icon: "document_settings"
      title: "การปรับแต่งเทมเพลตขั้นสูง"
      content: "จัดรูปแบบเทมเพลตด้วยตัวเลือกการจัดสไตล์เช่น ตัวเลข ตัวอักษร และอื่น ๆ."

    # feature loop
    - icon: "text"
      title: "สร้างบาร์โค้ดแบบพลศาสตร์"
      content: "สร้างและฝังภาพบาร์โค้ดโดยตรงเข้าไปในเอกสารของคุณตามที่ต้องการ."

    # feature loop
    - icon: "add"
      title: "การจัดรูปแบบข้อความที่ยืดหยุ่น"
      content: "นำรูปแบบข้อความเช่น การใช้ตัวใหญ่ทั้งหมดหรือชื่อตำแหน่งในเทมเพลตของคุณได้อย่างง่ายดาย."

    # feature loop
    - icon: "manipulate"
      title: "การแทรกเนื้อหาที่พลศาสตร์"
      content: "รวมเนื้อหาจากไฟล์ภายนอกแบบพลศาสตร์ในระหว่างการสร้างเอกสาร."

    # feature loop
    - icon: "convert"
      title: "ส่งออกไปยังรูปแบบต่าง ๆ"
      content: "บันทึกเอกสารในหลายรูปแบบตามการกำหนดค่าที่คุณระบุ."

    # feature loop
    - icon: "update"
      title: "แทรกสื่อแบบพลศาสตร์"
      content: "แทรกรูปภาพหรือวัตถุอื่น ๆ โดยใช้ข้อมูล Base64 เมื่อสร้างเอกสาร."

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "ค้นหาตัวอย่างการใช้งานจริงของ GroupDocs.Assembly สำหรับงานทั่วไป."
  items:
    # code sample loop
    - title: "เพิ่มรายการแบบมีสัญลักษณ์ในเอกสาร Word"
      content: |
        ดูวิธีการสร้าง [รายการแบบมีสัญลักษณ์](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) ในเอกสาร Word เพื่อจัดระเบียบข้อมูลได้อย่างมีประสิทธิภาพ. ตัวอย่างนี้แสดงให้เห็นถึงการสร้างรายการแบบมีสัญลักษณ์โดยใช้ GroupDocs.Assembly.
        {{< landing/code title="เพิ่มรายการแบบมีสัญลักษณ์ในเอกสาร Word">}}
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
    - title: "แทรกแผนภูมิวงกลมใน PowerPoint"
      content: |
        เรียนรู้วิธีใช้เทมเพลตและ XML เพื่อเพิ่ม [แผนภูมิวงกลม](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) ในงานนำเสนอของคุณ. ปรับปรุงรายงานของคุณด้วยแผนภูมิวงกลมเพื่อเสนอข้อมูลให้ชัดเจนและเข้าใจง่าย.
        {{< landing/code title="แทรกแผนภูมิวงกลมใน PowerPoint">}}
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