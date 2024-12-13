---
############################# Static ############################
layout: "family"
date:  2024-12-13T10:30:57
draft: false

product: "Assembly"
product_tag: "assembly"

lang: th

############################# Head ############################
head_title: "GroupDocs ภาษี .NET, Java APIs และแอปพลิเคชันการจัดการเอกสารออนไลน์"
head_description: "รับโซลูชันการทำเอกสารและรายงานแบบครบวงจรสำหรับแอปพลิเคชัน .NET และ Java สร้างเอกสารทั่วไปจากเทมเพลตและข้อมูลที่กำหนดเอง"

############################# Header ############################
title: "โซลูชันการทำเอกสารและรายงาน"
description:  |
  สร้างรายงานที่ละเอียดได้ด้วยเทมเพลตและแหล่งข้อมูลด้วยแอปพลิเคชันและ API แบบข้ามแพลตฟอร์มของเรา

  สร้างรายงานในรูปแบบต่างๆ เช่น Word, Excel, งานนำเสนอ และอีกมากมายโดยใช้เทมเพลตที่มีรูปร่างที่ปรับเปลี่ยนได้

  กรอกข้อมูลในกราฟ บาร์โค้ด ตาราง และองค์ประกอบอื่นๆ ด้วยข้อมูลจากแหล่งต่างๆ เช่น JSON, XML, CSV เป็นต้น

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "เลือกแพลตฟอร์มของคุณ"
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Assembly รองรับระบบปฏิบัติการและเฟรมเวิร์กต่อไปนี้:"
  details_link_title: "เรียนรู้เพิ่มเติม"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "ฟีเจอร์หลักของ GroupDocs.Assembly"
  description: "โซลูชันนี้ช่วยให้คุณสร้างรายงานในรูปแบบเอกสารยอดนิยมที่กรอกข้อมูลอัตโนมัติด้วยข้อมูลทางธุรกิจของคุณ ปรับกระบวนการสร้างเอกสารของคุณอัตโนมัติอย่างมีประสิทธิภาพ"

  items:
    # items loop
    - icon: "additional"
      title: "กรอกเทมเพลตด้วยข้อมูล"
      content: "กรอกรายงานโดยใช้ข้อมูลจากแหล่งข้อมูลที่รองรับ"

    # items loop
    - icon: "manipulate"
      title: "การทำเครื่องหมายที่ยืดหยุ่น"
      content: "เพิ่มข้อมูลลงในเอกสารในวิธีที่ปรับแต่งได้"

    # items loop
    - icon: "structure"
      title: "ฟีเจอร์เอกสารพื้นฐาน"
      content: "แสดงข้อมูลโดยใช้ตาราง กราฟ และบาร์โค้ด"

    # items loop
    - icon: "merge"
      title: "รูปแบบที่เป็นที่นิยมทั้งหมด"
      content: "รองรับรูปแบบเอกสารที่ใช้กันทั่วไปทั้งหมด"

############################# Code samples ############################
code_samples:
  enable: true
  title: "สร้างรายงานที่ปรับแต่งได้ดี"
  description: "GroupDocs.Assembly ตัวอย่างโค้ด"
  items:
    # code sample loop
    - title: "การใช้บาร์โค้ดที่สร้างขึ้น"
      content: |
       GroupDocs.Assembly อนุญาตให้มีการทำเครื่องหมายบาร์โค้ดในเทมเพลตรายงาน เมื่อสร้างรายงาน บาร์โค้ดจะถูกสร้างขึ้นตามเครื่องหมายและข้อมูลที่ให้ กำหนดเส้นทางไปยังเทมเพลตที่มีข้อความ วัตถุข้อมูล และการทำเครื่องหมาย นอกจากนี้ ยังต้องระบุแหล่งข้อมูลเพื่อเติมข้อมูลของบาร์โค้ด
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // สร้างอินสแตนซ์ของคลาส DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //ระบุเส้นทางไปยังเทมเพลต
            var tmp_path = "barcode_template.docx";

            //ระบุเส้นทางสำหรับเอกสารผลลัพธ์
            var res_path = "result.docx";

            //สร้างอินสแตนซ์ของแหล่งข้อมูล
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //เรียก AssembleDocument เพื่อสร้างรายงาน
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // สร้างอินสแตนซ์ของคลาส DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //ระบุเส้นทางไปยังเทมเพลต
            String tmp_path = "barcode_template.docx";

            //ระบุเส้นทางสำหรับเอกสารผลลัพธ์
            String res_path = "result.docx";

            //สร้างอินสแตนซ์ของแหล่งข้อมูล
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // เรียก AssembleDocument เพื่อสร้างรายงาน
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "รองรับรูปแบบไฟล์ 50+ รูปแบบ"
  description: "GroupDocs.Assembly ทำงานร่วมกับไฟล์รูปแบบยอดนิยมเกือบทั้งหมด"

############################# Metrics ###############################
metrics:
  enable: true
  title: "สถิติผลิตภัณฑ์ของเรา"
  description: "สำรวจเมตริกผลิตภัณฑ์เพื่อตรวจสอบความก้าวหน้า ผลกระทบ และการเติบโตของเรา"

  items:
    # items loop
    - number: "50+"
      title: "รูปแบบที่รองรับ"
      content: "เรารองรับรูปแบบเอกสารที่ใช้กันมากกว่า 50 รูปแบบ"

    # items loop
    - number: "650k"
      title: "การดาวน์โหลด NuGet"
      content: "GroupDocs.Assembly สำหรับ .NET เป็นไลบรารีที่ได้รับความนิยมมากกว่า 650,000 ครั้งที่ทำการดาวน์โหลดจาก NuGet"

    # items loop
    - number: "18k"
      title: "การดาวน์โหลด Maven"
      content: "นักพัฒนา Java ได้ดาวน์โหลด GroupDocs.Assembly บน Maven มากกว่า 18,000 ครั้ง"

    # items loop
    - number: "150+"
      title: "ลูกค้าที่พอใจ"
      content: "ผลิตภัณฑ์ของเราได้รับความไว้วางใจจากนักพัฒนาทั่วไปและบริษัทชั้นนำจากทั่วโลกในการสร้างโซลูชันที่สร้างสรรค์"


############################# Customers ###############################
customers:
  enable: true
  title: "ลูกค้าที่พอใจของเรา"
  description: "ห้องสมุด GroupDocs ถูกใช้โดยแบรนด์ที่มีชื่อเสียงและเป็นที่เคารพนับถือมากที่สุดทั่วโลก"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ทดสอบฟีเจอร์ของ GroupDocs.Assembly ฟรีบนแพลตฟอร์มของคุณ"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "คำถามที่พบบ่อย"
  description: "เรียกดูคำถามที่พบบ่อยของเรา"

  items:
    # items loop
    - question: "GroupDocs.Assembly ต้องการไลบรารีภายนอกสำหรับการสร้างเอกสารหรือไม่?"
      answer: "ไม่, GroupDocs.Assembly ทำงานอย่างอิสระและไม่ต้องการไลบรารีของบุคคลที่สามเช่น Adobe Acrobat หรือ Microsoft Office"

    # items loop
    - question: "ฉันสามารถทดสอบฟีเจอร์ของ GroupDocs.Assembly ก่อนทำการซื้อได้หรือไม่?"
      answer: "ใช่, คุณสามารถ! GroupDocs.Assembly มีการทดลองใช้ฟรี ติดตั้งและสำรวจฟีเจอร์ของมัน รุ่นทดลองใช้ฟรีจะเพิ่ม 'ป้ายการทดลอง' ลงในเอกสารของคุณและประมวลผลเฉพาะหน้าแรก 3 หน้า สำหรับประสบการณ์ที่สมบูรณ์แบบ ได้รับใบอนุญาตชั่วคราวฟรี 30 วันเพื่อเข้าถึงฟีเจอร์ทั้งหมด รายละเอียดเพิ่มเติมมีอยู่ภายใต้ [ใบอนุญาตชั่วคราว](https://purchase.groupdocs.com/temporary-license/)"

    # items loop
    - question: "มีประเภทใบอนุญาตใดบ้าง?"
      answer: "กำลังมองหาใบอนุญาต GroupDocs.Assembly หรือไม่? เรามีตัวเลือกที่หลากหลายให้เหมาะสมกับความต้องการของคุณ เลือกตามขนาดทีม สถานที่ติดตั้ง (สำนักงานเดียวหรือระยะไกล) และคุณต้องการแบ่งปัน SDK/API กับลูกค้าเพื่อทำการแจกจ่ายหรือไม่หรือไม่ นอกจากนี้ยังเลือกใบอนุญาตการใช้งานรายเดือนที่มีแผนการจับเมตริก—จ่ายเฉพาะสำหรับสิ่งที่คุณใช้ ค้นหาตัวเลือกที่ดีที่สุดสำหรับคุณที่ [ราคา](https://purchase.groupdocs.com/pricing/assembly/net/)"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Assembly API แบบ Low-Code"
  description: "สร้างเอกสารโดยใช้แอปพลิเคชันของคุณผ่าน REST API ที่ใช้คลาวด์ของเรา"
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "ใช้ cURL RESTful API เพื่อเพิ่มข้อมูลลงใน Word, Excel, PowerPoint และเทมเพลตอื่นๆ อีกมากมาย"
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "เพิ่มประสิทธิภาพแอปพลิเคชัน .NET ของคุณโดยการสร้างรายงานผ่าน Cloud SDK แสดงข้อมูลธุรกิจในรูปแบบที่กำหนดเอง"
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK มีตัวเลือกต่างๆ สำหรับแอปพลิเคชัน Java ในการสร้างเอกสารประเภทต่างๆ"
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Assembly แอปพลิเคชันเว็บ"
  description: "GroupDocs.Assembly มีแอปพลิเคชันเว็บฟรีสำหรับการสร้างเอกสาร คุณสามารถประมวลผลไฟล์รูปแบบยอดนิยมกว่า 50 รูปแบบได้โดยตรงในเบราว์เซอร์ของคุณ ฟรี"

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "สร้างรายงานใน Excel, Word, PowerPoint และไฟล์ประเภทอื่นๆ โดยตรงจากเบราว์เซอร์ของคุณ"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "สร้างเอกสาร Microsoft Word จากเทมเพลตและแหล่งข้อมูล"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "อัปโหลดเทมเพลตและแหล่งข้อมูลเพื่อสร้างรายงาน Excel ฟรี"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---