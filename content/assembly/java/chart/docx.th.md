



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: th
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "สร้างแผนภูมิในเอกสาร DOCX โดยใช้ Java"
head_description: "API GroupDocs.Assembly for Java อนุญาตให้นักพัฒนาสร้างและแทรกแผนภูมิหรือกราฟแบบไดนามิกลงในเอกสารได้อย่างราบรื่น โดยใช้ข้อมูลที่มีการอัปเดตแบบเรียลไทม์"

############################# Header ############################
title: "เพิ่มแผนภูมิในเอกสาร DOCX ด้วย API Java" 
description: "GroupDocs.Assembly for Java ช่วยให้ง่ายต่อการฝังแผนภูมิในเอกสาร DOCX โดยใช้ข้อมูลเรียลไทม์"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มต้นใช้งานฟรี"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "บทนำสู่ GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) เป็นโซลูชันที่หลากหลายสำหรับการสร้างเอกสารและรายงานโดยอัตโนมัติ ช่วยให้คุณสามารถเพิ่มแผนภูมิ ตาราง รายการ บาร์โค้ด และภาพลงในไฟล์ของคุณได้โดยตรง ด้วยเครื่องมือขั้นสูงสำหรับการจัดฟอร์แมตอย่างแม่นยำและการรวมข้อมูล แพลตฟอร์มนี้รองรับมากกว่า 50 รูปแบบ รวมถึง PDF ไฟล์ Microsoft Office และอีเมล

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการฝังแผนภูมิในเอกสาร DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ช่วยให้ง่ายต่อการแทรกแผนภูมิในเทมเพลต DOCX ในหลายรูปแบบ รวมถึงกราฟแท่ง แผนภูมิวงกลม และกราฟเส้น
      
      1. สร้างเทมเพลต DOCX พร้อมโดยใช้ตัวแทนสำหรับแผนภูมิ
      2. โหลดข้อมูลของคุณจากแหล่งข้อมูลที่เข้ากันได้
      3. ตั้งค่าแผนภูมิ เช่น ประเภท ป้ายชื่อ และสี
      4. บันทึกเอกสารที่มีแผนภูมิที่รวมอยู่
   
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
        // เพิ่มแท็กนี้ลงในเทมเพลตของคุณเพื่อรวมแผนภูมิ
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // ระบุเส้นทางไฟล์ไปยังเทมเพลตของคุณ
        String template = "chart_template.docx";

        // ดึงข้อมูลที่จำเป็นจากแหล่งข้อมูลของคุณ
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // บันทึกเอกสารสุดท้ายที่มีแผนภูมิฝังอยู่
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ฝังแผนภูมิแบบไดนามิกในเอกสารของคุณได้อย่างราบรื่น"
  description: "GroupDocs.Assembly for Java มอบวิธีการที่เหมาะสมในการสร้างเอกสารที่มีข้อมูลมากมายในรูปแบบที่นิยม ใช้เทมเพลตเพื่อนำเข้าแผนภูมิ ตาราง บาร์โค้ด รายการ ลิงก์ และภาพพร้อมการอัปเดตจากข้อมูลของคุณ"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Assembly"
  features:
    # feature loop
    - title: "แปลงข้อมูลเป็นแผนภูมิได้ง่าย"
      content: "ใช้ API เพื่อแปลงข้อมูลจาก JSON, XML, CSV หรือแหล่งข้อมูลอื่นเป็นแผนภูมิที่เรียบร้อยและเป็นมืออาชีพสำหรับเอกสารของคุณ"

    # feature loop
    - title: "สร้างเนื้อหาที่ชัดเจนและน่าสนใจ"
      content: "GroupDocs.Assembly รองรับรูปแบบการแสดงผลที่หลากหลายรวมถึงกราฟแท่ง แผนภูมิวงกลม และกราฟเส้น ซึ่งสามารถรวมกับตาราง บาร์โค้ด ภาพ และอื่นๆ เพื่อรายงานที่ดียิ่งขึ้น"

    # feature loop
    - title: "การจัดวางและการตกแต่งแผนภูมิที่ปรับแต่งได้"
      content: "ด้วยไวยกรณ์ที่ใช้ LINQ คุณสามารถสร้างและจัดตำแหน่งแผนภูมิในเอกสารได้แบบไดนามิก หมายถึงการปรับปรุงรูปแบบ สี และเค้าโครงตามความต้องการในการออกแบบของคุณ"

    # feature loop
    - title: "รองรับรูปแบบเอกสารหลายรูปแบบ"
      content: "สร้างเอกสารในรูปแบบเช่น MS Office, PDF, OpenOffice และ HTML แผนภูมิจะรวมเข้ากับรูปแบบใด ๆ ที่สนับสนุนเพื่อผลลัพธ์ระดับมืออาชีพ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "สร้างและฝังแผนภูมิแบบโปรแกรมmatically"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงวิธีการสร้างและฝังแผนภูมิในเอกสาร DOCX แบบโปรแกรมmatically
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // เตรียมเทมเพลตที่มีตัวแทนสำหรับแผนภูมิ
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // ระบุเส้นทางไฟล์ไปยังเทมเพลต
          String template = "table_template.docx";

          // โหลดข้อมูลจากแหล่งข้อมูลที่คุณเลือก
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // สร้างวัตถุข้อมูลที่มีข้อมูลที่เกี่ยวข้อง
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // กำหนดประเภทและรูปลักษณ์ของแผนภูมิ
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // เริ่มต้น DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // บันทึกเอกสารที่เสร็จสมบูรณ์พร้อมแผนภูมิที่ฝังอยู่
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "สำรวจความสามารถที่ทรงพลัง"
    exclude: "chart"
    description: "แพลตฟอร์มนี้ช่วยให้ขั้นตอนการออกแบบเอกสารที่เน้นข้อมูลและน่าดึงดูดตามความต้องการของคุณเป็นเรื่องง่าย"
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
    title: "สร้างรายงานที่ครอบคลุมในหลายรูปแบบ"
    exclude: "DOCX"
    description: "Java ช่วยให้คุณสร้างเอกสารที่มีแผนภูมิรวมอยู่ในรูปแบบไฟล์มากกว่า 50 รูปแบบ ทำให้การรวมเทมเพลตและข้อมูลทำได้อย่างราบรื่น"
    items: 
          
        # format loop 1
        - name: "แผนภูมิใน PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "แผนภูมิใน DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "เอกสาร XML เปิดของ Microsoft Word"
          
        # format loop 3
        - name: "แผนภูมิใน PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "การนำเสนอ XML เปิดของ PowerPoint"
          
        # format loop 4
        - name: "แผนภูมิใน XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "สเปรดชีต XML เปิดของ Microsoft Excel"


          

---