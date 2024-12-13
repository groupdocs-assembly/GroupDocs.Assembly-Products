---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: th
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
head_title: "API .NET สำหรับการทำเอกสาร การประกอบและการสร้างรายงาน"
head_description: "API C# .NET สำหรับการทำเอกสาร การประกอบและการสร้างรายงาน สร้าง PDF, Word, Excel, PPTX, HTML และเอกสารอีเมลจากเทมเพลตที่กำหนดเอง"

############################# Header ############################
title: "API การทำเอกสารและรายงาน .NET"
description: "สร้างรายงานในแอปพลิเคชัน .NET โดยการกำหนดเทมเพลตและรวมข้อมูล"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลดทดลองใช้ฟรีผ่าน NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "การจัดทำใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ลองใช้ฟีเจอร์ของ GroupDocs.Assembly ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} วางจำหน่ายแล้ว"
  notes: "ดูสิ่งที่ใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "กรอกกราฟใน DOCX โดยใช้ C#"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // เส้นทางไปยังเทมเพลตหลัก
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "ภาพรวม GroupDocs.Assembly"
  description: "โซลูชัน .NET สำหรับการทำเอกสารอัตโนมัติด้วยการรวมข้อมูลขั้นสูง"
  features:
    # feature loop
    - title: "เพิ่มข้อมูลทางธุรกิจลงในเทมเพลตเอกสารด้วย C#"
      content: "การสร้างรายงานที่ง่ายขึ้น: ด้วย GroupDocs.Assembly for .NET คุณสามารถแทรกข้อมูลจากแหล่งข้อมูลเช่น JSON หรือ XML ลงในเทมเพลตที่กำหนดล่วงหน้าได้อย่างง่ายดาย"

    # feature loop
    - title: "จัดการวัตถุข้อมูลพื้นฐาน"
      content: "ประเภทเอกสารที่รองรับรวมถึงวัตถุที่ฝังอยู่เช่น แผนภูมิ ตาราง และรายการที่สามารถกรอกได้โดยอัตโนมัติโดยข้อมูล"

    # feature loop
    - title: "ฟีเจอร์เพิ่มเติม"
      content: "GroupDocs.Assembly for .NET มีตัวเลือกการกำหนดค่าที่กว้างขวาง ออกแบบวัตถุข้อมูลในเชิงโปรแกรม สร้างบาร์โค้ด ใช้แหล่งข้อมูลออนไลน์ผ่าน URL และบันทึกผลลัพธ์ในรูปแบบต่างๆ"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Assembly for .NET รองรับระบบปฏิบัติการ เฟรมเวิร์ก และผู้จัดการแพ็กเกจต่อไปนี้"
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
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Assembly for .NET สามารถประมวลผลรูปแบบ [ไฟล์](https://docs.groupdocs.com/assembly/net/supported-document-formats/) ต่อไปนี้
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
  title: "ฟีเจอร์ของ GroupDocs.Assembly"
  description: "สร้างเอกสารและรายงานโดยใช้โมเดลข้อมูลขั้นสูง"

  items:
    # feature loop
    - icon: "preview"
      title: "การนำเสนอข้อมูลที่ก้าวหน้า"
      content: "รองรับวัตถุข้อมูลที่หลากหลายเช่น แผนภูมิ รายการ ตาราง รูปภาพ และอื่นๆ"

    # feature loop
    - icon: "manipulate"
      title: "การจัดการข้อมูล"
      content: "ใช้สูตรและการดำเนินการตามลำดับเพื่อจัดรูปแบบและแสดงข้อมูลอย่างมีประสิทธิภาพ"

    # feature loop
    - icon: "two_pages"
      title: "รองรับรูปแบบที่กว้างขวาง"
      content: "ทำงานโดยตรงกับรูปแบบเอกสารทั่วไปทั้งหมดสำหรับเทมเพลตหรือไฟล์ผลลัพธ์"

    # feature loop
    - icon: "document_settings"
      title: "การทำเครื่องหมายเทมเพลตที่หลากหลาย"
      content: "ใช้การจัดรูปแบบเชิงลำดับ หมายเลข และการจัดรูปแบบแบบอักษรในเทมเพลต"

    # feature loop
    - icon: "text"
      title: "ฝังบาร์โค้ด"
      content: "สร้างภาพบาร์โค้ดแบบไดนามิกและแทรกลงในเอกสารของคุณ"

    # feature loop
    - icon: "add"
      title: "การจัดรูปแบบข้อมูล"
      content: "จัดรูปแบบสตริงในเทมเพลตเป็นตัวพิมพ์ใหญ๋ ตัวพิมพ์เล็ก ซึ่งใช้รูปแบบตัวอักษรหรือใช้ต้นด้วยตัวพิมพ์ใหญ่"

    # feature loop
    - icon: "manipulate"
      title: "การจัดการเนื้อหาเอกสาร"
      content: "แทรกเนื้อหาจากเอกสารภายนอกไปยังรายงานของคุณได้อย่างไดนามิก"

    # feature loop
    - icon: "convert"
      title: "บันทึกในหลายรูปแบบ"
      content: "ระบุรูปแบบไฟล์ผลลัพธ์โดยใช้ส่วนขยายไฟล์หรือการกำหนดค่าที่ละเอียด"

    # feature loop
    - icon: "update"
      title: "การประมวลผลข้อมูลที่ยืดหยุ่น"
      content: "แทรกรูปภาพและเอกสารแบบไดนามิกโดยใช้ไบต์ที่เข้ารหัสใน Base64"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "ตัวอย่างโค้ดสำหรับการดำเนินการแบบทั่วไปของ GroupDocs.Assembly"
  items:
    # code sample loop
    - title: "รายการที่เป็นจุดในเอกสาร Microsoft Word"
      content: |
        [รายการที่เป็นจุด](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) เป็นวิธีทั่วไปในการนำเสนอข้อมูลทางธุรกิจ นี่คือตัวอย่างการเพิ่มรายการในเอกสาร Word โดยใช้ GroupDocs.Assembly
        {{< landing/code title="วิธีการกรอกข้อมูลในรายการในเอกสาร">}}
        ```csharp {style=abap}
        // แทรกเทมเพลตนี้บนหน้าของเอกสาร:
        // ตัวชี้วัดประสิทธิภาพของผู้จัดการ
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // ระบุเส้นทางเทมเพลต
        string template = "Bulleted List Template.docx";

        // ตั้งค่าเส้นทางไฟล์ผลลัพธ์
        string result = "Result Report.docx"

        // เรียกข้อมูลของผู้จัดการจากแหล่งข้อมูล JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // สร้างรายงานที่กรอกข้อมูล
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "กราฟวงกลมในงานนำเสนอ PPTX"
      content: |
        คุณสามารถสร้าง [กราฟวงกลม](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) โดยใช้เทมเพลตและข้อมูล XML เพิ่มความน่าสนใจให้กับรายงานของคุณด้วยการแสดงผลข้อมูลที่น่าสนใจ
        {{< landing/code title="วิธีการแสดงข้อมูลในกราฟวงกลม">}}
        ```csharp {style=abap}
        // เพิ่มเทมเพลตชื่อกราฟไปยังงานนำเสนอ:
        // รายได้จากลูกค้า <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // รวมเทมเพลตข้อมูลกราฟด้วย:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // ระบุเส้นทางเทมเพลตกราฟ
        string template = "Pie Chart Template.pptx";

        // ตั้งค่าเส้นทางไฟล์ผลลัพธ์
        string result = "Result Report.pptx"

        // เรียกข้อมูลของลูกค้าจากแหล่งข้อมูล XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // สร้างกราฟและบันทึกผลลัพธ์
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---