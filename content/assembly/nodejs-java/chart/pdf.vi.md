



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: vi
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Chèn Biểu Đồ vào Tập Tin PDF với JavaScript"
head_description: "Với GroupDocs.Assembly for Node.js via Java, các nhà phát triển có thể nhanh chóng tạo và nhúng biểu đồ động vào tài liệu sử dụng dữ liệu nguồn trực tiếp."

############################# Header ############################
title: "Thêm Biểu Đồ vào Tập Tin PDF Bằng Node.js" 
description: "GroupDocs.Assembly for Node.js via Java đơn giản hóa quy trình tích hợp biểu đồ vào tài liệu PDF với dữ liệu đầu vào thời gian thực."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt Đầu Miễn Phí Hôm Nay"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tổng Quan Về GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) là một giải pháp mạnh mẽ cho việc tạo tài liệu và báo cáo tự động. Thêm biểu đồ, bảng, hình ảnh, mã vạch và danh sách vào tập tin một cách chính xác. Nền tảng linh hoạt này hỗ trợ hơn 50 định dạng, bao gồm PDF, tài liệu Office và email.

############################# Steps ############################
steps:
    enable: true
    title: "Các Bước Thêm Một Biểu Đồ Vào Tài Liệu PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) giúp thêm biểu đồ vào tập tin PDF một cách dễ dàng. Chọn từ các loại biểu đồ như biểu đồ cột, biểu đồ đường hoặc biểu đồ tròn.
      
      1. Tạo một mẫu với các chỗ trống cho biểu đồ (mẫu PDF hiện không được hỗ trợ).
      2. Tải dữ liệu từ một nguồn hỗ trợ.
      3. Cấu hình các tùy chọn biểu đồ, bao gồm loại, màu sắc và nhãn.
      4. Lưu tài liệu với biểu đồ dưới dạng tệp PDF.
   
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
        // Bao gồm thẻ này trong mẫu của bạn để tạo biểu đồ
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Chỉ định đường dẫn đến tệp mẫu
        // Lưu ý: Mẫu PDF hiện không được hỗ trợ.
        const template = "chart_template.docx";

        // Trích xuất dữ liệu từ hệ thống nguồn của bạn
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Lưu tài liệu cuối cùng với biểu đồ đã nhúng
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Nhúng Biểu Đồ Một Cách Dễ Dàng Vào Tài Liệu Của Bạn"
  description: "GroupDocs.Assembly for Node.js via Java giúp tạo ra tài liệu đầy đủ tính năng trong các loại tập tin phổ biến. Sử dụng mẫu để thêm biểu đồ, bảng, mã vạch, danh sách, hình ảnh và nhiều hơn nữa với cập nhật dữ liệu thời gian thực."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Các Tính Năng Nổi Bật Của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Biến Dữ Liệu Thành Biểu Đồ Chuyên Nghiệp"
      content: "Chuyển đổi dữ liệu từ các nguồn như JSON, XML hoặc CSV thành biểu đồ chất lượng cao có thể được nhúng trực tiếp vào tài liệu."

    # feature loop
    - title: "Tạo Hình Ảnh Ấn Tượng"
      content: "Tạo các biểu đồ cột, biểu đồ tròn và biểu đồ đường hoạt động liền mạch với các yếu tố tài liệu khác như hình ảnh, bảng và mã vạch."

    # feature loop
    - title: "Phong Cách và Vị Trí Biểu Đồ Linh Hoạt"
      content: "Sử dụng mẫu LINQ để kiểm soát vị trí và kiểu dáng biểu đồ, bao gồm màu sắc, bố cục và nhãn, cho một buổi trình bày hoàn thiện."

    # feature loop
    - title: "Hỗ Trợ Nhiều Định Dạng Tập Tin"
      content: "Tạo tài liệu trong các định dạng như MS Office, PDF, OpenOffice và HTML, với biểu đồ được tích hợp hoàn hảo cho một kết thúc chuyên nghiệp."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tạo Và Nhúng Biểu Đồ Tự Động"
      content: |
        Ví dụ này minh họa cách để tạo và nhúng biểu đồ vào các tập tin PDF theo cách lập trình.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Thiết lập một mẫu với một chỗ trống cho biểu đồ
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Định nghĩa đường dẫn đến tệp mẫu
          // Lưu ý: Mẫu PDF hiện không được hỗ trợ.
          const template = "table_template.docx";

          // Lấy dữ liệu từ nguồn đã chọn
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Chuẩn bị một đối tượng dữ liệu chứa thông tin biểu đồ
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Chọn loại biểu đồ và tùy chỉnh hình thức của nó
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Khởi tạo DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Lưu tài liệu đã cập nhật với biểu đồ đã nhúng
          asm.assembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "Khám Phá Các Tính Năng Nâng Cao"
    exclude: "chart"
    description: "Nền tảng này đơn giản hóa việc tạo tài liệu với các công cụ được thiết kế cho trực quan hóa dữ liệu và tích hợp liền mạch."
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
    title: "Tạo Báo Cáo Trong Nhiều Định Dạng Tập Tin"
    exclude: "PDF"
    description: "Node.js via Java hỗ trợ hơn 50 định dạng, giúp kết hợp các mẫu với dữ liệu để sản xuất tài liệu hoàn hảo."
    items: 
          
        # format loop 1
        - name: "Biểu đồ trong PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Biểu đồ trong DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Biểu đồ trong PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Biểu đồ trong XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---