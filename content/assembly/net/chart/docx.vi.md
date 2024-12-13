



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: vi
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tạo biểu đồ trong tệp DOCX với C#"
head_description: "API GroupDocs.Assembly for .NET giúp các nhà phát triển dễ dàng tạo và chèn biểu đồ hoặc đồ thị vào tài liệu một cách động bằng dữ liệu thời gian thực."

############################# Header ############################
title: "Nhúng biểu đồ vào tệp DOCX với API .NET" 
description: "GroupDocs.Assembly for .NET cung cấp cách mạnh mẽ để làm đầy tệp DOCX bằng dữ liệu động và tích hợp biểu đồ một cách liền mạch."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dùng thử miễn phí"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET là gì?"
    link: "/assembly/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) là một công cụ được thiết kế để đơn giản hóa việc tạo tài liệu và báo cáo bằng cách tích hợp dữ liệu từ nhiều nguồn khác nhau. Tạo biểu đồ, bảng, danh sách, mã vạch và hình ảnh động. Các tùy chọn định dạng nâng cao cho phép đặt chính xác và tùy chỉnh nội dung của bạn. Nó hỗ trợ hơn 50 định dạng tệp, bao gồm PDF, tài liệu MS Office và email.

############################# Steps ############################
steps:
    enable: true
    title: "Cách thêm biểu đồ vào tài liệu DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) giúp đơn giản hóa việc tạo và nhúng biểu đồ vào các mẫu DOCX của bạn. Hỗ trợ nhiều loại biểu đồ như biểu đồ cột, biểu đồ tròn và biểu đồ đường.
      
      1. Thiết kế một mẫu DOCX với các vị trí dành cho biểu đồ.
      2. Lấy dữ liệu của bạn từ một nguồn tương thích.
      3. Xác định các tùy chọn biểu đồ như loại, nhãn và bảng màu.
      4. Lưu tệp đã cập nhật với biểu đồ được nhúng.
   
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
        // Bao gồm thẻ này trong mẫu của bạn để tạo biểu đồ
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Xác định đường dẫn tệp cho mẫu của bạn
        string template = "chart_template.docx";

        // Tải dữ liệu từ nguồn mà bạn chọn
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Lưu tài liệu với biểu đồ được nhúng
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Thêm biểu đồ động vào tài liệu của bạn một cách dễ dàng"
  description: "GroupDocs.Assembly for .NET đơn giản hóa việc tạo các tài liệu dựa trên dữ liệu trong các định dạng phổ biến. Sử dụng mẫu để chèn biểu đồ, bảng, mã vạch, danh sách, liên kết và hình ảnh với tích hợp dữ liệu động tiên tiến."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Chuyển đổi dữ liệu thành biểu đồ chuyên nghiệp"
      content: "Chuyển đổi dữ liệu từ JSON, XML, CSV và các nguồn khác thành các biểu đồ hấp dẫn một cách nhanh chóng bằng API của chúng tôi."

    # feature loop
    - title: "Tạo nội dung thu hút thị giác"
      content: "GroupDocs.Assembly hỗ trợ nhiều loại biểu đồ như biểu đồ cột, biểu đồ tròn và biểu đồ đường. Kết hợp chúng với bảng, mã vạch, hình ảnh và các yếu tố khác để tạo báo cáo chuyên nghiệp."

    # feature loop
    - title: "Đặt và tùy chỉnh biểu đồ một cách chính xác"
      content: "Với cú pháp LINQ, bạn có thể tạo và đặt biểu đồ một cách động chính xác nơi cần thiết. Tùy chỉnh kiểu dáng, màu sắc và bố cục để phù hợp với yêu cầu của bạn."

    # feature loop
    - title: "Hoạt động với nhiều định dạng tệp khác nhau"
      content: "Xuất bản tài liệu ở các định dạng phổ biến như MS Office, PDF, OpenOffice và HTML. Nhúng biểu đồ một cách liền mạch trong bất kỳ định dạng nào được hỗ trợ với khả năng tương thích hoàn toàn."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tạo biểu đồ lập trình"
      content: |
        Ví dụ này minh họa cách tạo và nhúng một biểu đồ vào tài liệu DOCX một cách động.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Chuẩn bị một mẫu với một vị trí dành cho biểu đồ
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Cung cấp đường dẫn đến tệp mẫu
          string template = "table_template.docx";

          // Lấy dữ liệu từ nguồn của bạn
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Xây dựng một đối tượng dữ liệu với các thông tin cần thiết
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Cài đặt thuộc tính biểu đồ như loại và hình thức
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Khởi tạo DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Xuất tài liệu với biểu đồ đã bao gồm
          asm.AssembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    exclude: "chart"
    description: "Nền tảng của chúng tôi giúp bạn tạo ra các tài liệu hấp dẫn, dựa trên dữ liệu được tùy chỉnh theo nhu cầu của bạn."
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
    title: "Tạo báo cáo phong phú về nội dung trong nhiều định dạng"
    exclude: "DOCX"
    description: ".NET cho phép bạn tạo tài liệu với các biểu đồ tích hợp trong hơn 50 định dạng được hỗ trợ, kết hợp các mẫu với dữ liệu của bạn một cách liền mạch."
    items: 
          
        # format loop 1
        - name: "Biểu đồ trong PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Biểu đồ trong DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Biểu đồ trong PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Biểu đồ trong XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---