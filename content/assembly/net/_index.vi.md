---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: vi
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "API .NET cho Tự động hóa Tài liệu, Lắp ráp & Tạo báo cáo"
head_description: "API C# .NET cho tự động hóa tài liệu, lắp ráp và tạo báo cáo. Tạo tài liệu PDF, Word, Excel, PPTX, HTML và email từ các mẫu tùy chỉnh."

############################# Header ############################
title: "API Tự động hóa Tài liệu & Báo cáo .NET"
description: "Tạo báo cáo trong các ứng dụng .NET bằng cách định nghĩa các mẫu và gộp dữ liệu."
words:
  for: "cho"

actions:
  main: "Tải xuống Bản dùng thử qua NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Bạn đã sẵn sàng bắt đầu chưa?"
  description: "Hãy thử các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu cấp phép."

release:
  title: "Phiên bản {0} đã được phát hành"
  notes: "Xem điều gì mới"
  downloads: "Tải xuống"

code:
  title: "Điền Biểu đồ trong DOCX Sử dụng C#"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Đường dẫn đến mẫu chính
    string template = "chart_template.docx";

    // Lấy dữ liệu năng suất của các quản lý từ nguồn
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Tạo một thể hiện của DataSourceInfo với dữ liệu
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Đặt màu sắc biểu đồ bằng cách sử dụng DataSourceInfo khác
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Điền mẫu bằng dữ liệu và lưu vào đầu ra
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Assembly"
  description: "Giải pháp .NET cho việc tự động hóa tạo tài liệu với tích hợp dữ liệu nâng cao."
  features:
    # feature loop
    - title: "Thêm Dữ liệu Doanh nghiệp vào Các Mẫu Tài liệu với C#"
      content: "Tạo báo cáo nhanh chóng: Với GroupDocs.Assembly for .NET, bạn có thể dễ dàng chèn dữ liệu từ các nguồn như JSON hoặc XML vào các mẫu đã được định nghĩa trước."

    # feature loop
    - title: "Xử lý Các Đối tượng Dữ liệu Bản địa"
      content: "Các loại tài liệu được hỗ trợ bao gồm các đối tượng nhúng như sơ đồ, biểu đồ, bảng và danh sách có thể được lấp đầy tự động với dữ liệu."

    # feature loop
    - title: "Các Tính năng Bổ sung"
      content: "GroupDocs.Assembly for .NET cung cấp nhiều tùy chọn tùy chỉnh. Thiết kế các đối tượng dữ liệu lập trình, tạo mã vạch, sử dụng nguồn dữ liệu trực tuyến qua URL và lưu đầu ra ở nhiều định dạng khác nhau."

############################# Platforms ############################
platforms:
  enable: true
  title: "Tính độc lập của nền tảng"
  description: "GroupDocs.Assembly for .NET tương thích với các hệ điều hành, khung phát triển và trình quản lý gói sau."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tệp được hỗ trợ"
  description: |
    GroupDocs.Assembly for .NET có thể xử lý các [định dạng tệp](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Định dạng Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Hình ảnh & Định dạng Khác
        * **Di động:** PDF
        * **Hình ảnh:** SVG, TIFF
        * **Định dạng văn phòng khác:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Định dạng khác
        * **Web:** HTML, MHTML
        * **Email:** EML, MSG, EMLX
        * **Khác:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Các Tính năng của GroupDocs.Assembly"
  description: "Tạo tài liệu và báo cáo bằng cách sử dụng mô hình dữ liệu nâng cao."

  items:
    # feature loop
    - icon: "preview"
      title: "Biểu diễn Dữ liệu Nâng cao"
      content: "Hỗ trợ nhiều loại đối tượng dữ liệu như biểu đồ, danh sách, bảng, hình ảnh và hơn thế nữa."

    # feature loop
    - icon: "manipulate"
      title: "Xử lý Dữ liệu"
      content: "Áp dụng công thức và thao tác tuần tự để định dạng và hiển thị dữ liệu hiệu quả."

    # feature loop
    - icon: "two_pages"
      title: "Dải Định dạng Được Hỗ trợ Rộng Rãi"
      content: "Làm việc liền mạch với tất cả các định dạng tài liệu phổ biến cho các mẫu hoặc tệp đầu ra."

    # feature loop
    - icon: "document_settings"
      title: "Cú pháp Mẫu Đảo ngữ"
      content: "Tận dụng định dạng số thứ tự, số đếm và định dạng số chữ cái trong các mẫu."

    # feature loop
    - icon: "text"
      title: "Chèn Mã vạch"
      content: "Tạo hình ảnh mã vạch một cách động và chèn chúng vào tài liệu của bạn."

    # feature loop
    - icon: "add"
      title: "Định dạng Dữ liệu"
      content: "Định dạng chuỗi trong các mẫu thành chữ hoa, chữ thường, viết hoa chữ cái đầu hoặc định dạng kiểu chữ cái đầu tiên."

    # feature loop
    - icon: "manipulate"
      title: "Xử lý Nội dung Tài liệu"
      content: "Chèn nội dung từ tài liệu bên ngoài vào báo cáo của bạn một cách động."

    # feature loop
    - icon: "convert"
      title: "Lưu Ở Nhiều Định dạng"
      content: "Chỉ định định dạng tệp đầu ra bằng cách sử dụng phần mở rộng tệp hoặc cấu hình chi tiết."

    # feature loop
    - icon: "update"
      title: "Xử lý Dữ liệu Linh hoạt"
      content: "Chèn hình ảnh và tài liệu một cách động bằng cách sử dụng byte được mã hóa Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Các đoạn mã cho các thao tác GroupDocs.Assembly điển hình."
  items:
    # code sample loop
    - title: "Danh sách Có dấu đầu dòng trong Tài liệu Microsoft Word"
      content: |
        [Danh sách có dấu đầu dòng](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) là một cách phổ biến để trình bày dữ liệu doanh nghiệp. Dưới đây là ví dụ về việc thêm danh sách vào tài liệu Word bằng cách sử dụng GroupDocs.Assembly.
        {{< landing/code title="Cách Lấp Đầy Danh Sách Trong Tài Liệu">}}
        ```csharp {style=abap}
        // Chèn mẫu này vào trang tài liệu:
        // Các chỉ số hiệu suất của các quản lý
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Chỉ định đường dẫn mẫu
        string template = "Bulleted List Template.docx";

        // Đặt đường dẫn tệp đầu ra
        string result = "Result Report.docx"

        // Lấy dữ liệu của các quản lý từ nguồn JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Tạo báo cáo với dữ liệu đã được lấp đầy
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Biểu đồ Bánh trong Bài thuyết trình PPTX"
      content: |
        Bạn có thể tạo [Biểu đồ Bánh](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) bằng cách sử dụng các mẫu và dữ liệu XML. Nâng cao báo cáo của bạn với các biểu diễn dữ liệu thu hút về mặt hình ảnh.
        {{< landing/code title="Cách Biểu diễn Dữ liệu trong Biểu đồ Bánh">}}
        ```csharp {style=abap}
        // Thêm mẫu tiêu đề biểu đồ vào bài thuyết trình:
        // Doanh thu của khách hàng <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Cũng bao gồm mẫu dữ liệu biểu đồ:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Chỉ định đường dẫn đến mẫu biểu đồ
        string template = "Pie Chart Template.pptx";

        // Đặt đường dẫn tệp đầu ra
        string result = "Result Report.pptx"

        // Lấy dữ liệu của khách hàng từ nguồn XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Tạo biểu đồ và lưu kết quả
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---