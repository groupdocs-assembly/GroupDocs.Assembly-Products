



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:05
draft: false
lang: vi
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Chèn Bảng vào Tài liệu PDF với JavaScript"
head_description: "Sử dụng GroupDocs.Assembly for Node.js via Java để nhanh chóng chèn bảng vào tài liệu hoặc email, lấy dữ liệu từ nhiều nguồn khác nhau."

############################# Header ############################
title: "Thêm Bảng vào Tập tin PDF một cách Nhanh Chóng với Node.js" 
description: "Với GroupDocs.Assembly for Node.js via Java, việc điền bảng vào tài liệu PDF trở nên đơn giản, sử dụng dữ liệu từ nhiều nguồn khác nhau."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt Đầu Dùng Thử Miễn Phí"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới Thiệu về GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) là một công cụ mạnh mẽ để tự động hóa việc tạo tài liệu. Nó cho phép bạn dễ dàng chèn bảng, biểu đồ, danh sách và hình ảnh vào các mẫu, với vị trí nội dung chính xác. Hỗ trợ trên 50 định dạng tệp, bao gồm PDF, Word và email, nó giúp tối ưu hóa quá trình tạo báo cáo và các tác vụ khác.

############################# Steps ############################
steps:
    enable: true
    title: "Cách Thêm Dữ Liệu vào Một Bảng trong PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) cho phép bạn nhanh chóng điền các mẫu bảng cho tệp PDF sử dụng các nguồn dữ liệu động.
      
      1. Tạo một mẫu với các vị trí cho bảng (các mẫu PDF hiện tại không được hỗ trợ).
      2. Tải dữ liệu từ một nguồn được hỗ trợ như JSON hoặc CSV.
      3. Sắp xếp và định dạng dữ liệu theo nhu cầu.
      4. Xuất tài liệu với bảng đã điền dưới dạng tệp PDF.
   
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
        // Bao gồm các thẻ này trong các vị trí hàng bảng của mẫu của bạn
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Chỉ định đường dẫn tệp mẫu
        // Các mẫu PDF hiện tại không được hỗ trợ.
        const template = "table_template.docx";

        // Tải dữ liệu từ nguồn đã chọn
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Lưu tài liệu cuối cùng với bảng đã hoàn tất
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Thêm Bảng Dựa trên Dữ Liệu vào Tài Liệu một cách Đơn Giản"
  description: "GroupDocs.Assembly for Node.js via Java cho phép người dùng tự động tạo bảng, đồng thời chèn biểu đồ, hình ảnh và danh sách bằng các quy trình dựa trên mẫu."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Các Tính Năng Nổi Bật của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo Bảng từ Dữ Liệu Có Cấu Trúc"
      content: "Lấy dữ liệu từ JSON, XML, CSV và các định dạng khác để tự động điền bảng tài liệu."

    # feature loop
    - title: "Tạo Nội Dung Hình Ảnh Chuyên Nghiệp"
      content: "Sử dụng GroupDocs.Assembly để thiết kế bảng, biểu đồ và danh sách chuyên nghiệp, và để thêm liên kết, hình ảnh và văn bản cho ngoại hình tài liệu tinh tế."

    # feature loop
    - title: "Cách Đặt Nội Dung Bảng Động"
      content: "Thêm hàng và cột một cách lập trình qua các mẫu dựa trên LINQ, và tùy chỉnh các kiểu như phông chữ, màu sắc, và căn chỉnh."

    # feature loop
    - title: "Hoạt Động Mượt Mà Trên Nhiều Định Dạng"
      content: "Dễ dàng tạo hoặc chỉnh sửa bảng trong MS Office, OpenOffice, PDF, HTML, và các định dạng khác, gộp chúng vào các tệp khi cần."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách Điền Bảng Qua Lập Trình"
      content: |
        Ví dụ này minh họa việc điền một bảng trong tài liệu PDF với dữ liệu từ một nguồn bên ngoài.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Thiết kế một mẫu với các vị trí cho bảng
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Chỉ định đường dẫn tệp đến mẫu
          // Các mẫu PDF hiện tại không được hỗ trợ.
          const template = "table_template.docx";

          // Tải dữ liệu cần thiết từ nguồn của bạn
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Sắp xếp dữ liệu vào cấu trúc cần thiết
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Khởi tạo DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Lưu tài liệu đầu ra với bảng đã hoàn tất
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    title: "Các Tính Năng Chính Nổi Bật"
    exclude: "table"
    description: "API của chúng tôi tự động hóa việc tạo bảng và nâng cao quy trình tạo tài liệu với các công cụ và mẫu đa dạng."
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
    title: "Tạo Bảng Trong Nhiều Định Dạng Khác Nhau"
    exclude: "PDF"
    description: "Với Node.js via Java, bạn có thể điền dữ liệu vào các mẫu và tạo các bảng toàn diện trên hơn 50 loại tệp được hỗ trợ."
    items: 
          
        # format loop 1
        - name: "Thêm bảng vào PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm bảng vào DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Thêm bảng vào PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Thêm bảng vào XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---