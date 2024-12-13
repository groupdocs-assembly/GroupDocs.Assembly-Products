



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:52
draft: false
lang: th
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "สร้างบาร์โค้ดในเอกสาร DOCX ด้วย C#"
head_description: "API ของ GroupDocs.Assembly for .NET ช่วยให้นักพัฒนาสามารถสร้างและฝังภาพบาร์โค้ดลงในเอกสารและอีเมลได้อย่างพลิกแพลง"

############################# Header ############################
title: "เพิ่มบาร์โค้ดในเอกสาร DOCX โดยใช้ API .NET ของเรา" 
description: "GroupDocs.Assembly for .NET รองรับการสร้างและฝังบาร์โค้ดในเอกสาร DOCX ได้อย่างเต็มที่"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดรุ่นทดลองใช้ฟรี"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "ภาพรวมของ GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ถูกสร้างขึ้นเพื่อช่วยให้คุณสร้างเอกสารและรายงานโดยการรวมข้อมูลจากแหล่งข้อมูลที่หลากหลาย สร้างเอกสารด้วยข้อความหรือข้อมูลเชิงตัวเลข สร้างแผนภูมิ ตาราง และรายการ หรือแทรกรูปภาพและบาร์โค้ดแบบเรียลไทม์ ใช้การทำเครื่องหมายขั้นสูงเพื่อตำแหน่งข้อมูลอย่างแม่นยำ รองรับรูปแบบมากกว่า 50 รูปแบบ รวมถึง PDF, ไฟล์ MS Office และอีเมล

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการเพิ่มบาร์โค้ดที่สร้างขึ้นในเอกสาร DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ทำให้ง่ายต่อการแทรกบาร์โค้ดในเท็มเพลตในรูปแบบ DOCX รองรับบาร์โค้ดมากกว่า 60 ประเภท รวมถึงรูปแบบเชิงหนึ่งและสองมิติ
      
      1. เตรียมเท็มเพลต DOCX พร้อมแท็กสำหรับบาร์โค้ด
      2. เรียกข้อมูลจากแหล่งข้อมูลที่รองรับใดๆ
      3. กำหนดคุณสมบัติเสริมเช่น ขนาดหรือความละเอียดของบาร์โค้ด
      4. บันทึกเท็มเพลตพร้อมบาร์โค้ดเป็นเอกสารใหม่
   
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
        // แทรกแท็กนี้ลงในเท็มเพลตเพื่อสร้างบาร์โค้ดในเอกสารสุดท้าย
        // <<barcode [barcode_expression] -barcode_type>>

        // ระบุเส้นทางไฟล์เท็มเพลต
        string template = "barcode_template.docx";

        // เรียกข้อมูลจากแหล่งที่มาของคุณ
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // บันทึกเอกสารพร้อมกับบาร์โค้ดที่สร้างขึ้น
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารโดยกรอกข้อมูลในเท็มเพลต"
  description: "GroupDocs.Assembly for .NET ถูกออกแบบมาเพื่อลดความซับซ้อนในการสร้างเอกสารในรูปแบบที่นิยม ใช้เท็มเพลตขั้นสูงและการทำเครื่องหมายเพื่อตั้งค่าแผนภูมิ รายการ ตาราง ลิงก์ รูปภาพ และบาร์โค้ด"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "คุณสมบัติของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากข้อมูลธุรกิจ"
      content: "API ของเราช่วยให้การกรอกข้อมูลในเอกสารรูปแบบที่นิยมเป็นไปอย่างมีประสิทธิภาพโดยใช้ข้อมูลจากแหล่งที่มาที่เป็นเช่น JSON, XML และ CSV"

    # feature loop
    - title: "ใช้เอฟเฟกต์กราฟิกเพื่อแสดงข้อมูล"
      content: "GroupDocs.Assembly รองรับการฝังองค์ประกอบพื้นเมือง เช่น รายการ ตาราง และแผนภูมิ รวมทั้งข้อความ ลิงก์ รูปภาพ และบาร์โค้ดที่สร้างขึ้นแบบพลริส"

    # feature loop
    - title: "แทรกข้อมูลได้ทุกที่ในเอกสาร"
      content: "ใช้ไวยากรณ์แบบ LINQ เพื่อวางข้อมูลอย่างแม่นยำตามที่ต้องการ อาเรย์สามารถแทรกได้โดยใช้ลูป for-each และการจัดรูปแบบ (เช่น สี) สามารถปรับเปลี่ยนได้ตามโปรแกรม"

    # feature loop
    - title: "รองรับรูปแบบที่หลากหลาย"
      content: "จัดการกับรูปแบบไฟล์ที่เป็นที่นิยม เช่น MS Office, OpenOffice, PDF, HTML และรูปแบบอีเมลต่างๆ คุณสามารถแทรกเอกสารหนึ่งในอีกเอกสารหนึ่งได้ตามต้องการ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการสร้างบาร์โค้ดแบบพลิกแพลง"
      content: |
        ตัวอย่างนี้แสดงถึงการฝังบาร์โค้ดที่สร้างขึ้นแบบพลิกแพลงลงในเอกสาร DOCX
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // ใช้เท็มเพลตนี้เพื่อแทรกบาร์โค้ดในเอกสาร
          // <<barcode [barcode_expression] -barcode_type>>

          // ระบุเส้นทางไปยังไฟล์เท็มเพลต
          string template = "barcode_template.docx";

          // เรียกข้อมูลจากแหล่งที่คุณเลือก
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // สร้างวัตถุแหล่งข้อมูลที่มีเฉพาะข้อมูลที่จำเป็นเท่านั้น
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // เริ่มต้น DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // ตั้งค่าคุณสมบัติเพิ่มเติมของบาร์โค้ด
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // บันทึกเอกสารสุดท้ายที่มีบาร์โค้ดฝังอยู่
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    exclude: "barcode"
    description: "โซลูชันของเราถูกออกแบบมาเพื่อปรับปรุงกระบวนการเอกสารธุรกิจของคุณ"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างรายงานในรูปแบบที่นิยม"
    exclude: "DOCX"
    description: ".NET รองรับการสร้างรายงานในมากกว่า 50 รูปแบบ ทำให้คุณสามารถรวมข้อมูลและเท็มเพลตได้อย่างลงตัวเพื่อผลลัพธ์ที่ยอดเยี่ยม"
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดลงใน PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดลงใน DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดลงใน PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดลงใน XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---