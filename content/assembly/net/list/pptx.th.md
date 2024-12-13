



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: th
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "สร้างรายการในเอกสาร PPTX ด้วย C#"
head_description: "API GroupDocs.Assembly for .NET ช่วยให้นักพัฒนาสามารถสร้างรายการข้อมูลแบบไดนามิกและฝังลงในเอกสารและเทมเพลตได้อย่างสะดวก"

############################# Header ############################
title: "เพิ่มรายการที่ขับเคลื่อนด้วยข้อมูลในเอกสาร PPTX โดยใช้ API .NET ของเรา" 
description: "GroupDocs.Assembly for .NET มอบเครื่องมืออันทรงพลังสำหรับการสร้างและฝังรายการในเอกสาร PPTX อย่างไดนามิก"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดเวอร์ชันทดลองฟรี"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "ภาพรวมของ GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ถูกออกแบบมาเพื่อทำให้การสร้างเอกสารและรายงานเป็นเรื่องง่ายด้วยการรวมข้อมูลจากแหล่งต่างๆ ได้อย่างราบรื่น สามารถเติมเทมเพลตด้วยรายการ แผนภูมิ ตาราง บาร์โค้ด หรือข้อความ และวางเนื้อหาอย่างแม่นยำโดยใช้ markup ขั้นสูง รองรับมากกว่า 50 รูปแบบ รวมถึง PDF ไฟล์ MS Office และอีเมล ทำให้เหมาะสมสำหรับการทำงานอัตโนมัติของเอกสาร

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการเพิ่มรายการที่เต็มไปด้วยข้อมูลในเอกสาร PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ทำให้การแทรกรายการที่ขับเคลื่อนด้วยข้อมูลในเทมเพลต PPTX เป็นเรื่องที่ตรงไปตรงมา สร้างและปรับแต่งรายการได้อย่างมีประสิทธิภาพ
      
      1. เตรียมเทมเพลต PPTX พร้อมช่องว่างสำหรับรายการ
      2. ตั้งค่าเส้นทางไปยังเทมเพลต
      3. ดึงข้อมูลจากแหล่งที่รองรับ เช่น JSON หรือตัว XML
      4. บันทึกเอกสารสุดท้ายพร้อมกับรายการที่ฝังอยู่
   
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
        // เพิ่มแท็กนี้ในเทมเพลตเพื่อมาร์กจุดที่รายการจะปรากฏ
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // ระบุเส้นทางไปยังไฟล์เทมเพลต
        string template = "list_template.pptx";

        // ดึงข้อมูลจากแหล่งที่เลือกของคุณ
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // บันทึกเอกสารพร้อมกับรายการที่สร้างขึ้น
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารโดยการเติมเทมเพลตด้วยข้อมูลที่มีโครงสร้าง"
  description: "GroupDocs.Assembly for .NET ทำให้การสร้างเอกสารที่ขับเคลื่อนด้วยข้อมูลเป็นเรื่องง่าย เพิ่มรายการ ตาราง บาร์โค้ด แผนภูมิ รูปภาพ และองค์ประกอบอื่นๆ อย่างไดนามิกด้วยเทมเพลตขั้นสูง"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "คุณสมบัติของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากข้อมูลธุรกิจ"
      content: "API จะเติมเอกสารในรูปแบบที่นิยมโดยใช้ข้อมูลจากแหล่งต่างๆ เช่น JSON, XML, CSV เป็นต้น ด้วยความถูกต้องและมีประสิทธิภาพ"

    # feature loop
    - title: "ใช้รายการและองค์ประกอบอื่นๆ เพื่อแสดงข้อมูล"
      content: "GroupDocs.Assembly ช่วยให้คุณฝังรายการ ตาราง และแผนภูมิ พร้อมกับข้อความ บาร์โค้ด ลิงก์ และรูปภาพเพื่อสร้างเอกสารที่มีโครงสร้างได้ดี"

    # feature loop
    - title: "แทรกข้อมูลในที่ที่ต้องการได้อย่างแม่นยำ"
      content: "ใช้ไวยากรณ์ที่อิงจาก LINQ เพื่อกำหนดตำแหน่งรายการและข้อมูลอื่นๆ ได้อย่างแม่นยำ ใช้ลูปเพื่อเติมรายการแบบไดนามิกและใช้การกำหนดรูปแบบที่กำหนดเองในแบบโปรแกรม"

    # feature loop
    - title: "รองรับหลายรูปแบบเอกสาร"
      content: "สร้างและจัดการเอกสารในรูปแบบต่างๆ เช่น MS Office, OpenOffice, PDF, HTML และไฟล์อีเมล รวมหลายเอกสารเข้าด้วยกันได้อย่างง่ายดาย"
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีสร้างรายการแบบไดนามิก"
      content: |
        ตัวอย่างนี้แสดงให้เห็นว่าการฝังรายการที่สร้างขึ้นแบบไดนามิกในเอกสาร PPTX ทำได้อย่างไร
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // เพิ่มแท็กตัว placeholder ในเทมเพลตสำหรับรายการ
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // ระบุเส้นทางไปยังไฟล์เทมเพลต
          string template = "numlist_template.pptx";

          // ดึงข้อมูลเพื่อเติมรายการ
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // สร้างออบเจ็กต์แหล่งข้อมูลด้วยข้อมูลที่จำเป็น
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // เริ่มต้น DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกเอกสารสุดท้ายพร้อมกับรายการที่สร้างขึ้น
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "สำรวจคุณสมบัติหลัก"
    exclude: "list"
    description: "แพลตฟอร์มของเราถูกสร้างขึ้นเพื่อทำให้การสร้างและรวมเนื้อหาที่ขับเคลื่อนด้วยข้อมูลในเอกสารเป็นเรื่องง่าย"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างเอกสารที่มีโครงสร้างในรูปแบบที่นิยม"
    exclude: "PPTX"
    description: ".NET รองรับมากกว่า 50 รูปแบบ ทำให้คุณสามารถผสานข้อมูลและเทมเพลตเพื่อผลิตผลลัพธ์ที่มีคุณภาพและมีโครงสร้าง"
    items: 
          
        # format loop 1
        - name: "สร้างรายการใน PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "สร้างรายการใน DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "สร้างรายการใน PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "สร้างรายการใน XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---