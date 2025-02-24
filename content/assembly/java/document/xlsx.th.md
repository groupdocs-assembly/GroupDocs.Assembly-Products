



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: th
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "แทรกเอกสารหนึ่งลงในอีกเอกสารในรูปแบบ XLSX โดยใช้ Java"
head_description: "รวมไฟล์ XLSX ด้วย Java ได้อย่างมีประสิทธิภาพ GroupDocs.Assembly ทำให้กระบวนการรวมเอกสารง่ายขึ้นในไม่กี่บรรทัดของโค้ด"

############################# Header ############################
title: "ฝังเนื้อหาเข้าสู่ไฟล์ XLSX อย่างมีประสิทธิภาพ" 
description: "ใช้ GroupDocs.Assembly for Java ในการแทรกเอกสาร XLSX หนึ่งเข้าไปอีกเอกสารหนึ่งได้อย่างราบรื่น รับผลที่แม่นยำด้วยเครื่องมือที่ยืดหยุ่นและเชื่อถือได้"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "รับฟรีตอนนี้"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "คืออะไร GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) เป็นโซลูชันที่หลากหลายสำหรับการจัดการเอกสาร มันช่วยให้คุณสามารถรวมเอกสารหนึ่งเข้าไปในอีกเอกสารหนึ่งได้อย่างง่ายดาย รองรับกว่า 50 รูปแบบ เช่น PDFs และไฟล์ MS Office ปรับแต่งผลลัพธ์ของคุณโดยการรวม แก้ไข และจัดระเบียบเนื้อหาให้ตรงตามต้องการ

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการแทรกเอกสารลงในไฟล์ XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ทำให้การฝังเอกสาร XLSX หนึ่งเข้าไปอีกเอกสารหนึ่งเป็นเรื่องง่ายและปรับแต่งได้
      
      1. เตรียมเทมเพลต XLSX โดยมีพ้อยส์สำหรับเนื้อหาที่ฝังอยู่
      2. ระบุที่อยู่ไฟล์สำหรับเทมเพลต
      3. ให้ที่อยู่ไฟล์สำหรับเอกสารที่จะฝัง
      4. บันทึกไฟล์เอาต์พุตพร้อมเนื้อหาที่ผสม
   
    code:
      platform: "java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "เอกสารตัวอย่าง"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "คลิกเพื่อลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // ใช้แท็กนี้ในเทมเพลตของคุณเพื่อทำเครื่องหมายจุดที่จะแทรกเอกสาร
        // <<doc [doc_expression]>>

        // ตั้งค่าที่อยู่ไฟล์สำหรับเทมเพลตหลัก
        String template = "doc_template.xlsx";

        // ระบุที่อยู่ไฟล์สำหรับเอกสารที่คุณต้องการแทรก
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // บันทึกไฟล์สุดท้ายพร้อมเนื้อหาที่ถูกแทรก
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "เครื่องมือที่ก้าวหน้าสำหรับการรวมเอกสาร"
  description: "ด้วย GroupDocs.Assembly for Java การฝังเอกสารเป็นเรื่องที่ตรงไปตรงมาและปรับแต่งได้ ไม่ว่าไฟล์ประเภทใดก็ตาม ทำให้คุณได้ผลลัพธ์ที่เรียบร้อยและสม่ำเสมอในโครงการของคุณ"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "จุดเด่นของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานโดยใช้ข้อมูลธุรกิจ"
      content: "กรอกเอกสารด้วยข้อมูลจากแหล่งต่างๆ เช่น JSON, XML หรือ CSV ได้อย่างรวดเร็วและเชื่อถือได้ ช่วยให้กระบวนการทำงานของคุณราบรื่น"

    # feature loop
    - title: "เพิ่มเนื้อหาภาพลงในเอกสาร"
      content: "GroupDocs.Assembly ช่วยให้คุณสามารถแทรกตาราง แผนภูมิ และรายการควบคู่ไปกับข้อความ ลิงก์ ไฮเปอร์ลิงก์ รูปภาพ และแม้กระทั่งบาร์โค้ดที่มีพลศาสตร์"

    # feature loop
    - title: "จัดวางข้อมูลอย่างแม่นยำ"
      content: "เทมเพลต LINQ ช่วยให้จัดตำแหน่งข้อมูลของคุณได้อย่างเที่ยงตรง จัดการกับองค์ประกอบที่ทำซ้ำเช่นอาร์เรย์ และใช้สไตล์ที่กำหนดเองได้อย่างง่ายดาย"

    # feature loop
    - title: "เข้ากันได้กับรูปแบบไฟล์หลากหลาย"
      content: "รวมเอกสารข้ามรูปแบบต่างๆ รวมถึง PDFs, HTML, ไฟล์ MS Office, และ OpenOffice เพื่อให้มั่นใจถึงความยืดหยุ่นสำหรับโครงการของคุณ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการแทรกรูปภาพเข้าไปในเอกสารด้วยโปรแกรม"
      content: |
        ตัวอย่างนี้แสดงวิธีการฝังรูปภาพลงในไฟล์ XLSX โดยใช้ GroupDocs.Assembly
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // เพิ่มแท็กแทนในไฟล์เทมเพลต
          // <<image [expression]>>

          // กำหนดที่อยู่ไฟล์เทมเพลต
          String template = "template.xlsx";

          // ระบุที่อยู่ไฟล์สำหรับรูปภาพ
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // เริ่มต้นอินสแตนซ์ของ DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกไฟล์ที่มีรูปภาพที่ถูกแทรก
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "คัดลอก"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "คลิกเพื่อลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.xlsx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "สำรวจฟีเจอร์ของ GroupDocs.Assembly ฟรี หรือขอใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลดจาก Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "เรียนรู้เกี่ยวกับการอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ความสามารถหลักในภาพรวม"
    exclude: "document"
    description: "ค้นพบคุณสมบัติที่หลากหลายที่ GroupDocs.Assembly มีเพื่อทำให้การฝังและรวมเอกสารเป็นไปอย่างมีประสิทธิภาพและไม่มีปัญหา"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รวมไฟล์ประเภทต่างๆ"
    exclude: "XLSX"
    description: "ด้วย Java คุณสามารถฝังและรวมเนื้อหาจากรูปแบบไฟล์มากกว่า 50 รูปแบบ ได้อย่างราบรื่นเพื่อสร้างผลลัพธ์ที่เป็นมืออาชีพ"
    items: 
          
        # format loop 1
        - name: "ฝังเอกสารใน PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ฝังเอกสารใน DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "ฝังเอกสารใน PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "ฝังเอกสารใน XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---