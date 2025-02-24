



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: vi
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Kết hợp Tài liệu trong XLSX với JavaScript"
head_description: "Kết hợp các tệp XLSX bằng JavaScript. GroupDocs.Assembly đơn giản hóa việc kết hợp tài liệu chỉ sau vài bước đơn giản."

############################# Header ############################
title: "Kết hợp Nội dung trong Các Tệp XLSX một cách Nhanh chóng" 
description: "Với GroupDocs.Assembly for Node.js via Java, việc tích hợp một tệp XLSX vào tệp khác diễn ra nhanh chóng và chính xác. Tận hưởng công cụ linh hoạt, đáng tin cậy cho việc kết hợp liền mạch."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Thử Miễn Phí"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tổng Quan về GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) cung cấp một cách mạnh mẽ để quản lý tài liệu. Kết hợp một tệp vào một tệp khác một cách dễ dàng trong khi hỗ trợ hơn 50 định dạng, như PDF và MS Office. Tùy chỉnh bố cục, chỉnh sửa nội dung và sắp xếp tài liệu theo đúng cách bạn cần.

############################# Steps ############################
steps:
    enable: true
    title: "Cách Kết Hợp một Tài Liệu vào một Tệp XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) giúp bạn chèn một tệp XLSX vào một tệp khác với các tùy chọn tùy biến.
      
      1. Thiết kế một mẫu XLSX với các chỗ trống cho nội dung.
      2. Đặt đường dẫn tệp cho mẫu.
      3. Cung cấp đường dẫn tệp cho tài liệu để kết hợp.
      4. Xuất tệp cuối cùng với nội dung đã kết hợp.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Tài liệu mẫu"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Nhiều ví dụ hơn"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Chèn thẻ này vào mẫu của bạn để xác định nơi tài liệu sẽ được nhúng
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Đặt đường dẫn tệp cho mẫu chính
        const template = "doc_template.xlsx";

        // Cung cấp đường dẫn cho tài liệu bạn muốn kết hợp
        const data 
            = new assemblyLib.DataSourceInfo("insert.xlsx", "doc_expression");

        // Lưu đầu ra cuối cùng với tài liệu đã nhúng
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Công Cụ Mạnh Mẽ cho Việc Tích Hợp Tài Liệu"
  description: "GroupDocs.Assembly for Node.js via Java giúp việc nhúng tệp qua các định dạng khác nhau trở nên dễ dàng và hoàn toàn tùy chỉnh. Đảm bảo mang lại kết quả nhất quán và chuyên nghiệp mỗi lần."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Các Tính Năng Nổi Bật của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo Báo Cáo với Dữ Liệu Kinh Doanh"
      content: "Kéo dữ liệu từ các nguồn JSON, XML hoặc CSV để tạo báo cáo và tài liệu toàn diện một cách nhanh chóng và chính xác."

    # feature loop
    - title: "Thêm Các Yếu Tố Hình Ảnh Đa Dạng"
      content: "GroupDocs.Assembly cho phép bạn bao gồm bảng, biểu đồ, danh sách, hình ảnh và mã vạch bên cạnh văn bản và liên kết."

    # feature loop
    - title: "Đặt Dữ Liệu Chính Xác"
      content: "Sử dụng các mẫu LINQ để định vị dữ liệu chính xác ở vị trí mà nó thuộc về, xử lý các mục lặp lại như mảng và tùy chỉnh kiểu dáng một cách dễ dàng."

    # feature loop
    - title: "Hoạt Động với Nhiều Định Dạng Khác Nhau"
      content: "Kết hợp nội dung liền mạch qua các định dạng như PDF, tệp MS Office, HTML và OpenOffice, cung cấp sự linh hoạt cho tất cả các dự án."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Nhúng Hình Ảnh vào Tài Liệu Qua Mã Lập Trình"
      content: |
        Ví dụ này minh họa cách chèn một hình ảnh vào tệp XLSX bằng cách sử dụng GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Thêm một chỗ trống trong mẫu cho hình ảnh
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Chỉ định đường dẫn đến tệp mẫu
          const template = "template.xlsx";

          // Đặt đường dẫn đến hình ảnh bạn muốn nhúng
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Khởi tạo đối tượng DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Lưu tài liệu với hình ảnh đã bao gồm
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Sao chép"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.xlsx"
        links:
          #  loop
          - title: "Nhiều ví dụ hơn"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Tài liệu"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu chưa?"
  description: "Khám phá các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống từ NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Tìm hiểu về giấy phép"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Các Tính Năng Cốt Lõi Tóm Tắt"
    exclude: "document"
    description: "Khám phá các công cụ toàn diện mà GroupDocs.Assembly cung cấp cho việc kết hợp tài liệu hiệu quả và liền mạch."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Kết Hợp Tài Liệu trong Nhiều Định Dạng"
    exclude: "XLSX"
    description: "Sử dụng Node.js via Java để kết hợp nội dung qua hơn 50 định dạng tệp, đảm bảo kết quả chuyên nghiệp và trau chuốt."
    items: 
          
        # format loop 1
        - name: "Nhúng tài liệu vào PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Nhúng tài liệu vào DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Nhúng tài liệu vào PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Nhúng tài liệu vào XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---