



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:03:58
draft: false
lang: th
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "เพิ่มบาร์โค้ดในไฟล์ XLSX โดยใช้ JavaScript"
head_description: "สร้างและฝังบาร์โค้ดในเอกสารและอีเมลของคุณด้วย API ของ GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "สร้างบาร์โค้ดสำหรับไฟล์ XLSX โดยใช้ Node.js" 
description: "ด้วย GroupDocs.Assembly for Node.js via Java คุณสามารถสร้างบาร์โค้ดแบบไดนามิก ปรับแต่ง และฝังลงในเอกสาร XLSX ได้."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มต้นใช้งาน"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "แนะนำเกี่ยวกับ GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ช่วยให้คุณสร้างเอกสารระดับมืออาชีพโดยการรวมข้อมูลจากแหล่งที่มาหลายๆ แห่ง เพิ่มกราฟ ตาราง รายการ รูปภาพ และบาร์โค้ดลงในไฟล์ของคุณได้อย่างมีประสิทธิภาพ ใช้เทมเพลตเพื่อจัดระเบียบเนื้อหาให้เหมาะสมที่สุด รองรับมากกว่า 50 รูปแบบ รวมถึง PDFs เอกสาร Office และอีเมล

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการเพิ่มบาร์โค้ดในไฟล์ XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ช่วยให้คุณฝังบาร์โค้ดในเอกสาร XLSX ได้ง่าย รองรับประเภทบาร์โค้ดมากกว่า 60 ประเภท รวมถึงรูปแบบ 1D และ 2D.
      
      1. สร้างเทมเพลต XLSX โดยมี placeholder สำหรับบาร์โค้ด.
      2. ดึงข้อมูลจากแหล่งข้อมูลที่เข้ากันได้.
      3. ตั้งค่าตัวเลือกบาร์โค้ด เช่น ขนาดและความละเอียด.
      4. บันทึกเอกสารสุดท้ายที่มีบาร์โค้ดฝังอยู่.
   
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
        // ใช้แท็กนี้ในเทมเพลตเพื่อรวมบาร์โค้ดในเอกสารผลลัพธ์
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // ระบุที่อยู่ไฟล์เทมเพลต
        const template = "barcode_template.xlsx";

        // โหลดข้อมูลที่จำเป็นจากแหล่งที่มา
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // บันทึกเอกสารพร้อมบาร์โค้ดที่ประยุกต์แล้ว
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารด้วยเทมเพลตที่ขับเคลื่อนด้วยข้อมูล"
  description: "ด้วย GroupDocs.Assembly for Node.js via Java คุณสามารถสร้างไฟล์ระดับมืออาชีพในรูปแบบยอดนิยมโดยการฝังกราฟ ตาราง รายการ ลิงค์ รูปภาพ และบาร์โค้ดได้อย่างลงตัว."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานด้วยข้อมูลธุรกิจ"
      content: "ใช้ API ในการเติมเต็มเทมเพลตด้วยข้อมูลจากรูปแบบต่างๆ เช่น JSON, XML และ CSV ได้อย่างรวดเร็วและถูกต้อง."

    # feature loop
    - title: "เพิ่มส่วนประกอบภาพ"
      content: "GroupDocs.Assembly รองรับการแทรกองค์ประกอบเช่น กราฟ ตาราง รายการ ข้อความ ลิงค์ รูปภาพ และบาร์โค้ดแบบเรียลไทม์."

    # feature loop
    - title: "ควบคุมการวางข้อมูล"
      content: "ด้วยเทมเพลตที่ใช้ LINQ คุณสามารถวางข้อมูลได้อย่างแม่นยำ ทำการวนลูปผ่านอาร์เรย์ และนำรูปแบบที่กำหนดเองมาใช้ในโปรแกรม."

    # feature loop
    - title: "เข้ากันได้กับหลายรูปแบบ"
      content: "ทำงานกับไฟล์เช่น เอกสาร MS Office PDFs HTML เอกสาร OpenOffice และอีเมล รวมกันหลายเอกสารเมื่อจำเป็น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ตัวอย่าง: สร้างบาร์โค้ดแบบโปรแกรมmatically"
      content: |
        ตัวอย่างนี้แสดงวิธีการสร้างและแทรกบาร์โค้ดลงในเอกสาร XLSX แบบโปรแกรมmatically.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // ออกแบบเทมเพลตด้วย placeholder สำหรับบาร์โค้ด
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // ระบุที่อยู่ของไฟล์เทมเพลต
          const template = "barcode_template.xlsx";

          // ดึงข้อมูลจากแหล่งที่มา
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // สร้างวัตถุข้อมูลแหล่งด้วยข้อมูลที่จำเป็น
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // เริ่มต้นอินสแตนซ์ของ DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // ตั้งค่าการกำหนดค่าบาร์โค้ด
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // บันทึกเอกสารพร้อมบาร์โค้ดที่รวมอยู่
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: "สำรวจคุณสมบัติหลัก"
    exclude: "barcode"
    description: "ทำให้การประมวลเอกสารง่ายขึ้นด้วยเครื่องมืออันทันสมัยและความสามารถในการทำงานอัตโนมัติ."
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รูปแบบไฟล์ที่รองรับสำหรับการสร้างรายงาน"
    exclude: "XLSX"
    description: "Node.js via Java รองรับไฟล์มากกว่า 50 รูปแบบ ทำให้คุณสามารถรวมข้อมูลและประมวลผลเทมเพลตเพื่อผลลัพธ์ที่มีคุณภาพสูงได้."
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดลงใน PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดลงใน DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดลงใน PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดลงใน XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---