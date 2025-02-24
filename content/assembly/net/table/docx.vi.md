



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: vi
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tạo bảng trong tài liệu DOCX với C#"
head_description: "API GroupDocs.Assembly for .NET cho phép các nhà phát triển dễ dàng thêm và điền bảng trong tài liệu và email bằng dữ liệu từ các nguồn động."

############################# Header ############################
title: "Tạo bảng dữ liệu trong tài liệu DOCX sử dụng API .NET của chúng tôi" 
description: "GroupDocs.Assembly for .NET giúp điền tự động các bảng trong tài liệu DOCX với dữ liệu từ nhiều nguồn khác nhau."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống phiên bản dùng thử miễn phí"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Tổng quan về GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) được xây dựng để tạo tài liệu và báo cáo bằng cách điền các mẫu với dữ liệu từ nhiều nguồn. Dễ dàng chèn dữ liệu có cấu trúc vào bảng, danh sách, và biểu đồ, hoặc nhúng hình ảnh một cách động. Cú pháp nâng cao đảm bảo việc đặt dữ liệu chính xác. Hỗ trợ hơn 50 định dạng, bao gồm PDF, tài liệu MS Office, và tệp email.

############################# Steps ############################
steps:
    enable: true
    title: "Cách điền một bảng trong tài liệu DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) cho phép bạn điền động các bảng trong các mẫu cho các định dạng như DOCX. Chèn dữ liệu từ nhiều nguồn khác nhau vào bảng của bạn.
      
      1. Tạo một mẫu DOCX với các chỗ trống cho bảng.
      2. Lấy dữ liệu từ bất kỳ nguồn nào được hỗ trợ.
      3. Lọc dữ liệu để chỉ bao gồm những thông tin cần thiết.
      4. Lưu tài liệu với bảng đã được điền.
   
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
        // Thêm các thẻ này vào hàng bảng của mẫu
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Đặt đường dẫn tệp cho mẫu
        string template = "table_template.docx";

        // Lấy dữ liệu từ một nguồn được hỗ trợ
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Lưu tài liệu với bảng đã được điền dữ liệu
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tạo tài liệu với bảng động"
  description: "GroupDocs.Assembly for .NET tối ưu hóa việc tạo tài liệu bằng cách tự động điền bảng và hỗ trợ các yếu tố bổ sung như biểu đồ, danh sách, và hình ảnh thông qua các mẫu và cú pháp nâng cao."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo báo cáo từ dữ liệu có cấu trúc"
      content: "API xử lý dữ liệu từ các nguồn như JSON, XML, và CSV để điền bảng trong các tài liệu văn phòng một cách hiệu quả và chính xác."

    # feature loop
    - title: "Hiển thị dữ liệu một cách trực quan"
      content: "GroupDocs.Assembly cho phép tạo các bảng, danh sách, và biểu đồ, cùng với việc nhúng văn bản, liên kết, và hình ảnh cho thiết kế tài liệu chuyên nghiệp."

    # feature loop
    - title: "Đặt dữ liệu bảng một cách chính xác"
      content: "Sử dụng cú pháp dựa trên LINQ để động thêm hàng và cột trong bảng. Tùy chỉnh kiểu dáng, bao gồm màu sắc và định dạng, bằng cách lập trình."

    # feature loop
    - title: "Hỗ trợ nhiều định dạng khác nhau"
      content: "Xử lý dễ dàng các định dạng tệp phổ biến như MS Office, OpenOffice, PDF, và HTML. Chèn các bảng được điền một cách liền mạch vào các loại tài liệu được hỗ trợ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách điền động một bảng dữ liệu"
      content: |
        Ví dụ này minh họa cách điền một bảng trong tài liệu DOCX bằng dữ liệu động.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Chuẩn bị một mẫu với một chỗ trống cho bảng
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Chỉ định đường dẫn tệp đến mẫu
          string template = "table_template.docx";

          // Lấy dữ liệu từ nguồn đã chọn của bạn
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Tạo một đối tượng nguồn dữ liệu với các dữ liệu cần thiết
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Khởi tạo DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tài liệu hoàn thành với bảng đã được điền
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    title: "Khám phá các tính năng chính"
    exclude: "table"
    description: "Giải pháp của chúng tôi đơn giản hóa việc tạo ra các tài liệu chuyên nghiệp với các bảng được điền động và các yếu tố bổ sung."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tạo báo cáo với bảng chi tiết"
    exclude: "DOCX"
    description: ".NET cho phép tạo ra các báo cáo toàn diện bằng cách điền các mẫu với bảng và các yếu tố dữ liệu khác trong hơn 50 định dạng được hỗ trợ."
    items: 
          
        # format loop 1
        - name: "Thêm bảng vào PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm bảng vào DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Thêm bảng vào PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Thêm bảng vào XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---