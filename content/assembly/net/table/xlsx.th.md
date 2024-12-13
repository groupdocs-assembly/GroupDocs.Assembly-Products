



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:57
draft: false
lang: th
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "สร้างตารางในเอกสาร XLSX ด้วย C#"
head_description: "API GroupDocs.Assembly for .NET ช่วยให้นักพัฒนาสามารถเพิ่มและเติมตารางในเอกสารและอีเมลด้วยข้อมูลจากแหล่งข้อมูลไดนามิกได้อย่างมีประสิทธิภาพ"

############################# Header ############################
title: "สร้างตารางข้อมูลในเอกสาร XLSX โดยใช้ API .NET ของเรา" 
description: "GroupDocs.Assembly for .NET ทำให้การเติมตารางในเอกสาร XLSX ด้วยข้อมูลจากแหล่งที่มาแตกต่างกันเป็นเรื่องง่าย"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดการทดลองใช้ฟรี"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "ภาพรวมของ GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ถูกสร้างขึ้นเพื่อสร้างเอกสารและรายงานโดยการเติมเทมเพลตด้วยข้อมูลจากหลายแหล่ง ข้อมูลที่มีโครงสร้างสามารถถูกเพิ่มเข้าไปในตาราง รายการ และกราฟอย่างง่ายดาย หรือแทรกรูปภาพแบบไดนามิกได้ การใช้งานซินแทกซ์ขั้นสูงทำให้การจัดวางข้อมูลนั้นถูกต้อง รองรับกว่า 50 รูปแบบ รวมถึง PDF เอกสาร MS Office และไฟล์อีเมล

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการเติมตารางในเอกสาร XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ช่วยให้คุณสามารถเติมตารางในเทมเพลตสำหรับรูปแบบเช่น XLSX ได้อย่างไดนามิก ใส่ข้อมูลจากแหล่งที่มาหลายแห่งลงในตารางของคุณ
      
      1. สร้างเทมเพลต XLSX พร้อมที่ว่างสำหรับตาราง
      2. ดึงข้อมูลจากแหล่งที่รองรับใด ๆ
      3. กรองข้อมูลเพื่อรวมเฉพาะข้อมูลที่ต้องการ
      4. บันทึกเอกสารที่มีตารางที่เติมข้อมูลแล้ว
   
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
        // เพิ่มแท็กเหล่านี้เข้าไปในแถวของเทมเพลตตาราง
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // ตั้งค่าพาธไฟล์สำหรับเทมเพลต
        string template = "table_template.xlsx";

        // ดึงข้อมูลจากแหล่งข้อมูลที่รองรับ
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // บันทึกเอกสารที่มีตารางที่เติมข้อมูลแล้ว
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารที่มีตารางไดนามิก"
  description: "GroupDocs.Assembly for .NET ช่วยให้การสร้างเอกสารเป็นไปอย่างราบรื่นโดยการทำให้ตารางถูกเติมโดยอัตโนมัติ และสนับสนุนองค์ประกอบอื่น ๆ เช่น กราฟ รายการ และรูปภาพผ่านเทมเพลตและมาร์กอัปขั้นสูง"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากข้อมูลที่มีโครงสร้าง"
      content: "API สามารถประมวลผลข้อมูลจากแหล่งเช่น JSON, XML และ CSV เพื่อเติมตารางในเอกสารสำนักงานได้อย่างมีประสิทธิภาพและแม่นยำ"

    # feature loop
    - title: "แสดงข้อมูลด้วยภาพ"
      content: "GroupDocs.Assembly อนุญาตให้สร้างตาราง รายการ และกราฟ รวมถึงการแทรกข้อความ ลิงก์ และรูปภาพเพื่อออกแบบเอกสารที่มีคุณภาพสูง"

    # feature loop
    - title: "จัดวางข้อมูลในตารางอย่างแม่นยำ"
      content: "ใช้ซินแทกซ์ที่อิงตาม LINQ เพื่อเพิ่มแถวและคอลัมน์ในตารางแบบไดนามิก ปรับแต่งสไตล์ รวมถึงสีและรูปแบบได้อย่างมีประสิทธิภาพ"

    # feature loop
    - title: "รองรับรูปแบบที่หลากหลาย"
      content: "จัดการกับรูปแบบไฟล์ที่เป็นที่นิยมเช่น MS Office, OpenOffice, PDF และ HTML ได้อย่างราบรื่น แทรกตารางที่เติมข้อมูลแล้วเข้ากับประเภทเอกสารที่รองรับ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการเติมตารางข้อมูลแบบไดนามิก"
      content: |
        ตัวอย่างนี้แสดงวิธีการเติมตารางในเอกสาร XLSX โดยใช้ข้อมูลแบบไดนามิก
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // เตรียมเทมเพลตพร้อมที่ว่างสำหรับตาราง
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // ระบุพาธไฟล์ไปยังเทมเพลต
          string template = "table_template.xlsx";

          // ดึงข้อมูลจากแหล่งข้อมูลที่คุณเลือก
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // สร้างวัตถุแหล่งข้อมูลด้วยข้อมูลที่จำเป็น
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // เริ่มต้น DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกเอกสารที่เสร็จสมบูรณ์พร้อมด้วยตารางที่เติมข้อมูลแล้ว
          asm.AssembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_table.xlsx"
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
    exclude: "table"
    description: "โซลูชันของเราช่วยให้การสร้างเอกสารมืออาชีพที่มีตารางที่เติมข้อมูลแบบไดนามิกและองค์ประกอบเพิ่มเติมนั้นเป็นเรื่องง่าย"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างรายงานที่มีตารางรายละเอียด"
    exclude: "XLSX"
    description: ".NET สามารถสร้างรายงานที่ครอบคลุมโดยการเติมเทมเพลตด้วยตารางและองค์ประกอบข้อมูลอื่น ๆ ในมากกว่า 50 รูปแบบที่รองรับ"
    items: 
          
        # format loop 1
        - name: "เพิ่มตารางใน PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มตารางใน DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "เพิ่มตารางใน PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "เพิ่มตารางใน XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---