



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: th
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ฝังบาร์โค้ดในไฟล์ DOCX ด้วย Java"
head_description: "API GroupDocs.Assembly for Java ทำให้การสร้างและแทรกภาพบาร์โค้ดในเอกสารและอีเมลของคุณเป็นเรื่องง่ายในเวลาจริง."

############################# Header ############################
title: "สร้างบาร์โค้ดสำหรับไฟล์ DOCX ด้วย API Java ของเรา" 
description: "GroupDocs.Assembly for Java ให้เครื่องมือที่ครอบคลุมในการสร้าง ปรับแต่ง และฝังบาร์โค้ดในไฟล์ DOCX ได้อย่างมีประสิทธิภาพ."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดทันที"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java คืออะไร?"
    link: "/assembly/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) ช่วยให้คุณสร้างและปรับแต่งเอกสารโดยการเพิ่มข้อมูลจากหลายแหล่ง. แทรกข้อความ ตัวเลข แผนภูมิ ตาราง รายการ รูปภาพ และบาร์โค้ด. ใช้เทมเพลตขั้นสูงเพื่อให้ข้อมูลแสดงผลตามที่คุณต้องการ. รองรับรูปแบบมากกว่า 50 รูปแบบ รวมถึง PDF, เอกสาร Office และอีเมล.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีฝังบาร์โค้ดในเอกสาร DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ช่วยให้คุณแทรกบาร์โค้ดในรูปแบบที่ได้รับความนิยม เช่น เทมเพลต DOCX รองรับประเภทบาร์โค้ดมากกว่า 60 ประเภท รวมถึงบาร์โค้ด 1D และ 2D.
      
      1. ตั้งค่าเทมเพลต DOCX พร้อมเครื่องหมายบาร์โค้ด.
      2. ดึงข้อมูลจากแหล่งข้อมูลที่รองรับ.
      3. ปรับแต่งการตั้งค่าบาร์โค้ด เช่น ขนาดและความละเอียด.
      4. บันทึกเอกสารพร้อมบาร์โค้ดที่ฝังอยู่.
   
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
        // ใช้แท็กนี้ในเทมเพลตของคุณเพื่อสร้างบาร์โค้ดในเอกสารที่ส่งออก
        // <<barcode [barcode_expression] -barcode_type>>

        // ตั้งค่าเส้นทางไฟล์สำหรับเทมเพลต
        String template = "barcode_template.docx";

        // ดึงข้อมูลจากแหล่งข้อมูลของคุณ
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // บันทึกเอกสารที่ปรับปรุงพร้อมบาร์โค้ด
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "สร้างเอกสารโดยใช้เทมเพลตที่ขับเคลื่อนด้วยข้อมูล"
  description: "GroupDocs.Assembly for Java ทำให้การสร้างเอกสารง่ายขึ้นในไฟล์ประเภทยอดนิยม. ใช้เทมเพลตเพื่อเพิ่มแผนภูมิ ตาราง รายการ ลิงก์ รูปภาพ และบาร์โค้ดได้อย่างราบรื่น."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "ฟีเจอร์ของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "สร้างรายงานโดยใช้ข้อมูลธุรกิจ"
      content: "API จะเติมเอกสารด้วยข้อมูลจากรูปแบบต่างๆ เช่น JSON, XML และ CSV อย่างมีประสิทธิภาพและแม่นยำ."

    # feature loop
    - title: "แสดงข้อมูลด้วยองค์ประกอบในตัว"
      content: "GroupDocs.Assembly รองรับองค์ประกอบพื้นฐาน เช่น ตาราง แผนภูมิ และรายการ รวมถึงข้อความ ลิงก์ รูปภาพ และการสร้างบาร์โค้ดในเวลาจริง."

    # feature loop
    - title: "แทรกข้อมูลในที่ที่คุณต้องการ"
      content: "ด้วยเทมเพลตที่ใช้ LINQ คุณสามารถวางข้อมูลได้อย่างแม่นยำ ใช้ลูปเพื่อเพิ่มอาร์เรย์ และปรับแต่งรูปแบบเช่นสีได้ทางโปรแกรม."

    # feature loop
    - title: "รองรับความเข้ากันได้กว้างกับประเภทไฟล์"
      content: "จัดการไฟล์ต่างๆ เช่น เอกสาร MS Office, PDF, HTML, OpenOffice และอีเมล. คุณยังสามารถรวมเอกสารหนึ่งเข้าไปในอีกเอกสารหนึ่งได้."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีสร้างบาร์โค้ดแบบไดนามิก"
      content: |
        ในตัวอย่างนี้จะแสดงวิธีการสร้างและเพิ่มบาร์โค้ดไปยังเอกสาร DOCX แบบไดนามิก.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // เตรียมเทมเพลตที่มีช่องว่างสำหรับบาร์โค้ด
          // <<barcode [barcode_expression] -barcode_type>>

          // ตั้งค่าเส้นทางไปยังไฟล์เทมเพลตของคุณ
          String template = "barcode_template.docx";

          // โหลดข้อมูลจากแหล่งข้อมูลเฉพาะ
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // สร้างวัตถุแหล่งข้อมูลด้วยข้อมูลที่จำเป็น
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // สร้างอินสแตนซ์ของ DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // ปรับแต่งการตั้งค่าบาร์โค้ด
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // บันทึกเอกสารที่ปรับปรุงพร้อมบาร์โค้ด
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    title: "ค้นพบฟีเจอร์หลัก"
    exclude: "barcode"
    description: "แพลตฟอร์มของเราทำให้การจัดการเอกสารธุรกิจง่ายขึ้นด้วยเครื่องมือและการทำงานอัตโนมัติที่มีพลัง."
    items: 
          
        # operation loop 1
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "สร้างและเพิ่มบาร์โค้ดให้กับเอกสารอย่างไดนามิก"

        # operation loop 2
        - name: "แสดงข้อมูลด้วยแผนภูมิ"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "เติมข้อมูลให้กับประเภทของแผนภูมิต่างๆ"

        # operation loop 3
        - name: "รวมเอกสาร"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "รวมเนื้อหาของเอกสารหนึ่งเข้ากับอีกเอกสารหนึ่ง"

        # operation loop 4
        - name: "แสดงข้อมูลด้วยรายการ"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "สร้างรายการในเอกสารโดยใช้ข้อมูลเฉพาะ"

        # operation loop 5
        - name: "จัดระเบียบข้อมูลในตาราง"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "ดึงข้อมูลจากแหล่งใดๆ และเติมลงในตาราง"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้างรายงานในรูปแบบต่างๆ"
    exclude: "DOCX"
    description: "Java รองรับไฟล์มากกว่า 50 ประเภท, ช่วยให้การรวมข้อมูลและการประมวลผลเทมเพลตเป็นเรื่องง่ายสำหรับผลลัพธ์ที่เป็นมืออาชีพ."
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดลงใน PDF"
          format: "PDF"
          link: "/assembly/java/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดลงใน DOCX"
          format: "DOCX"
          link: "/assembly/java/barcode/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดลงใน PPTX"
          format: "PPTX"
          link: "/assembly/java/barcode/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดลงใน XLSX"
          format: "XLSX"
          link: "/assembly/java/barcode/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---