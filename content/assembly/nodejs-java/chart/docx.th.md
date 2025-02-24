



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: th
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "แทรกกราฟในไฟล์ DOCX ด้วย JavaScript"
head_description: "ด้วย GroupDocs.Assembly for Node.js via Java นักพัฒนาสามารถสร้างและฝังกราฟที่เคลื่อนไหวได้อย่างรวดเร็วในเอกสารโดยใช้แหล่งข้อมูลสด"

############################# Header ############################
title: "เพิ่มกราฟลงในไฟล์ DOCX โดยใช้ Node.js" 
description: "GroupDocs.Assembly for Node.js via Java ทำให้การรวมกราฟเข้ากับเอกสาร DOCX ด้วยการป้อนข้อมูลแบบเรียลไทม์เป็นเรื่องง่าย"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มใช้งานฟรีวันนี้"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "ภาพรวมของ GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) เป็นโซลูชันที่มีความสามารถในการสร้างเอกสารและรายงานอัตโนมัติ เพิ่มกราฟ, ตาราง, รูปภาพ, บาร์โค้ด และรายการลงในไฟล์ด้วยความแม่นยำ โซลูชันนี้รองรับรูปแบบกว่า 50 รูปแบบรวมถึง PDF, เอกสาร Office และอีเมล

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการเพิ่มกราฟเข้าไปในเอกสาร DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ช่วยให้การเพิ่มกราฟในไฟล์ DOCX เป็นเรื่องง่าย เลือกประเภทกราฟเช่น กราฟแท่ง, กราฟเส้น หรือกราฟวงกลม.
      
      1. ออกแบบเทมเพลต DOCX โดยมีที่ว่างสำหรับกราฟ.
      2. โหลดข้อมูลจากแหล่งข้อมูลที่รองรับ.
      3. กำหนดค่าออปชั่นกราฟ รวมถึงประเภท, สี และป้ายชื่อ.
      4. ส่งออกเอกสารพร้อมกราฟที่แทรก.
   
    code:
      platform: "java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "เอกสารตัวอย่าง"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "คลิกเพื่อลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // เพิ่มแท็กนี้ในเทมเพลตเพื่อสร้างกราฟ
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // ระบุเส้นทางไฟล์เทมเพลต
        const template = "chart_template.docx";

        // ดึงข้อมูลจากระบบแหล่งข้อมูลของคุณ
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // บันทึกเอกสารสุดท้ายพร้อมกราฟที่ฝัง
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ฝังกราฟในเอกสารของคุณอย่างมีประสิทธิภาพ"
  description: "GroupDocs.Assembly for Node.js via Java ช่วยให้การสร้างเอกสารที่มีฟีเจอร์หลากหลายในไฟล์ประเภทที่นิยมเป็นเรื่องง่าย ใช้เทมเพลตเพื่อเพิ่มกราฟ, ตาราง, บาร์โค้ด, รายการ, รูปภาพ และอื่นๆ โดยมีการอัปเดตข้อมูลแบบเรียลไทม์"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "ฟีเจอร์เด่นของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "แปลงข้อมูลเป็นกราฟระดับมืออาชีพ"
      content: "แปลงข้อมูลจากแหล่งเช่น JSON, XML หรือ CSV เป็นกราฟคุณภาพสูงที่สามารถฝังลงในเอกสารได้โดยตรง"

    # feature loop
    - title: "สร้างภาพที่น่าประทับใจ"
      content: "สร้างกราฟแท่ง, กราฟวงกลม และกราฟเส้นที่ทำงานร่วมกับองค์ประกอบเอกสารอื่น ๆ เช่น รูปภาพ, ตาราง และบาร์โค้ดได้อย่างไม่มีปัญหา"

    # feature loop
    - title: "การตั้งค่ากราฟและการจัดวางที่ยืดหยุ่น"
      content: "ใช้เทมเพลต LINQ ในการควบคุมการจัดตำแหน่งและรูปแบบกราฟ รวมถึงสี, รูปแบบ และป้ายเพื่อการนำเสนอที่สวยงาม"

    # feature loop
    - title: "รองรับหลายรูปแบบไฟล์"
      content: "สร้างเอกสารในรูปแบบต่างๆ เช่น MS Office, PDF, OpenOffice และ HTML โดยมีกราฟที่แทรกอย่างลงตัวเพื่อผลลัพธ์ที่เป็นมืออาชีพ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "สร้างและแทรกรูปกราฟแบบไดนามิก"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงวิธีการสร้างและฝังกราฟลงในไฟล์ DOCX โดยใช้โปรแกรม.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // ตั้งค่าเทมเพลตโดยมีที่ว่างสำหรับกราฟ
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // กำหนดเส้นทางไปยังไฟล์เทมเพลต
          const template = "table_template.docx";

          // ดึงข้อมูลจากแหล่งเลือก
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // เตรียมวัตถุข้อมูลที่มีข้อมูลกราฟ
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // เลือกประเภทกราฟและปรับแต่งรูปลักษณ์
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // เริ่มต้น DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // บันทึกเอกสารที่ปรับปรุงพร้อมกราฟที่แทรก
          asm.assembleDocument(template, "result.docx", data, design);
          ```
        platform: "java"
        copy_title: "คัดลอก"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "คลิกเพื่อลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.docx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "สำรวจฟีเจอร์ของ GroupDocs.Assembly ฟรี หรือขอใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลดจาก NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "เรียนรู้เกี่ยวกับการอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ค้นพบฟีเจอร์ขั้นสูง"
    exclude: "chart"
    description: "แพลตฟอร์มนี้ช่วยให้การสร้างเอกสารเป็นเรื่องง่ายด้วยเครื่องมือที่ออกแบบมาสำหรับการแสดงผลข้อมูลและการรวมที่ราบรื่น"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างรายงานในหลายรูปแบบไฟล์"
    exclude: "DOCX"
    description: "Node.js via Java รองรับมากกว่า 50 รูปแบบ ทำให้ง่ายต่อการรวมเทมเพลตกับข้อมูลเพื่อผลิตเอกสารที่มีคุณภาพ"
    items: 
          
        # format loop 1
        - name: "แผนภูมิใน PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "แผนภูมิใน DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "แผนภูมิใน PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "แผนภูมิใน XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---