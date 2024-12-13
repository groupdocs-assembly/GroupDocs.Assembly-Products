



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: vi
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tạo danh sách trong tài liệu PDF bằng C#"
head_description: "API GroupDocs.Assembly for .NET cho phép các nhà phát triển tạo và nhúng danh sách đầy dữ liệu vào tài liệu và mẫu một cách linh hoạt."

############################# Header ############################
title: "Thêm danh sách dữ liệu vào tài liệu PDF bằng API .NET của chúng tôi" 
description: "GroupDocs.Assembly for .NET cung cấp các công cụ mạnh mẽ để tạo và nhúng danh sách vào tài liệu PDF một cách linh hoạt."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống Bản dùng thử miễn phí"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Tổng quan về GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) được thiết kế để đơn giản hóa việc tạo ra tài liệu và báo cáo bằng cách tích hợp liền mạch dữ liệu từ nhiều nguồn khác nhau. Điền dữ liệu vào các mẫu với danh sách, biểu đồ, bảng, mã vạch hoặc văn bản, và đặt nội dung một cách chính xác sử dụng đánh dấu nâng cao. Với hỗ trợ hơn 50 định dạng—bao gồm PDF, tệp MS Office và email—nó lý tưởng cho việc tự động hóa quy trình công việc tài liệu.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để thêm danh sách dữ liệu vào tài liệu PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) giúp đơn giản hóa việc thêm danh sách dựa trên dữ liệu vào các mẫu PDF. Tạo và tùy chỉnh danh sách một cách linh hoạt.
      
      1. Tạo một mẫu với các vị trí xác định cho danh sách (tài liệu mẫu PDF hiện không được hỗ trợ).
      2. Đặt đường dẫn tới mẫu.
      3. Lấy dữ liệu từ các nguồn hỗ trợ như JSON hoặc XML.
      4. Xuất tài liệu đã hoàn thành với danh sách dưới dạng tệp PDF.
   
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
        // Thêm thẻ này vào mẫu của bạn để đánh dấu nơi danh sách sẽ xuất hiện
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Chỉ định đường dẫn đến tệp mẫu
        // Hỗ trợ dành cho mẫu PDF hiện không có sẵn.
        string template = "list_template.docx";

        // Lấy dữ liệu từ nguồn bạn chọn
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Lưu tài liệu với danh sách đã tạo
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tạo tài liệu bằng cách điền dữ liệu có cấu trúc vào mẫu"
  description: "GroupDocs.Assembly for .NET đơn giản hóa việc xây dựng tài liệu dựa trên dữ liệu. Thêm danh sách, bảng, mã vạch, biểu đồ, hình ảnh và các yếu tố khác một cách linh hoạt với các mẫu nâng cao."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Các tính năng của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo báo cáo từ dữ liệu doanh nghiệp"
      content: "API này điền dữ liệu vào tài liệu ở các định dạng phổ biến sử dụng dữ liệu từ các nguồn như JSON, XML, CSV, v.v. với độ chính xác và hiệu quả cao."

    # feature loop
    - title: "Sử dụng danh sách và các yếu tố khác để trình bày dữ liệu"
      content: "GroupDocs.Assembly cho phép bạn nhúng danh sách, bảng, và biểu đồ cùng với văn bản, mã vạch, hyperlink, và hình ảnh để tạo ra tài liệu có cấu trúc tốt."

    # feature loop
    - title: "Chèn dữ liệu chính xác nơi cần thiết"
      content: "Tận dụng cú pháp dựa trên LINQ để định vị danh sách và các yếu tố dữ liệu khác một cách chính xác. Sử dụng vòng lặp để điền danh sách một cách linh hoạt và áp dụng định dạng tùy chỉnh một cách lập trình."

    # feature loop
    - title: "Hỗ trợ nhiều định dạng tài liệu"
      content: "Tạo và quản lý tài liệu ở nhiều định dạng như MS Office, OpenOffice, PDF, HTML, và các tệp email. Tích hợp nhiều tài liệu vào một tài liệu duy nhất một cách đơn giản."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách tạo danh sách động"
      content: |
        Ví dụ này minh họa cách nhúng một danh sách được tạo động vào một tài liệu PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Thêm một thẻ chỗ để danh sách vào mẫu của bạn
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Chỉ định đường dẫn đến tệp mẫu
          // Hỗ trợ dành cho mẫu PDF hiện không có sẵn.
          string template = "numlist_template.docx";

          // Lấy dữ liệu để điền vào danh sách
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Tạo một đối tượng nguồn dữ liệu với thông tin cần thiết
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Khởi tạo DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tài liệu cuối cùng với danh sách đã tạo
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "Khám phá các khả năng chính"
    exclude: "list"
    description: "Nền tảng của chúng tôi được xây dựng để đơn giản hóa việc tạo ra và tích hợp nội dung tài liệu dựa trên dữ liệu."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tạo tài liệu có cấu trúc trong các định dạng phổ biến"
    exclude: "PDF"
    description: ".NET hỗ trợ hơn 50 định dạng, cho phép bạn tích hợp dữ liệu và mẫu một cách liền mạch để tạo ra kết quả có cấu trúc và hoàn thiện."
    items: 
          
        # format loop 1
        - name: "Tạo danh sách trong PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Tạo danh sách trong DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Tạo danh sách trong PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Tạo danh sách trong XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---