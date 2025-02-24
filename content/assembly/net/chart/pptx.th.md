



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: th
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# สร้างกราฟในไฟล์ PPTX"
head_description: "API GroupDocs.Assembly for .NET ช่วยให้นักพัฒนาสามารถสร้างและแทรกรูปกราฟหรือกราฟลงในเอกสารโดยอัตโนมัติด้วยข้อมูลเรียลไทม์."

############################# Header ############################
title: "แทรกรูปกราฟในไฟล์ PPTX ด้วย API .NET" 
description: "GroupDocs.Assembly for .NET มอบวิธีการที่ทรงพลังในการเติมข้อมูลที่เป็นพลศาสตร์ลงในไฟล์ PPTX และรวมกราฟได้อย่างราบรื่น."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ทดลองใช้งานฟรี"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET คืออะไร?"
    link: "/assembly/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) เป็นเครื่องมือที่ออกแบบมาเพื่อทำให้การสร้างเอกสารและรายงานมีความเรียบง่ายโดยการรวมข้อมูลจากแหล่งข้อมูลที่หลากหลาย สามารถสร้างกราฟ, ตาราง, รายการ, บาร์โค้ดและภาพได้โดยอัตโนมัติ ตัวเลือกการตั้งค่าขั้นสูงช่วยให้สามารถจัดวางและปรับแต่งเนื้อหาของคุณได้อย่างแม่นยำ สนับสนุนไฟล์มากกว่า 50 รูปแบบ รวมถึง PDF, เอกสาร MS Office และอีเมล.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการเพิ่มกราฟลงในเอกสาร PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ทำให้การสร้างและแทรกรูปกราฟลงในเทมเพลต PPTX เป็นเรื่องง่าย รองรับประเภทกราฟที่หลากหลาย เช่น กราฟแท่ง, กราฟวงกลม และกราฟเส้น.
      
      1. ออกแบบเทมเพลต PPTX โดยมีพื้นที่สำหรับกราฟ.
      2. ดึงข้อมูลจากแหล่งข้อมูลที่รองรับ.
      3. กำหนดตัวเลือกกราฟ เช่น ประเภท, แท็ก และโทนสี.
      4. บันทึกไฟล์ที่อัปเดตพร้อมกราฟที่แทรกอยู่.
   
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
        // รวมแท็กนี้ในเทมเพลตของคุณเพื่อสร้างกราฟ
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // ระบุเส้นทางไฟล์สำหรับเทมเพลตของคุณ
        string template = "chart_template.pptx";

        // โหลดข้อมูลจากแหล่งที่คุณต้องการ
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // บันทึกเอกสารที่แทรกรูปกราฟแล้ว
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มกราฟพลศาสตร์ลงในเอกสารของคุณได้อย่างราบรื่น"
  description: "GroupDocs.Assembly for .NET ทำให้การสร้างเอกสารที่ขับเคลื่อนด้วยข้อมูลในรูปแบบที่ใช้กันทั่วไปเป็นไปอย่างสะดวก ใช้เทมเพลตเพื่อแทรกรูปกราฟ, ตาราง, บาร์โค้ด, รายการ, ลิงก์และภาพด้วยการรวมข้อมูลที่เป็นพลศาสตร์อย่างก้าวหน้ากว่า."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "แปลงข้อมูลเป็นกราฟมืออาชีพ"
      content: "เปลี่ยนข้อมูลจาก JSON, XML, CSV, และแหล่งข้อมูลอื่น ๆ ให้เป็นกราฟที่น่าดึงดูดด้วยขั้นตอนง่าย ๆ โดยใช้ API ของเรา."

    # feature loop
    - title: "สร้างเนื้อหาที่ดึงดูดสายตา"
      content: "GroupDocs.Assembly รองรับประเภทกราฟหลายแบบ เช่น กราฟแท่ง, กราฟวงกลม, และกราฟเส้น รวมเข้ากับตาราง, บาร์โค้ด, ภาพ และองค์ประกอบอื่น ๆ เพื่อสร้างรายงานระดับมืออาชีพ."

    # feature loop
    - title: "จัดวางและปรับแต่งกราฟอย่างแม่นยำ"
      content: "ด้วยไวยากรณ์ LINQ คุณสามารถสร้างและวางกราฟที่จำเป็นได้ตามต้องการ ปรับแต่งสไตล์, สี และรูปแบบให้ตรงกับความต้องการของคุณได้อย่างง่ายดาย."

    # feature loop
    - title: "ทำงานกับรูปแบบไฟล์ที่หลากหลาย"
      content: "ผลิตเอกสารในรูปแบบที่นิยมเช่น MS Office, PDF, OpenOffice และ HTML แทรกรูปกราฟได้อย่างราบรื่นในรูปแบบที่รองรับทั้งหมด."
      
  code_samples_ext:
    # code sample ext loop
    - title: "สร้างกราฟโดยโปรแกรม"
      content: |
        ตัวอย่างนี้แสดงวิธีการสร้างและแทรกรูปกราฟในเอกสาร PPTX โดยอัตโนมัติ.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // เตรียมเทมเพลตพร้อมพื้นที่สำหรับกราฟ
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // ระบุเส้นทางไปยังไฟล์เทมเพลต
          string template = "table_template.pptx";

          // ดึงข้อมูลจากแหล่งที่คุณเลือก
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // สร้างอ็อบเจ็กต์ข้อมูลที่มีข้อมูลที่จำเป็น
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // ตั้งค่าคุณสมบัติของกราฟ เช่น ประเภทและลักษณะ
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // เริ่มต้น DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // ส่งออกเอกสารพร้อมกราฟที่รวมอยู่
          asm.AssembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "ค้นพบความสามารถหลัก"
    exclude: "chart"
    description: "แพลตฟอร์มของเราช่วยให้คุณสร้างเอกสารที่น่าดึงดูดและขับเคลื่อนด้วยข้อมูลที่ปรับแต่งตามความต้องการของคุณ."
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
    title: "สร้างรายงานที่มีภาพลักษณ์หลากหลายรูปแบบ"
    exclude: "PPTX"
    description: ".NET ช่วยให้คุณสร้างเอกสารที่มีกราฟที่รวมอยู่ในรูปแบบที่รองรับมากกว่า 50 รูปแบบ โดยการรวมเทมเพลตกับข้อมูลของคุณอย่างราบรื่น."
    items: 
          
        # format loop 1
        - name: "แผนภูมิใน PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "แผนภูมิใน DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "แผนภูมิใน PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "แผนภูมิใน XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---