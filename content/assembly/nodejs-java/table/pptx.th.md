



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: th
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "แทรกตารางในเอกสาร PPTX ด้วย JavaScript"
head_description: "ใช้ GroupDocs.Assembly for Node.js via Java เพื่อแทรกตารางในเอกสารหรืออีเมลได้อย่างรวดเร็ว โดยดึงข้อมูลจากแหล่งต่างๆ."

############################# Header ############################
title: "เพิ่มตารางลงในไฟล์ PPTX อย่างไม่ยุ่งยากด้วย Node.js" 
description: "ด้วย GroupDocs.Assembly for Node.js via Java การกรอกตารางในเอกสาร PPTX เป็นเรื่องง่าย โดยใช้ข้อมูลจากหลายแหล่ง."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มทดลองใช้งานฟรีของคุณ"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "แนะนำ GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) เป็นเครื่องมือทรงพลังสำหรับการสร้างเอกสารอัตโนมัติ ช่วยให้คุณสามารถแทรกตาราง แผนภูมิ รายการ และรูปภาพลงในเทมเพลต พร้อมการวางเนื้อหาที่แม่นยำ สนับสนุนกว่า 50 รูปแบบไฟล์ รวมถึง PDF, Word, และอีเมล ช่วยให้กระบวนการสร้างรายงานและงานอื่นๆ เป็นไปอย่างราบรื่น.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีเพิ่มข้อมูลในตารางใน PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ช่วยให้คุณสามารถกรอกเทมเพลตตารางสำหรับไฟล์ PPTX ได้อย่างรวดเร็ว โดยใช้แหล่งข้อมูลเชิงพลศาสตร์.
      
      1. สร้างเทมเพลต PPTX พร้อมตัวแทนสำหรับแถวและคอลัมน์ตาราง.
      2. โหลดข้อมูลจากแหล่งที่รองรับ เช่น JSON หรือ CSV.
      3. จัดระเบียบและจัดรูปแบบข้อมูลตามต้องการ.
      4. สร้างเอกสารที่มีตารางที่เสร็จสมบูรณ์.
   
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
        // รวมแท็กเหล่านี้ในตัวแทนแถวตารางของเทมเพลตของคุณ
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // ระบุที่อยู่ไฟล์เทมเพลต
        const template = "table_template.pptx";

        // นำเข้าข้อมูลจากแหล่งที่เลือก
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // บันทึกเอกสารสุดท้ายด้วยตารางที่เสร็จสมบูรณ์
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มตารางที่ขับเคลื่อนด้วยข้อมูลลงในเอกสารอย่างง่ายดาย"
  description: "GroupDocs.Assembly for Node.js via Java ช่วยให้ผู้ใช้สร้างตารางอัตโนมัติ ขณะเดียวกันก็แทรกแผนภูมิ รูปภาพ และรายการโดยใช้การทำงานตามเทมเพลต."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "คุณสมบัติเด่นของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างตารางจากข้อมูลที่มีโครงสร้าง"
      content: "ดึงข้อมูลจาก JSON, XML, CSV, และรูปแบบอื่นๆ เพื่อกรอกข้อมูลในตารางเอกสารโดยอัตโนมัติ."

    # feature loop
    - title: "สร้างเนื้อหาที่มีลักษณะสวยงาม"
      content: "ใช้ GroupDocs.Assembly ในการออกแบบตาราง แผนภูมิ และรายการระดับมืออาชีพ และเพิ่มลิงค์ รูปภาพ และข้อความเพื่อปรับแต่งลักษณะของเอกสาร."

    # feature loop
    - title: "การวางเนื้อหาตารางแบบไดนามิก"
      content: "เพิ่มแถวและคอลัมน์ด้วยโปรแกรมโดยใช้เทมเพลตพื้นฐาน LINQ และปรับแต่งสไตล์ เช่น ฟอนต์ สี และการจัดแนว."

    # feature loop
    - title: "ทำงานได้อย่างไร้รอยต่อในหลากหลายรูปแบบ"
      content: "สร้างหรือแก้ไขตารางใน MS Office, OpenOffice, PDF, HTML, และรูปแบบอื่นๆ ได้โดยง่าย รวมเข้ากับไฟล์ตามที่ต้องการ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการกรอกตารางแบบโปรแกรม"
      content: |
        ตัวอย่างนี้แสดงการกรอกตารางในเอกสาร PPTX ด้วยข้อมูลจากแหล่งภายนอก.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // ออกแบบเทมเพลตที่มีตัวแทนสำหรับตาราง
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // ระบุที่อยู่ไฟล์สำหรับเทมเพลต
          const template = "table_template.pptx";

          // โหลดข้อมูลที่จำเป็นจากแหล่งของคุณ
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // จัดระเบียบข้อมูลให้อยู่ในโครงสร้างที่จำเป็น
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // เริ่มต้น DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // บันทึกเอกสารผลลัพธ์ด้วยตารางที่เสร็จสมบูรณ์
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "คุณสมบัติหลักในภาพรวม"
    exclude: "table"
    description: "API ของเราช่วยให้อัตโนมัติในการสร้างตารางและพัฒนากระบวนการสร้างเอกสารด้วยเครื่องมือและเทมเพลตที่หลากหลาย."
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างตารางในรูปแบบที่หลากหลาย"
    exclude: "PPTX"
    description: "ด้วย Node.js via Java คุณสามารถกรอกเทมเพลตและสร้างตารางที่ครบถ้วนในมากกว่า 50 รูปแบบไฟล์ที่รองรับ."
    items: 
          
        # format loop 1
        - name: "เพิ่มตารางใน PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มตารางใน DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "เพิ่มตารางใน PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "เพิ่มตารางใน XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---