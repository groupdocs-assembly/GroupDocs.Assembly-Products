



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: th
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "เพิ่มตารางในเอกสาร PPTX โดยใช้ Java"
head_description: "ด้วย GroupDocs.Assembly for Java นักพัฒนาสามารถรวมตารางเข้ากับเอกสารและอีเมลได้อย่างรวดเร็ว โดยดึงข้อมูลจากแหล่งข้อมูลแบบไดนามิก"

############################# Header ############################
title: "เติมตารางในไฟล์ PPTX ด้วย API Java ของเรา" 
description: "GroupDocs.Assembly for Java ช่วยให้กระบวนการเติมตารางในเอกสาร PPTX ด้วยข้อมูลจากแหล่งข้อมูลต่างๆ เป็นเรื่องง่าย"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ขอทดลองใช้งานฟรี"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java คืออะไร?"
    link: "/assembly/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) เป็นเครื่องมือสำหรับสร้างเอกสารและรายงานโดยการแทรกข้อมูลลงในแม่แบบที่ออกแบบไว้ล่วงหน้าโดยอัตโนมัติ คุณสามารถเพิ่มตาราง รายการ แผนภูมิ และรูปภาพได้อย่างง่ายดาย คุณลักษณะที่ทันสมัยช่วยให้คุณวางเนื้อหาในเอกสารของคุณได้อย่างแม่นยำ รองรับไฟล์มากกว่า 50 ประเภท รวมถึง PDF, MS Office และรูปแบบอีเมล

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการแทรกข้อมูลลงในตาราง PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ช่วยให้คุณกรอกแม่แบบตารางสำหรับ PPTX และรูปแบบอื่น ๆ ใช้ข้อมูลไดนามิกจากแหล่งของคุณเพื่อสร้างตารางอย่างมีประสิทธิภาพ
      
      1. ตั้งค่าแม่แบบ PPTX พร้อมที่ว่างสำหรับแถวและคอลัมน์ของตาราง
      2. ดึงข้อมูลจากแหล่งข้อมูลที่รองรับ
      3. กรองหรือแปรรูปข้อมูลให้ตรงตามความต้องการของคุณ
      4. สร้างเอกสารสุดท้ายพร้อมตารางที่เสร็จสมบูรณ์
   
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
        // ใช้แท็กเหล่านี้ในที่เก็บแท็บในแถวของตารางภายในแม่แบบของคุณ
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // กำหนดเส้นทางไปยังไฟล์แม่แบบ
        String template = "table_template.pptx";

        // โหลดข้อมูลจากแหล่งที่คุณเลือก
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // บันทึกไฟล์ผลลัพธ์ที่มีการกรอกตาราง
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารที่มีตารางที่เต็มไปด้วยข้อมูล"
  description: "GroupDocs.Assembly for Java ทำให้การสร้างตารางในเอกสารของคุณเป็นเรื่องง่าย นอกจากนี้ยังสนับสนุนการเพิ่มองค์ประกอบเช่น แผนภูมิ รายการ และรูปภาพ โดยใช้แม่แบบ"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากหลายรูปแบบข้อมูล"
      content: "API ทำงานร่วมกับ JSON, XML, CSV และรูปแบบอื่นๆ ได้อย่างราบรื่นเพื่อตอบสนองความต้องการในการกรอกตารางในเอกสารของคุณด้วยข้อมูลที่จัดระเบียบ"

    # feature loop
    - title: "นำเสนอข้อมูลอย่างมีภาพลักษณ์"
      content: "GroupDocs.Assembly ช่วยให้คุณสร้างตาราง รายการ และแผนภูมิที่ดูเป็นมืออาชีพ รวมทั้งแทรกลิงก์ ข้อความ และรูปภาพ เพื่อให้มีรูปลักษณ์ที่เหมาะสม"

    # feature loop
    - title: "วางเนื้อหาตารางอย่างแม่นยำ"
      content: "ใช้ไวยากรณ์ที่ยืดหยุ่นตาม LINQ เพื่อเพิ่มแถวและคอลัมน์แบบไดนามิก ปรับแต่งลักษณะเช่น สไตล์ฟอนต์และสี ได้อย่างเป็นโปรแกรม"

    # feature loop
    - title: "เข้ากันได้กับหลายรูปแบบ"
      content: "ทำงานกับ MS Office, OpenOffice, PDF, HTML และอื่นๆ รวมตารางเข้ากับรูปแบบไฟล์ที่รองรับได้โดยไม่ยุ่งยาก"
      
  code_samples_ext:
    # code sample ext loop
    - title: "สร้างตารางที่มีข้อมูลโดยใช้วิธีการไดนามิก"
      content: |
        ตัวอย่างนี้แสดงวิธีการกรอกข้อมูลในตารางในเอกสาร PPTX โดยใช้ข้อมูลป้อนเข้าที่เป็นไดนามิก
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // ออกแบบแม่แบบที่มีที่ว่างสำหรับตาราง
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // ตั้งค่าที่ตั้งไฟล์แม่แบบ
          String template = "table_template.pptx";

          // โหลดข้อมูลจากแหล่งที่คุณต้องการ
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // เตรียมอ็อบเจ็กต์ข้อมูลที่มีฟิลด์ที่จำเป็น
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // สร้างอินสแตนซ์ของ DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกเอกสารที่มีการกรอกตาราง
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "ฟีเจอร์หลักในภาพรวม"
    exclude: "table"
    description: "API ของเราช่วยให้การสร้างเอกสารที่มีคุณภาพเป็นเรื่องง่ายโดยการอัตโนมัติการกรอกตารางพร้อมองค์ประกอบที่มีประสิทธิภาพอื่นๆ"
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างตารางที่มีรายละเอียดในรูปแบบต่างๆ"
    exclude: "PPTX"
    description: "ด้วย Java คุณสามารถกรอกข้อมูลในแม่แบบและสร้างรายงานที่มีรายละเอียดในมากกว่า 50 ประเภทไฟล์"
    items: 
          
        # format loop 1
        - name: "เพิ่มตารางใน PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มตารางใน DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "เพิ่มตารางใน PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "เพิ่มตารางใน XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---