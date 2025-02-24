



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: th
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "สร้างรายการแบบไดนามิกใน XLSX ด้วย JavaScript"
head_description: "ออกแบบและแทรกรายการในเทมเพลต XLSX โดยใช้ API ของ GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "แทรกรายการที่ขับเคลื่อนด้วยข้อมูลในไฟล์ XLSX ด้วย Node.js" 
description: "GroupDocs.Assembly for Node.js via Java มอบเครื่องมือที่ทรงพลังในการเพิ่มรายการที่ยืดหยุ่นและขับเคลื่อนด้วยข้อมูลลงในเอกสาร XLSX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มต้นใช้งานฟรี"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับ GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ช่วยให้การสร้างเอกสารเป็นเรื่องง่ายด้วยการดึงข้อมูลจากแหล่งต่าง ๆ และแทรกเข้าไปในเทมเพลต ใช้เพื่อสร้างรายการ ตาราง แผนภูมิ และองค์ประกอบอื่น ๆ พร้อมตัวเลือกในการจัดวางและการจัดรูปแบบที่แม่นยำ รองรับกว่า 50 รูปแบบ รวมทั้ง PDF, MS Office และอีเมล ช่วยให้คุณสามารถทำงานเอกสารอัตโนมัติได้

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการแทรกรายการลงในไฟล์ XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ทำให้การเพิ่มรายการที่มีรายละเอียดและขับเคลื่อนด้วยข้อมูลลงในเทมเพลต XLSX เป็นเรื่องง่าย.
      
      1. สร้างเทมเพลต XLSX และกำหนดจุดแทนสำหรับรายการ.
      2. ระบุเส้นทางไฟล์ของเทมเพลต.
      3. โหลดข้อมูลจากแหล่งที่รองรับ เช่น JSON หรือ XML.
      4. บันทึกเอกสารพร้อมกับรายการที่สร้างขึ้น.
   
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
        // แทรกแท็กนี้ในเทมเพลตเพื่อทำเครื่องหมายจุดที่รายการจะไป
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // ตั้งค่าเส้นทางไฟล์สำหรับเทมเพลตของคุณ
        const template = "list_template.xlsx";

        // ดึงข้อมูลจากแหล่งที่คุณต้องการใช้งาน
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // บันทึกไฟล์พร้อมด้วยรายการที่แทรก
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารได้อย่างง่ายดายด้วยข้อมูลที่รวมเข้าด้วยกัน"
  description: "ด้วย GroupDocs.Assembly for Node.js via Java คุณสามารถแทรกรายการ ตาราง แผนภูมิ และองค์ประกอบอื่น ๆ ลงในเทมเพลต ช่วยประหยัดเวลาและความพยายาม."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "จุดเด่นของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากแหล่งข้อมูลหลายแห่ง"
      content: "นำเข้าข้อมูลจาก JSON, XML, CSV หรือรูปแบบอื่น ๆ เพื่อนำไปใช้ในการเติมรายการและองค์ประกอบอื่น ๆ ได้อย่างมีประสิทธิภาพ."

    # feature loop
    - title: "เพิ่มรายการและองค์ประกอบภาพอื่น ๆ"
      content: "GroupDocs.Assembly ช่วยให้คุณแทรกรายการ ตาราง แผนภูมิ และอื่น ๆ ได้อย่างไร้รอยต่อควบคู่ไปกับข้อความ รูปภาพ และลิงก์เพื่อผลลัพธ์ที่ดูดี."

    # feature loop
    - title: "ควบคุมตำแหน่งและสไตล์ข้อมูลอย่างแม่นยำ"
      content: "เทมเพลตที่ใช้ LINQ ช่วยให้คุณควบคุมได้อย่างแน่ชัดว่ารายการและข้อมูลอื่น ๆ จะปรากฏที่ใด ใช้ลูปสำหรับรายการที่ซ้ำกัน และปรับแต่งสไตล์ให้เหมาะกับความต้องการของคุณ."

    # feature loop
    - title: "ทำงานในหลายรูปแบบ"
      content: "สร้างเอกสารในรูปแบบต่าง ๆ เช่น MS Office, PDF, OpenOffice, HTML และอีเมล รวมเนื้อหาจากแหล่งต่าง ๆ เป็นไฟล์เดียว."
      
  code_samples_ext:
    # code sample ext loop
    - title: "สร้างรายการในเอกสารด้วยโปรแกรม"
      content: |
        ตัวอย่างนี้แสดงวิธีการเพิ่มรายการแบบไดนามิกไปยังเอกสาร XLSX โดยใช้ GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // เพิ่มจุดแทนในเทมเพลตสำหรับรายการ
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // ระบุเส้นทางไฟล์ของเทมเพลต
          const template = "numlist_template.xlsx";

          // โหลดข้อมูลเพื่อนำไปเติมรายการ
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // เตรียมแหล่งข้อมูลด้วยรายละเอียดที่จำเป็น
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // เริ่มต้น DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // บันทึกเอกสารสุดท้ายพร้อมด้วยรายการที่รวมอยู่
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "สำรวจฟีเจอร์ของ GroupDocs.Assembly"
    exclude: "list"
    description: "ออกแบบและสร้างเอกสารที่อุดมไปด้วยข้อมูลได้อย่างง่ายดายด้วยเครื่องมือการรวมที่ทรงพลัง."
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
    title: "สร้างเอกสารในหลายรูปแบบ"
    exclude: "XLSX"
    description: "Node.js via Java รองรับรูปแบบไฟล์มากกว่า 50 รูปแบบ ทำให้การรวมเทมเพลตและข้อมูลเป็นไปอย่างมืออาชีพ."
    items: 
          
        # format loop 1
        - name: "สร้างรายการใน PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "สร้างรายการใน DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "สร้างรายการใน PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "สร้างรายการใน XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---