



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:02
draft: false
lang: th
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "รวมเอกสารในรูปแบบ PDF ด้วย JavaScript"
head_description: "รวมไฟล์ PDF โดยใช้ JavaScript. GroupDocs.Assembly ช่วยให้การรวมเอกสารถูกต้องและรวดเร็วในไม่กี่ขั้นตอนง่ายๆ."

############################# Header ############################
title: "รวมเนื้อหาในไฟล์ PDF ได้อย่างมีประสิทธิภาพ" 
description: "ด้วย GroupDocs.Assembly for Node.js via Java การรวมไฟล์ PDF เข้าไปในอีกไฟล์หนึ่งเป็นเรื่องที่รวดเร็วและแม่นยำ เพลิดเพลินไปกับเครื่องมือที่ยืดหยุ่นและเชื่อถือได้สำหรับการรวมเนื้อหาอย่างไร้รอยต่อ."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ทดลองใช้งานฟรี"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "ภาพรวมของ GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ให้วิธีการที่ทรงพลังในการจัดการเอกสาร รวมไฟล์หนึ่งไปยังอีกไฟล์หนึ่งได้อย่างมีประสิทธิภาพ รองรับรูปแบบมากกว่า 50 รูปแบบ เช่น PDF และ MS Office ปรับแต่งรูปแบบ แก้ไขเนื้อหา และจัดระเบียบเอกสารได้ตามต้องการ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการรวมเอกสารเข้ากับไฟล์ PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ทำให้การแทรกไฟล์ PDF ลงในอีกไฟล์หนึ่งเป็นเรื่องที่ปรับแต่งได้ง่าย.
      
      1. ออกแบบเทมเพลตที่มีที่ว่างสำหรับเนื้อหาที่ฝัง (ไม่รองรับเทมเพลต PDF).
      2. กำหนดเส้นทางไฟล์สำหรับเทมเพลต.
      3. ระบุเส้นทางไฟล์สำหรับเอกสารที่ต้องการรวม.
      4. บันทึกเอกสารที่เสร็จสมบูรณ์พร้อมเนื้อหาที่รวมในรูปแบบไฟล์ PDF.
   
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
        // เพิ่มแท็กนี้ลงในเทมเพลตเพื่อกำหนดตำแหน่งที่เอกสารจะถูกฝัง
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // กำหนดเส้นทางไฟล์สำหรับเทมเพลตหลัก
        // ในปัจจุบันไม่ได้รองรับเทมเพลต PDF.
        const template = "doc_template.docx";

        // ระบุเส้นทางสำหรับเอกสารที่คุณต้องการรวม
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // บันทึกผลลัพธ์สุดท้ายพร้อมเอกสารที่ฝังอยู่
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "เครื่องมือที่ทรงพลังสำหรับการรวมเอกสาร"
  description: "GroupDocs.Assembly for Node.js via Java ช่วยให้การฝังไฟล์ในรูปแบบต่างๆ เป็นเรื่องง่ายและปรับแต่งได้เต็มที่ มอบผลลัพธ์ที่สม่ำเสมอและเป็นมืออาชีพทุกครั้ง."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานด้วยข้อมูลธุรกิจ"
      content: "ดึงข้อมูลจาก JSON, XML หรือ CSV เพื่อสร้างรายงานและเอกสารที่ละเอียดและแม่นยำอย่างรวดเร็ว."

    # feature loop
    - title: "เพิ่มองค์ประกอบภาพที่หลากหลาย"
      content: "GroupDocs.Assembly ช่วยให้คุณรวมตาราง กราฟ รายการ รูปภาพ และบาร์โค้ดร่วมกับข้อความและลิงก์ได้."

    # feature loop
    - title: "การวางข้อมูลอย่างแม่นยำ"
      content: "ใช้เทมเพลต LINQ เพื่อจัดตำแหน่งข้อมูลให้ถูกต้องตามที่ต้องการ จัดการกับข้อมูลซ้ำ เช่น อาร์เรย์ และปรับแต่งสไตล์ได้อย่างง่ายดาย."

    # feature loop
    - title: "ทำงานกับรูปแบบที่หลากหลาย"
      content: "รวมเนื้อหาอย่างไร้รอยต่อในรูปแบบต่างๆ เช่น PDF ไฟล์ MS Office HTML และ OpenOffice โดยมอบความยืดหยุ่นสำหรับทุกโปรเจกต์."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ฝังภาพลงในเอกสารโดยโปรแกรม"
      content: |
        ตัวอย่างนี้แสดงให้เห็นวิธีการแทรกรูปภาพลงในไฟล์ PDF โดยใช้ GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // เพิ่มที่ว่างในเทมเพลตสำหรับภาพ
          // <<image [expression]>>

          // ระบุเส้นทางไปยังไฟล์เทมเพลต
          // ในปัจจุบันไม่ได้รองรับเทมเพลต PDF.
          String template = "template.docx";
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // กำหนดเส้นทางไปยังรูปภาพที่คุณต้องการฝัง
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // เริ่มต้นวัตถุ DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // บันทึกเอกสารพร้อมด้วยภาพที่ฝังอยู่
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "ฟีเจอร์หลักในภาพรวม"
    exclude: "document"
    description: "สำรวจเครื่องมือที่ครบครันที่ GroupDocs.Assembly มีเพื่อการรวมเอกสารที่มีประสิทธิภาพและไร้รอยต่อ."
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รวมเอกสารในหลายรูปแบบ"
    exclude: "PDF"
    description: "ใช้ Node.js via Java เพื่อรวมเนื้อหาในกว่ารูปแบบไฟล์ 50 รูปแบบ เพื่อผลลัพธ์ที่เป็นมืออาชีพและดูดี."
    items: 
          
        # format loop 1
        - name: "ฝังเอกสารใน PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ฝังเอกสารใน DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "ฝังเอกสารใน PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "ฝังเอกสารใน XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---