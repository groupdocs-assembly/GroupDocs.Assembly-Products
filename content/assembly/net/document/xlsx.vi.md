



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: vi
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Nhúng một tài liệu vào tài liệu khác trong XLSX với API C#"
head_description: "Kết hợp tài liệu XLSX bằng C#. Với GroupDocs.Assembly, kết hợp các tệp một cách liền mạch chỉ với vài bước."

############################# Header ############################
title: "Kết hợp tài liệu theo định dạng XLSX" 
description: "Với GroupDocs.Assembly for .NET, bạn có thể nhanh chóng nhúng một tài liệu XLSX vào tài liệu khác. API này cung cấp những công cụ mạnh mẽ cho việc kết hợp tài liệu chính xác."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET là gì?"
    link: "/assembly/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) là một công cụ mạnh mẽ cho việc biên soạn và thao tác tài liệu. Nó cho phép người dùng nhúng một tài liệu vào tài liệu khác, tạo điều kiện cho việc kết hợp nội dung một cách liền mạch. Với hỗ trợ cho hơn 50 định dạng - bao gồm PDF, tệp MS Office và nhiều hơn nữa - bạn có thể tổ chức, chỉnh sửa và tùy chỉnh đầu ra cuối cùng để đáp ứng yêu cầu của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Cách kết hợp một tài liệu vào tệp XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) cho phép bạn nhúng một tài liệu vào một tệp XLSX khác một cách dễ dàng. Kết hợp và tùy chỉnh nội dung một cách thuận lợi.
      
      1. Thiết kế một mẫu XLSX với các vị trí dành cho tài liệu nhúng.
      2. Xác định đường dẫn tệp cho mẫu.
      3. Xác định đường dẫn tệp của tài liệu cần nhúng.
      4. Lưu tệp cuối cùng với nội dung đã được nhúng.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Tài liệu mẫu"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Nhiều ví dụ hơn"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Thêm thẻ này vào mẫu của bạn để đánh dấu điểm chèn
        // <<doc [doc_expression]>>

        // Xác định đường dẫn tệp cho mẫu
        string template = "doc_template.xlsx";

        // Cung cấp đường dẫn của tài liệu cần nhúng
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // Lưu tài liệu đã được kết hợp
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Đơn giản hóa kết hợp tài liệu với các công cụ tiên tiến"
  description: "Thư viện GroupDocs.Assembly for .NET đơn giản hóa việc nhúng một tài liệu vào tài liệu khác, hỗ trợ nhiều định dạng tệp và cung cấp tùy chỉnh cho việc tích hợp liền mạch."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo báo cáo từ dữ liệu kinh doanh của bạn"
      content: "Tự động điền tài liệu với dữ liệu từ JSON, XML, CSV hoặc nguồn khác, đảm bảo quy trình làm việc chính xác và hiệu quả."

    # feature loop
    - title: "Làm phong phú tài liệu với các yếu tố trực quan"
      content: "GroupDocs.Assembly cho phép bạn bao gồm bảng, biểu đồ và danh sách, cũng như văn bản, liên kết, hình ảnh và mã vạch được tạo động."

    # feature loop
    - title: "Đặt và định dạng dữ liệu một cách chính xác"
      content: "Các mẫu dựa trên LINQ giúp bạn kiểm soát vị trí dữ liệu, cho phép xử lý vòng lặp cho các mảng và cho phép định dạng như tùy chỉnh màu sắc."

    # feature loop
    - title: "Hỗ trợ nhiều định dạng tệp"
      content: "Nhúng tài liệu vào nhau một cách đơn giản qua các định dạng như MS Office, PDF, HTML, OpenOffice và nhiều hơn nữa."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách nhúng hình ảnh vào một tài liệu lập trình"
      content: |
        Ví dụ này minh họa cách chèn một hình ảnh vào tài liệu XLSX bằng GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Thêm một thẻ giữ chỗ trong mẫu của bạn
          // <<image [expression]>>

          // Xác định đường dẫn tệp cho mẫu
          string template = "template.xlsx";

          // Đặt đường dẫn tới tệp hình ảnh
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Khởi tạo một thể hiện của DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tài liệu với hình ảnh đã được nhúng
          asm.AssembleDocument(template, "result.xlsx", data);
          ```
        platform: "net"
        copy_title: "Sao chép"
        install:
          command: "dotnet add package GroupDocs.Assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Tài liệu"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu chưa?"
  description: "Khám phá các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống từ Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Tìm hiểu về giấy phép"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Khám phá các công cụ mạnh mẽ của chúng tôi"
    exclude: "document"
    description: "Khám phá các tính năng mà GroupDocs.Assembly cung cấp cho việc nhúng và kết hợp tài liệu một cách chính xác."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Kết hợp tài liệu trong các định dạng khác nhau"
    exclude: "XLSX"
    description: "Với API .NET, bạn có thể kết hợp tài liệu qua hơn 50 định dạng được hỗ trợ. Nhúng tệp hoặc các phần vào tài liệu cuối cùng của bạn một cách dễ dàng."
    items: 
          
        # format loop 1
        - name: "Nhúng tài liệu vào PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Nhúng tài liệu vào DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Nhúng tài liệu vào PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Nhúng tài liệu vào XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---