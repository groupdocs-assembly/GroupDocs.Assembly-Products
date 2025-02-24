---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: vi
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Bộ Công Cụ Node.js để Xây Dựng, Tự Động Hóa và Tùy Chỉnh Tài Liệu"
head_description: "Thư viện Node.js để tự động hóa quy trình làm việc tài liệu. Tạo tệp PDF, Word, Excel, PowerPoint, HTML và email từ các mẫu của bạn."

############################# Header ############################
title: "API Node.js cho Tự Động Hóa Tài Liệu và Báo Cáo Đơn Giản"
description: "Tối ưu hóa việc tạo báo cáo JavaScript bằng cách kết hợp dữ liệu của bạn với các mẫu đã được xây dựng sẵn."
words:
  for: "cho"

actions:
  main: "Bắt Đầu Dùng Thử Trên NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Bạn đã sẵn sàng bắt đầu chưa?"
  description: "Hãy thử các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu cấp phép."

release:
  title: "Phiên bản {0} đã được phát hành"
  notes: "Xem điều gì mới"
  downloads: "Tải xuống"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Tạo Biểu Đồ Trong Tài Liệu Word Sử Dụng Node.js"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Đường dẫn đến mẫu chính
    const template = "chart_template.docx";

    // Lấy dữ liệu năng suất của các quản lý từ nguồn
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Tạo một thể hiện của DataSourceInfo với dữ liệu
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Đặt màu sắc biểu đồ bằng cách sử dụng DataSourceInfo khác
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Điền mẫu bằng dữ liệu và lưu vào đầu ra
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Assembly"
  description: "Thư viện Node.js được xây dựng để tạo tài liệu theo cách lập trình với việc xử lý dữ liệu tích hợp."
  features:
    # feature loop
    - title: "Tích Hợp Dữ Liệu Kinh Doanh Vào Mẫu Với JavaScript"
      content: "Tạo báo cáo chuyên nghiệp bằng cách nhúng JSON, XML hoặc dữ liệu khác vào mẫu với GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Quản Lý Nội Dung Nhúng"
      content: "Tự động điền bảng, biểu đồ và các hình ảnh khác trong tài liệu của bạn bằng cách sử dụng dữ liệu bên ngoài."

    # feature loop
    - title: "Tùy Chọn Tùy Biến"
      content: "GroupDocs.Assembly for Node.js via Java cho phép bạn thêm các tính năng như mã vạch, lấy dữ liệu từ URL và xuất tệp trong nhiều định dạng khác nhau."

############################# Platforms ############################
platforms:
  enable: true
  title: "Tính độc lập của nền tảng"
  description: "GroupDocs.Assembly for Node.js via Java tích hợp mượt mà với các hệ điều hành, framework và trình quản lý gói hàng đầu."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tệp được hỗ trợ"
  description: |
    GroupDocs.Assembly for Node.js via Java hỗ trợ một loạt [định dạng tài liệu](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "Các Tính Năng Cốt Lõi Của GroupDocs.Assembly"
  description: "Tạo tài liệu và báo cáo động với các công cụ quản lý dữ liệu mạnh mẽ."

  items:
    # feature loop
    - icon: "preview"
      title: "Hình Ảnh Dữ Liệu Đầy Đủ"
      content: "Chèn đầy đủ biểu đồ, bảng, hình ảnh và danh sách vào tài liệu của bạn với tùy chỉnh hoàn toàn."

    # feature loop
    - icon: "manipulate"
      title: "Chuyển Đổi Dữ Liệu Của Bạn"
      content: "Sử dụng các công cụ như công thức và sắp xếp để cấu trúc và hiển thị thông tin hiệu quả."

    # feature loop
    - icon: "two_pages"
      title: "Tính Tương Thích Định Dạng Rộng"
      content: "Làm việc liền mạch với các định dạng tệp phổ biến cho mẫu và đầu ra."

    # feature loop
    - icon: "document_settings"
      title: "Tùy Chỉnh Mẫu Cao Cấp"
      content: "Định dạng các mẫu với các tùy chọn kiểu dáng số, chữ cái và các kiểu khác."

    # feature loop
    - icon: "text"
      title: "Tạo Mã Vạch Động"
      content: "Tạo và nhúng hình ảnh mã vạch trực tiếp vào tài liệu của bạn theo yêu cầu."

    # feature loop
    - icon: "add"
      title: "Tùy Chỉnh Kiểu Chữ Linh Hoạt"
      content: "Áp dụng các kiểu chữ như chữ viết hoa hoặc chữ cái đầu tiên trong mẫu của bạn một cách dễ dàng."

    # feature loop
    - icon: "manipulate"
      title: "Chèn Nội Dung Động"
      content: "Bao gồm nội dung từ các tệp bên ngoài một cách động trong quá trình tạo tài liệu."

    # feature loop
    - icon: "convert"
      title: "Xuất Sang Nhiều Định Dạng"
      content: "Lưu tài liệu ở nhiều định dạng với các cấu hình mà bạn chỉ định."

    # feature loop
    - icon: "update"
      title: "Nhúng Media Động"
      content: "Chèn hình ảnh hoặc các yếu tố khác bằng cách sử dụng dữ liệu Base64 khi tạo tài liệu."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Khám phá các ví dụ thực tiễn về cách sử dụng GroupDocs.Assembly cho các tác vụ phổ biến."
  items:
    # code sample loop
    - title: "Thêm Danh Sách Có Dấu Chấm Trong Tài Liệu Word"
      content: |
        Xem cách tạo [danh sách có dấu chấm](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) trong tài liệu Word để tổ chức dữ liệu hiệu quả. Ví dụ này minh họa cách tạo một danh sách có dấu chấm bằng GroupDocs.Assembly.
        {{< landing/code title="Thêm Danh Sách Có Dấu Chấm Trong Tài Liệu Word">}}
        ```javascript {style=abap}
        // Chèn mẫu này vào trang tài liệu:
        // Các chỉ số hiệu suất của các quản lý
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Chỉ định đường dẫn mẫu
        const template = "Bulleted List Template.docx";

        // Đặt đường dẫn tệp đầu ra
        const result = "Result Report.docx"

        // Lấy dữ liệu của các quản lý từ nguồn JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Tạo báo cáo với dữ liệu đã được lấp đầy
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Chèn Biểu Đồ Bánh Vào PowerPoint"
      content: |
        Tìm hiểu cách sử dụng các mẫu và XML để thêm [biểu đồ bánh](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) vào bài thuyết trình của bạn. Nâng cao báo cáo của bạn với biểu đồ bánh để trình bày dữ liệu một cách trực quan và rõ ràng.
        {{< landing/code title="Chèn Biểu Đồ Bánh Vào PowerPoint">}}
        ```javascript {style=abap} 
        // Thêm mẫu tiêu đề biểu đồ vào bài thuyết trình:
        // Doanh thu của khách hàng <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Cũng bao gồm mẫu dữ liệu biểu đồ:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Chỉ định đường dẫn đến mẫu biểu đồ
        const template = "Pie Chart Template.pptx";

        // Đặt đường dẫn tệp đầu ra
        const result = "Result Report.pptx"

        // Lấy dữ liệu của khách hàng từ nguồn XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Tạo biểu đồ và lưu kết quả
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---