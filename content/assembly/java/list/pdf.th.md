



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: th
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "สร้างรายการในเอกสาร PDF ด้วย Java"
head_description: "ออกแบบและแทรกรายการที่มีข้อมูลแบบไดนามิกลงในเทมเพลต PDF ของคุณด้วย API GroupDocs.Assembly for Java."

############################# Header ############################
title: "เพิ่มรายการแบบไดนามิกลงในไฟล์ PDF ด้วย API Java ของเรา" 
description: "GroupDocs.Assembly for Java ให้เครื่องมือที่ยืดหยุ่นในการสร้างและแทรกข้อมูลที่มีความละเอียดสูงโดยตรงลงในเอกสาร PDF."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ลองใช้งานฟรี"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java คืออะไร?"
    link: "/assembly/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) ช่วยให้การออกแบบเอกสารมืออาชีพเป็นเรื่องง่ายโดยดึงข้อมูลจากหลายแหล่ง ใช้เพื่อสร้างรายการ ตาราง แผนภูมิ หรือข้อความ และวางองค์ประกอบเหล่านี้ในตำแหน่งที่ต้องการโดยใช้ฟีเจอร์ของเทมเพลตที่มีความก้าวหน้า มีการสนับสนุนรูปแบบมากกว่า 50 รูปแบบ รวมถึง PDF เอกสาร MS Office และอีเมล เพื่อช่วยในการอัตโนมัตและปรับปรุงกระบวนการทำงานของคุณ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการเพิ่มรายการที่ขับเคลื่อนด้วยข้อมูลในเอกสาร PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ช่วยให้คุณแทรกรายการที่มีข้อมูลอย่างรวดเร็วในเทมเพลต PDF ได้อย่างมีประสิทธิภาพและจัดระเบียบเนื้อหาได้ง่าย.
      
      1. ออกแบบเทมเพลตและระบุพื้นที่ว่างสำหรับรายการ (ไม่รองรับเทมเพลต PDF).
      2. ตั้งค่าเส้นทางไฟล์ไปยังเทมเพลต.
      3. ดึงข้อมูลจากรูปแบบที่สนับสนุน เช่น JSON หรือ XML.
      4. บันทึกเอกสารที่เสร็จสมบูรณ์พร้อมรายการที่แนบมาเป็น PDF.
   
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
        // เพิ่มแท็กนี้ในเทมเพลตของคุณที่ซึ่งควรมีการแสดงรายการ
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // กำหนดเส้นทางไฟล์ของเทมเพลต
        // ไม่รองรับเทมเพลต PDF ณ ขณะนี้.
        String template = "list_template.docx";

        // ดึงข้อมูลจากแหล่งที่เลือกของคุณ
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // บันทึกเอกสารพร้อมรายการที่ฝังอยู่
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารจากเทมเพลตโดยมีการรวมข้อมูล"
  description: "GroupDocs.Assembly for Java ทำให้การเพิ่มรายการแบบไดนามิก ตาราง แผนภูมิ และองค์ประกอบอื่นในเทมเพลตเอกสารเป็นเรื่องง่าย."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานจากข้อมูลหลากหลายแหล่ง"
      content: "ใช้ข้อมูลจากรูปแบบต่างๆ เช่น JSON, XML และ CSV เพื่อทำการเติมข้อมูลในรายการและองค์ประกอบอื่นๆ ได้อย่างมีประสิทธิภาพ."

    # feature loop
    - title: "เพิ่มรายการและแหล่งข้อมูลอื่นๆ อย่างไม่มีสะดุด"
      content: "GroupDocs.Assembly ช่วยให้สามารถฝังรายการ แผนภูมิ ตาราง และอื่นๆ ควบคู่ไปกับข้อความ รูปภาพ และลิงก์เพื่อสร้างเอกสารที่ดูน่าเชื่อถือ."

    # feature loop
    - title: "ควบคุมตำแหน่งการปรากฏของข้อมูลอย่างแม่นยำ"
      content: "เทมเพลตที่ใช้ LINQ ช่วยให้คุณกำหนดตำแหน่งสำหรับรายการและข้อมูลได้อย่างแม่นยำ ใช้ลูปเพื่อสร้างรายการที่ละเอียดอัตโนมัติและปรับใช้การจัดรูปแบบแบบกำหนดเอง."

    # feature loop
    - title: "รองรับรูปแบบเอกสารที่หลากหลาย"
      content: "สร้างหรือแก้ไขไฟล์ในรูปแบบต่างๆ เช่น MS Office, PDF, OpenOffice, HTML และอีเมล รวมเนื้อหาจากเอกสารหลายไฟล์ตามที่ต้องการ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการสร้างรายการโดยการเขียนโปรแกรม"
      content: |
        ตัวอย่างนี้แสดงวิธีการเพิ่มรายการแบบไดนามิกลงในแฟ้ม PDF โดยใช้ GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // เพิ่มแท็กพื้นที่ว่างในเทมเพลตของคุณสำหรับรายการ
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // ระบุเส้นทางไฟล์ไปยังเทมเพลตของคุณ
          // ไม่รองรับเทมเพลต PDF ณ ขณะนี้.
          String template = "numlist_template.docx";

          // ดึงข้อมูลที่ต้องการเพื่อนำเข้ารายการ
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // จัดเตรียมแหล่งข้อมูลพร้อมรายละเอียดที่จำเป็น
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // เริ่มต้น DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกเอกสารผลลัพธ์พร้อมรายการที่เสร็จสมบูรณ์
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "ค้นพบสิ่งที่ GroupDocs.Assembly สามารถทำได้"
    exclude: "list"
    description: "ออกแบบและสร้างเอกสารที่มีเนื้อหาที่ซับซ้อนได้อย่างง่ายดายด้วยเครื่องมือการรวมข้อมูลที่มีความก้าวหน้า."
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างเอกสารในรูปแบบต่างๆ"
    exclude: "PDF"
    description: "Java รองรับรูปแบบมากกว่า 50 รูปแบบ ทำให้คุณสร้างเอกสารที่มีโครงสร้างโดยการรวมข้อมูลและเทมเพลต."
    items: 
          
        # format loop 1
        - name: "สร้างรายการใน PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "สร้างรายการใน DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "สร้างรายการใน PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "สร้างรายการใน XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---