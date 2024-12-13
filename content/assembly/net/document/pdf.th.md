



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: th
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ฝังเอกสารหนึ่งในอีกเอกสารหนึ่งในรูปแบบ PDF ด้วย API C#"
head_description: "รวมเอกสาร PDF อย่างมีประสิทธิภาพโดยใช้ C# ด้วย GroupDocs.Assembly รวมไฟล์ได้อย่างราบรื่นในไม่กี่ขั้นตอน"

############################# Header ############################
title: "รวมเอกสารในรูปแบบ PDF" 
description: "ด้วย GroupDocs.Assembly for .NET คุณสามารถฝังเอกสาร PDF หนึ่งในอีกเอกสารหนึ่งได้อย่างรวดเร็ว API นี้มอบเครื่องมือที่มีประสิทธิภาพสำหรับการรวมเอกสารอย่างแม่นยำ"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET คืออะไร?"
    link: "/assembly/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) เป็นเครื่องมือที่ทรงพลังสำหรับการจัดเรียงและจัดการเอกสาร มันช่วยให้ผู้ใช้สามารถฝังเอกสารหนึ่งในอีกเอกสารหนึ่ง ซึ่งช่วยให้รวมเนื้อหาได้อย่างราบรื่น โดยสนับสนุนรูปแบบมากกว่า 50 รูปแบบ—รวมถึง PDF, ไฟล์ MS Office และอื่น ๆ คุณสามารถจัดระเบียบ แก้ไข และปรับแต่งผลลัพธ์สุดท้ายให้ตรงตามความต้องการของคุณ

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการรวมเอกสารลงในไฟล์ PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ช่วยให้คุณสามารถฝังเอกสารหนึ่งในไฟล์ PDF อื่นได้อย่างราบรื่น รวมและปรับแต่งเนื้อหาได้อย่างมีประสิทธิภาพ
      
      1. ออกแบบเทมเพลตด้วยช่องว่างเฉพาะสำหรับเนื้อหาที่จะฝัง (ไม่สนับสนุนเทมเพลต PDF)
      2. กำหนดเส้นทางไฟล์สำหรับเทมเพลต
      3. ระบุเส้นทางไฟล์ของเอกสารที่จะฝัง
      4. ส่งออกไฟล์ที่เสร็จสมบูรณ์พร้อมเนื้อหาที่รวมเป็นเอกสาร PDF
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "เอกสารตัวอย่าง"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "คลิกเพื่อลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // เพิ่มแท็กนี้ในเทมเพลตของคุณเพื่อทำเครื่องหมายจุดที่แทรก
        // <<doc [doc_expression]>>

        // ระบุเส้นทางไฟล์สำหรับเทมเพลต
        // ขณะนี้ไม่สามารถใช้เทมเพลต PDF ได้
        string template = "doc_template.docx";

        // ระบุเส้นทางของเอกสารที่ต้องการฝัง
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // บันทึกเอกสารที่รวม
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ทำให้การรวมเอกสารง่ายขึ้นด้วยเครื่องมือขั้นสูง"
  description: "ห้องสมุด GroupDocs.Assembly for .NET ช่วยให้การฝังเอกสารหนึ่งในอีกเอกสารหนึ่งง่ายขึ้น สนับสนุนหลายรูปแบบไฟล์และเสนอการปรับแต่งสำหรับการรวมแบบไร้รอยต่อ"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากข้อมูลธุรกิจของคุณ"
      content: "เติมเอกสารโดยอัตโนมัติด้วยข้อมูลจาก JSON, XML, CSV หรือแหล่งข้อมูลอื่น ๆ เพื่อให้การทำงานมีประสิทธิภาพ"

    # feature loop
    - title: "เพิ่มองค์ประกอบภาพในเอกสาร"
      content: "GroupDocs.Assembly ช่วยให้คุณสามารถรวมตาราง, แผนภูมิ, และรายการ รวมถึงข้อความ, ลิงค์, รูปภาพ, และบาร์โค้ดที่สร้างขึ้นโดยอัตโนมัติ"

    # feature loop
    - title: "จัดวางและจัดรูปแบบข้อมูลอย่างแม่นยำ"
      content: "เทมเพลตที่ใช้ LINQ ช่วยให้คุณควบคุมการวางข้อมูล จัดการลูปสำหรับอาร์เรย์ และอนุญาตให้มีการปรับแต่งรูปแบบเช่นการเปลี่ยนสี"

    # feature loop
    - title: "รองรับการทำงานกับหลายรูปแบบไฟล์"
      content: "ฝังเอกสารในเอกสารอื่นได้อย่างราบรื่นข้ามรูปแบบต่าง ๆ เช่น MS Office, PDF, HTML, OpenOffice และอื่น ๆ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการฝังภาพลงในเอกสารโปรแกรมmatically"
      content: |
        ตัวอย่างนี้แสดงวิธีการแทรกรูปภาพลงในเอกสาร PDF โดยใช้ GroupDocs.Assembly
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // เพิ่มแท็กช่องว่างในเทมเพลตของคุณ
          // <<image [expression]>>

          // ระบุเส้นทางไฟล์สำหรับเทมเพลต
          // ขณะนี้ไม่สามารถใช้เทมเพลต PDF ได้
          string template = "template.docx";

          // กำหนดเส้นทางไปยังไฟล์ภาพ
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // เริ่มต้นอินสแตนซ์ของ DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกเอกสารที่มีรูปภาพที่ฝัง
          asm.AssembleDocument(template, "result.pdf", data);
          ```
        platform: "net"
        copy_title: "คัดลอก"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "คลิกเพื่อลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.pdf"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "สำรวจฟีเจอร์ของ GroupDocs.Assembly ฟรี หรือขอใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลดจาก Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "เรียนรู้เกี่ยวกับการอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ค้นพบเครื่องมืออันทรงพลังของเรา"
    exclude: "document"
    description: "สำรวจคุณสมบัติที่ GroupDocs.Assembly มีให้ สำหรับการฝังและรวมเอกสารอย่างแม่นยำ"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รวมเอกสารในหลากหลายรูปแบบ"
    exclude: "PDF"
    description: "ด้วย API .NET คุณสามารถรวมเอกสารจากรูปแบบที่สนับสนุนกว่า 50 รูปแบบ ทำให้การฝังไฟล์หรือส่วนต่าง ๆ ลงในเอกสารสุดท้ายของคุณเป็นเรื่องง่าย"
    items: 
          
        # format loop 1
        - name: "ฝังเอกสารใน PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ฝังเอกสารใน DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "ฝังเอกสารใน PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "ฝังเอกสารใน XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---