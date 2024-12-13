



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: vi
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Chèn một tài liệu vào tài liệu khác trong PDF bằng Java"
head_description: "Kết hợp các tệp PDF bằng Java. GroupDocs.Assembly đơn giản hóa quy trình hợp nhất tài liệu chỉ với một vài dòng mã."

############################# Header ############################
title: "Nhúng nội dung vào tệp PDF một cách hiệu quả" 
description: "Sử dụng GroupDocs.Assembly for Java để chèn một tài liệu PDF vào tài liệu khác một cách liền mạch. Đạt được kết quả chính xác với các công cụ linh hoạt và đáng tin cậy."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nhận miễn phí"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java là gì?"
    link: "/assembly/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) là một giải pháp đa năng cho việc xử lý tài liệu. Nó cho phép bạn tích hợp một tài liệu vào tài liệu khác mà không gặp khó khăn, hỗ trợ hơn 50 định dạng như PDF và tệp MS Office. Tùy chỉnh đầu ra của bạn bằng cách hợp nhất, chỉnh sửa và tổ chức nội dung đúng theo ý muốn.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để chèn một tài liệu vào tệp PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) giúp việc nhúng một tài liệu PDF vào tài liệu khác trở nên đơn giản và có thể tùy chỉnh.
      
      1. Tạo một mẫu với các ký hiệu cho nội dung được nhúng (mẫu PDF hiện không được hỗ trợ).
      2. Chỉ định đường dẫn tệp cho mẫu.
      3. Cung cấp đường dẫn tệp cho tài liệu cần nhúng.
      4. Lưu tệp cuối cùng với nội dung đã hợp nhất dưới dạng PDF.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Tài liệu mẫu"
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
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Nhiều ví dụ hơn"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Sử dụng thẻ này trong mẫu của bạn để đánh dấu vị trí cho tài liệu được nhúng
        // <<doc [doc_expression]>>

        // Đặt đường dẫn tệp cho mẫu chính
        // Mẫu PDF hiện không được hỗ trợ.
        String template = "doc_template.docx";

        // Cung cấp đường dẫn đến tài liệu mà bạn muốn chèn
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Lưu tệp cuối cùng với nội dung đã nhúng
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Công cụ nâng cao để đơn giản hóa tích hợp tài liệu"
  description: "Với GroupDocs.Assembly for Java, việc nhúng tài liệu là đơn giản và có thể tùy chỉnh, bất kể loại tệp nào. Đạt được kết quả sạch sẽ và đồng nhất trên các dự án của bạn."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Điểm nổi bật của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo báo cáo sử dụng dữ liệu kinh doanh"
      content: "Điền vào tài liệu với dữ liệu từ các nguồn như JSON, XML hoặc CSV một cách nhanh chóng và đáng tin cậy, giúp tinh giản quy trình làm việc của bạn."

    # feature loop
    - title: "Cải thiện tài liệu với nội dung trực quan"
      content: "GroupDocs.Assembly cho phép bạn nhúng bảng, biểu đồ và danh sách bên cạnh văn bản, liên kết, hình ảnh và thậm chí mã vạch động."

    # feature loop
    - title: "Đặt dữ liệu chính xác nơi nó thuộc về"
      content: "Các mẫu LINQ giúp xác định vị trí dữ liệu của bạn một cách chính xác, xử lý các yếu tố lặp lại như mảng và áp dụng kiểu tùy chỉnh một cách dễ dàng."

    # feature loop
    - title: "Tương thích với nhiều định dạng tệp khác nhau"
      content: "Hợp nhất tài liệu từ các định dạng khác nhau, bao gồm PDF, HTML, tệp MS Office và OpenOffice, đảm bảo tính linh hoạt cho các dự án của bạn."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách nhúng một hình ảnh vào tài liệu lập trình"
      content: |
        Ví dụ này cho thấy cách nhúng một hình ảnh vào tệp PDF sử dụng GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Thêm một thẻ ký hiệu trong tệp mẫu
          // <<image [expression]>>

          // Xác định đường dẫn đến mẫu
          // Mẫu PDF hiện không được hỗ trợ.
          String template = "template.docx";

          // Chỉ định đường dẫn đến hình ảnh
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Khởi tạo thể hiện DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tệp với hình ảnh đã nhúng
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "Sao chép"
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
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.pdf"
        links:
          #  loop
          - title: "Nhiều ví dụ hơn"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Tài liệu"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu chưa?"
  description: "Khám phá các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống từ Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Tìm hiểu về giấy phép"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Các khả năng chính trong tầm nhìn"
    exclude: "document"
    description: "Khám phá các tính năng phong phú mà GroupDocs.Assembly cung cấp để làm cho việc nhúng và kết hợp tài liệu trở nên hiệu quả và không gặp rắc rối."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Hợp nhất giữa các loại tài liệu khác nhau"
    exclude: "PDF"
    description: "Với Java, bạn có thể nhúng và kết hợp nội dung qua hơn 50 định dạng tệp. Thêm tài liệu một cách liền mạch để tạo ra những kết quả chuyên nghiệp."
    items: 
          
        # format loop 1
        - name: "Nhúng tài liệu vào PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Nhúng tài liệu vào DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Nhúng tài liệu vào PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Nhúng tài liệu vào XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---