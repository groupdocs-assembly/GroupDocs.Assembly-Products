



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:03:59
draft: false
lang: vi
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Thêm mã vạch vào tệp PDF bằng JavaScript"
head_description: "Tạo và nhúng mã vạch vào tài liệu và email của bạn với API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Tạo mã vạch cho tệp PDF bằng Node.js" 
description: "Với GroupDocs.Assembly for Node.js via Java, bạn có thể tạo mã vạch một cách động, tùy chỉnh và nhúng chúng vào tài liệu PDF."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) cho phép bạn tạo tài liệu chuyên nghiệp bằng cách kết hợp dữ liệu từ nhiều nguồn. Thêm biểu đồ, bảng, danh sách, hình ảnh và mã vạch vào tệp của bạn một cách tiện lợi. Sử dụng các mẫu để tổ chức nội dung đúng vị trí. Hỗ trợ hơn 50 định dạng, bao gồm PDF, tài liệu Office và email.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước thêm mã vạch vào tệp PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) giúp nhúng mã vạch vào tài liệu PDF một cách dễ dàng. Nó hỗ trợ hơn 60 loại mã vạch, bao gồm các định dạng 1D và 2D.
      
      1. Thiết kế một mẫu với các vị trí mã vạch (mẫu PDF không được hỗ trợ).
      2. Lấy dữ liệu từ một nguồn tương thích.
      3. Đặt tùy chọn mã vạch như kích thước và độ phân giải.
      4. Xuất tài liệu với mã vạch dưới dạng tệp PDF.
   
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
        // Sử dụng thẻ này trong mẫu để bao gồm mã vạch trong tài liệu đầu ra
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Chỉ định đường dẫn đến tệp mẫu
        // Lưu ý: Mẫu PDF hiện chưa được hỗ trợ.
        const template = "barcode_template.docx";

        // Tải dữ liệu cần thiết từ nguồn của bạn
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Xuất tài liệu với mã vạch dưới dạng tệp PDF.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Tạo tài liệu với mẫu dữ liệu động"
  description: "Với GroupDocs.Assembly for Node.js via Java, bạn có thể tạo các tệp chuyên nghiệp ở các định dạng phổ biến bằng cách nhúng liền mạch biểu đồ, bảng, danh sách, liên kết, hình ảnh và mã vạch."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Xây dựng báo cáo với dữ liệu kinh doanh"
      content: "Sử dụng API để nhanh chóng và chính xác làm đầy các mẫu bằng dữ liệu từ các định dạng như JSON, XML và CSV."

    # feature loop
    - title: "Thêm các yếu tố hình ảnh"
      content: "GroupDocs.Assembly hỗ trợ việc chèn các yếu tố như biểu đồ, bảng, danh sách, văn bản, liên kết, hình ảnh và mã vạch theo thời gian thực."

    # feature loop
    - title: "Kiểm soát vị trí dữ liệu"
      content: "Với các mẫu dựa trên LINQ, bạn có thể định vị chính xác dữ liệu, lặp qua các mảng và áp dụng định dạng tùy chỉnh một cách lập trình."

    # feature loop
    - title: "Tương thích với nhiều định dạng"
      content: "Làm việc với các tệp như tài liệu MS Office, PDF, HTML, tệp OpenOffice và email. Kết hợp nhiều tài liệu khi cần thiết."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ví dụ: Tạo mã vạch một cách lập trình"
      content: |
        Ví dụ này minh họa cách tạo và chèn mã vạch vào tài liệu PDF một cách lập trình.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Thiết kế một mẫu với một vị trí mã vạch
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Chỉ định đường dẫn đến tệp mẫu
          // Lưu ý: Mẫu PDF hiện chưa được hỗ trợ.
          const template = "barcode_template.docx";

          // Lấy dữ liệu từ nguồn của bạn
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Tạo một đối tượng nguồn dữ liệu với các chi tiết cần thiết
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Khởi tạo một thể hiện của DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Thiết lập cấu hình mã vạch
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Lưu tài liệu với mã vạch đã bao gồm
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "Khám phá các tính năng chính"
    exclude: "barcode"
    description: "Đơn giản hóa quy trình xử lý tài liệu với các công cụ và khả năng tự động hóa tiên tiến."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Các định dạng tệp được hỗ trợ cho việc tạo báo cáo"
    exclude: "PDF"
    description: "Node.js via Java xử lý hơn 50 loại tệp, giúp đơn giản hóa việc kết hợp dữ liệu và xử lý mẫu để đạt được kết quả chất lượng cao."
    items: 
          
        # format loop 1
        - name: "Thêm mã vạch vào PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm mã vạch vào DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Thêm mã vạch vào PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Thêm mã vạch vào XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---