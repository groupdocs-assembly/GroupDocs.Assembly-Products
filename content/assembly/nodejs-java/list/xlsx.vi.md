



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: vi
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tạo danh sách động trong XLSX bằng JavaScript"
head_description: "Thiết kế và chèn danh sách vào mẫu XLSX sử dụng API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Nhúng danh sách dựa trên dữ liệu vào tệp XLSX với Node.js" 
description: "GroupDocs.Assembly for Node.js via Java cung cấp công cụ mạnh mẽ để thêm danh sách linh hoạt, dựa trên dữ liệu vào tài liệu XLSX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu miễn phí"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) đơn giản hóa việc tạo tài liệu bằng cách kéo dữ liệu từ nhiều nguồn và nhúng nó vào các mẫu. Sử dụng nó để xây dựng danh sách, bảng biểu, biểu đồ và các phần tử khác, với các tùy chọn định vị và định dạng chính xác. Hỗ trợ hơn 50 định dạng, bao gồm PDF, MS Office và email, nó giúp tự động hóa quy trình tạo tài liệu của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để chèn danh sách vào tệp XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) giúp thêm danh sách chi tiết, dựa trên dữ liệu vào các mẫu XLSX của bạn.
      
      1. Tạo một mẫu XLSX và xác định các chỗ trống cho danh sách.
      2. Cung cấp đường dẫn tệp của mẫu.
      3. Tải dữ liệu từ các nguồn hỗ trợ như JSON hoặc XML.
      4. Lưu tài liệu với danh sách đã được tạo.
   
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
        // Đặt thẻ này trong mẫu của bạn để đánh dấu vị trí của danh sách
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Chỉ định đường dẫn tệp cho mẫu của bạn
        const template = "list_template.xlsx";

        // Lấy dữ liệu từ nguồn bạn muốn sử dụng
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Lưu tệp với danh sách đã nhúng
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Tạo tài liệu dễ dàng với dữ liệu tích hợp"
  description: "Với GroupDocs.Assembly for Node.js via Java, bạn có thể nhúng danh sách, bảng biểu, biểu đồ và các phần tử khác vào các mẫu, tiết kiệm thời gian và công sức."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Điểm nổi bật của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo báo cáo từ nhiều nguồn dữ liệu"
      content: "Nhập dữ liệu từ JSON, XML, CSV hoặc các định dạng khác để làm đầy danh sách và các thành phần khác một cách hiệu quả."

    # feature loop
    - title: "Thêm danh sách và các phần tử hình ảnh khác"
      content: "GroupDocs.Assembly cho phép bạn nhúng một cách liền mạch danh sách, bảng biểu, biểu đồ và nhiều hơn nữa bên cạnh văn bản, hình ảnh và liên kết để có kết quả tinh xảo."

    # feature loop
    - title: "Định vị và định dạng dữ liệu chính xác"
      content: "Các mẫu dựa trên LINQ cho phép bạn kiểm soát chính xác nơi danh sách và dữ liệu khác xuất hiện, sử dụng vòng lặp cho các mục lặp lại và tùy chỉnh kiểu dáng theo nhu cầu của bạn."

    # feature loop
    - title: "Hoạt động trên nhiều định dạng"
      content: "Tạo tài liệu ở các định dạng như MS Office, PDF, OpenOffice, HTML và email. Gộp nội dung từ nhiều nguồn vào một tệp duy nhất."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tạo danh sách trong một tài liệu một cách lập trình"
      content: |
        Ví dụ này minh họa cách thêm động một danh sách vào tài liệu XLSX bằng cách sử dụng GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Thêm một chỗ trống trong mẫu của bạn cho danh sách
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Chỉ định đường dẫn tệp của mẫu
          const template = "numlist_template.xlsx";

          // Tải dữ liệu để làm đầy danh sách
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Chuẩn bị nguồn dữ liệu với các chi tiết cần thiết
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Khởi tạo DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Lưu tài liệu cuối cùng với danh sách được bao gồm
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "Khám phá các tính năng của GroupDocs.Assembly"
    exclude: "list"
    description: "Thiết kế và tạo tài liệu phong phú dữ liệu một cách hiệu quả bằng cách sử dụng các công cụ tích hợp mạnh mẽ."
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
    title: "Tạo tài liệu ở nhiều định dạng"
    exclude: "XLSX"
    description: "Node.js via Java hỗ trợ hơn 50 định dạng tệp, giúp dễ dàng kết hợp các mẫu và dữ liệu vào kết quả chuyên nghiệp."
    items: 
          
        # format loop 1
        - name: "Tạo danh sách trong PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Tạo danh sách trong DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Tạo danh sách trong PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Tạo danh sách trong XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---