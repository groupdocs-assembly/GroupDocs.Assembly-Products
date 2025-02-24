---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: th
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
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "ไลบรารี Java สำหรับการสร้างเอกสาร การทำงานอัตโนมัติ และการรายงาน"
head_description: "ไลบรารี Java สำหรับการทำงานอัตโนมัติในการสร้างเอกสารและการสร้างรายงาน สร้าง PDF, Word, Excel, PPTX, HTML และเอกสารอีเมลโดยใช้เทมเพลตที่กำหนดเอง"

############################# Header ############################
title: "API Java สำหรับการทำงานอัตโนมัติรายงานและเอกสาร"
description: "ทำให้การสร้างรายงานใน Java ง่ายขึ้นโดยการรวมข้อมูลกับเทมเพลต"
words:
  for: "สำหรับ"

actions:
  main: "ขอทดลองใช้ฟรีผ่าน Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "การจัดทำใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ลองใช้ฟีเจอร์ของ GroupDocs.Assembly ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} วางจำหน่ายแล้ว"
  notes: "ดูสิ่งที่ใหม่"
  downloads: "ดาวน์โหลด"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "สร้างกราฟใน DOCX ด้วย Java"
  more: "ตัวอย่างเพิ่มเติม"
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
    // เส้นทางไปยังเทมเพลตหลัก
    String template = "chart_template.docx";

    // เรียกข้อมูลผลิตภาพของผู้จัดการจากแหล่งข้อมูล
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // สร้างอินสแตนซ์ของ DataSourceInfo ด้วยข้อมูล
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // ตั้งค่าสีกราฟโดยใช้อีก DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // กรอกข้อมูลลงในเทมเพลตและบันทึกไว้ที่เอาต์พุต
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "ภาพรวม GroupDocs.Assembly"
  description: "ไลบรารี Java ที่ออกแบบมาเพื่อการสร้างเอกสารอัตโนมัติและการรวมข้อมูลอย่างราบรื่น"
  features:
    # feature loop
    - title: "รวมข้อมูลทางธุรกิจลงในเทมเพลตด้วย Java"
      content: "สร้างรายงานระดับมืออาชีพได้ง่ายโดยการฝังข้อมูลจาก JSON, XML หรือแหล่งข้อมูลอื่นๆ ในเทมเพลตที่ออกแบบล่วงหน้าด้วย GroupDocs.Assembly for Java"

    # feature loop
    - title: "ทำงานกับวัตถุที่แทรก"
      content: "กรอกรายละเอียดต่างๆ เช่น ตาราง กราฟ และแผนภาพในเอกสารอัตโนมัติโดยใช้ข้อมูลจากแหล่งข้อมูลภายนอก"

    # feature loop
    - title: "การปรับแต่งขั้นสูง"
      content: "GroupDocs.Assembly for Java มีฟีเจอร์ที่ยืดหยุ่นเช่น การสร้างบาร์โค้ด การดึงข้อมูลออนไลน์ผ่าน URL และการส่งออกผลลัพธ์ในรูปแบบที่แตกต่างกัน"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Assembly for Java ทำงานอย่างราบรื่นกับระบบปฏิบัติการ เฟรมเวิร์ก และผู้จัดการแพ็กเกจยอดนิยม"
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
    GroupDocs.Assembly for Java รองรับ [รูปแบบเอกสาร](https://docs.groupdocs.com/assembly/java/supported-document-formats/) ที่หลากหลาย
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
  title: "ความสามารถหลักของ GroupDocs.Assembly"
  description: "สร้างเอกสารและรายงานระดับมืออาชีพด้วยการจัดการข้อมูลขั้นสูง"

  items:
    # feature loop
    - icon: "preview"
      title: "องค์ประกอบข้อมูลเชิงภาพ"
      content: "เพิ่มและปรับรูปแบบองค์ประกอบ เช่น แผนภูมิ ตาราง รูปภาพ และรายการโดยตรงในเอกสารของคุณ"

    # feature loop
    - icon: "manipulate"
      title: "การแปลงข้อมูล"
      content: "ใช้สูตร การจัดเรียง และเครื่องมืออื่นๆ เพื่อจัดระเบียบและนำเสนอข้อมูลของคุณอย่างมีประสิทธิภาพ"

    # feature loop
    - icon: "two_pages"
      title: "รองรับหลายรูปแบบ"
      content: "ทำงานอย่างง่ายดายกับประเภทไฟล์ทั่วไปสำหรับเทมเพลตและไฟล์ผลลัพธ์"

    # feature loop
    - icon: "document_settings"
      title: "การปรับแต่งเทมเพลตที่เพิ่มขึ้น"
      content: "ปรับแต่งเทมเพลตด้วยรูปแบบเชิงตัวเลข ตัวอักษร และตัวเลือกการจัดรูปแบบขั้นสูงอื่นๆ"

    # feature loop
    - icon: "text"
      title: "การสร้างบาร์โค้ดแบบไดนามิก"
      content: "สร้างและแทรกรูปภาพบาร์โค้ดอย่างรวดเร็วในเอกสารตามที่ต้องการ"

    # feature loop
    - icon: "add"
      title: "การจัดรูปแบบข้อความที่ยืดหยุ่น"
      content: "ใช้การเปลี่ยนแปลงข้อความ เช่น ตัวพิมพ์ใหญ่ ตัวพิมพ์เล็ก ตัวอักษรศีรษะ หรือรูปแบบอื่นๆ ในเทมเพลต"

    # feature loop
    - icon: "manipulate"
      title: "นำเข้าพื้นที่เนื้อหาภายนอก"
      content: "จัดใส่เนื้อหาจากไฟล์ภายนอกแบบไดนามิกขณะสร้างเอกสาร"

    # feature loop
    - icon: "convert"
      title: "ส่งออกในหลายรูปแบบ"
      content: "บันทึกเอกสารสุดท้ายในรูปแบบไฟล์ต่างๆ โดยใช้ส่วนขยายหรือการกำหนดค่า"

    # feature loop
    - icon: "update"
      title: "การแทรกสื่อแบบไดนามิก"
      content: "แทรกรูปภาพหรือเนื้อหาอื่นๆ โดยใช้ข้อมูลที่เข้ารหัสใน Base64 ขณะสร้างเอกสาร"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "สำรวจตัวอย่างโค้ดสำหรับงานทั่วไปด้วย GroupDocs.Assembly"
  items:
    # code sample loop
    - title: "สร้างรายการที่มีลูกศรใน Word"
      content: |
        เรียนรู้วิธีการเพิ่ม [รายการที่มีลูกศร](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) ในเอกสาร Word เพื่อการแสดงข้อมูลที่เป็นระเบียบ ตัวอย่างนี้แสดงวิธีการสร้างรายการใน Word โดยใช้ GroupDocs.Assembly
        {{< landing/code title="สร้างรายการที่มีลูกศรใน Word">}}
        ```java {style=abap}
        // แทรกเทมเพลตนี้บนหน้าของเอกสาร:
        // ตัวชี้วัดประสิทธิภาพของผู้จัดการ
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // ระบุเส้นทางเทมเพลต
        String template = "Bulleted List Template.docx";

        // ตั้งค่าเส้นทางไฟล์ผลลัพธ์
        String result = "Result Report.docx"

        // เรียกข้อมูลของผู้จัดการจากแหล่งข้อมูล JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // สร้างรายงานที่กรอกข้อมูล
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "สร้างกราฟวงกลมใน PPTX"
      content: |
        ใช้เทมเพลตและ XML เพื่อเพิ่ม [กราฟวงกลม](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) ในงานนำเสนอของคุณ ทำให้รายงานของคุณมีเสน่ห์มากขึ้นโดยการรวมกราฟวงกลมเพื่อแสดงข้อมูล
        {{< landing/code title="สร้างกราฟวงกลมใน PPTX">}}
        ```java {style=abap}   
        // เพิ่มเทมเพลตชื่อกราฟไปยังงานนำเสนอ:
        // รายได้จากลูกค้า <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // รวมเทมเพลตข้อมูลกราฟด้วย:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // ระบุเส้นทางเทมเพลตกราฟ
        String template = "Pie Chart Template.pptx";

        // ตั้งค่าเส้นทางไฟล์ผลลัพธ์
        String result = "Result Report.pptx"

        // เรียกข้อมูลของลูกค้าจากแหล่งข้อมูล XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // สร้างกราฟและบันทึกผลลัพธ์
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---