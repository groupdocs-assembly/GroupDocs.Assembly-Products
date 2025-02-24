---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: vi
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

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
head_title: "Thư viện Java cho Tạo Tài liệu, Tự động hóa & Báo cáo"
head_description: "Thư viện Java cho việc tự động hóa tạo tài liệu và tạo báo cáo. Tạo tài liệu PDF, Word, Excel, PPTX, HTML và email bằng cách sử dụng các mẫu tùy chỉnh."

############################# Header ############################
title: "API Java cho Tự động hóa Báo cáo và Tài liệu"
description: "Đơn giản hóa việc tạo báo cáo trong Java bằng cách gộp dữ liệu với các mẫu."
words:
  for: "cho"

actions:
  main: "Nhận Bản dùng thử qua Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Bạn đã sẵn sàng bắt đầu chưa?"
  description: "Hãy thử các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu cấp phép."

release:
  title: "Phiên bản {0} đã được phát hành"
  notes: "Xem điều gì mới"
  downloads: "Tải xuống"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Tạo Biểu đồ trong DOCX bằng Java"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Đường dẫn đến mẫu chính
    String template = "chart_template.docx";

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
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Assembly"
  description: "Thư viện Java được thiết kế để tự động hóa việc tạo tài liệu và tích hợp dữ liệu liền mạch."
  features:
    # feature loop
    - title: "Gộp Dữ liệu Doanh nghiệp vào Các Mẫu bằng Java"
      content: "Dễ dàng tạo báo cáo chuyên nghiệp bằng cách nhúng dữ liệu từ JSON, XML hoặc các nguồn khác vào các mẫu được thiết kế trước bằng GroupDocs.Assembly for Java."

    # feature loop
    - title: "Làm việc với Các Đối tượng Nhúng"
      content: "Tự động lấp đầy các phần tử như bảng, biểu đồ và sơ đồ trong tài liệu bằng dữ liệu từ các nguồn bên ngoài."

    # feature loop
    - title: "Tùy chỉnh Nâng cao"
      content: "GroupDocs.Assembly for Java cung cấp các tính năng linh hoạt như tạo mã vạch, lấy dữ liệu trực tuyến thông qua URL và xuất đầu ra ở nhiều định dạng khác nhau."

############################# Platforms ############################
platforms:
  enable: true
  title: "Tính độc lập của nền tảng"
  description: "GroupDocs.Assembly for Java làm việc liền mạch với các hệ điều hành phổ biến, khung phát triển và trình quản lý gói."
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
    GroupDocs.Assembly for Java hỗ trợ một loạt các [định dạng tài liệu](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Các Khả năng Chính của GroupDocs.Assembly"
  description: "Tạo tài liệu và báo cáo chuyên nghiệp với việc xử lý dữ liệu nâng cao."

  items:
    # feature loop
    - icon: "preview"
      title: "Các Thành Phần Dữ liệu Thị giác"
      content: "Thêm và định dạng các phần tử như biểu đồ, bảng, hình ảnh và danh sách trực tiếp trong tài liệu của bạn."

    # feature loop
    - icon: "manipulate"
      title: "Biến đổi Dữ liệu"
      content: "Sử dụng công thức, sắp xếp và các công cụ khác để tổ chức và trình bày dữ liệu của bạn hiệu quả."

    # feature loop
    - icon: "two_pages"
      title: "Hỗ trợ Nhiều Định dạng"
      content: "Dễ dàng làm việc với các loại tệp phổ biến cho cả mẫu và tệp đầu ra."

    # feature loop
    - icon: "document_settings"
      title: "Định dạng Mẫu Nâng cao"
      content: "Tùy chỉnh các mẫu với các tùy chọn định dạng số, chữ cái và định dạng nâng cao khác."

    # feature loop
    - icon: "text"
      title: "Tạo Mã vạch Động"
      content: "Nhanh chóng tạo và chèn hình ảnh mã vạch vào tài liệu khi cần."

    # feature loop
    - icon: "add"
      title: "Định dạng Văn bản Linh hoạt"
      content: "Áp dụng các biến đổi văn bản như chữ hoa, chữ thường, chữ viết hoa hoặc các kiểu khác trong các mẫu."

    # feature loop
    - icon: "manipulate"
      title: "Nhập Nội dung Bên ngoài"
      content: "Chèn nội dung từ các tệp bên ngoài một cách động trong khi tạo tài liệu."

    # feature loop
    - icon: "convert"
      title: "Xuất ở Nhiều Định dạng"
      content: "Lưu các tài liệu cuối cùng ở nhiều định dạng tệp khác nhau bằng cách sử dụng các phần mở rộng hoặc cấu hình đã chỉ định."

    # feature loop
    - icon: "update"
      title: "Nhúng Tài nguyên Động"
      content: "Chèn hình ảnh hoặc nội dung khác bằng cách sử dụng dữ liệu mã hóa Base64 trong quá trình tạo tài liệu."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Khám phá mã mẫu cho các tác vụ chung với GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Tạo Danh sách Có Dấu đầu dòng trong Word"
      content: |
        Tìm hiểu cách thêm [danh sách có dấu đầu dòng](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) vào tài liệu Word để đại diện cho dữ liệu có tổ chức. Ví dụ này cho thấy cách tạo một danh sách trong Word bằng GroupDocs.Assembly.
        {{< landing/code title="Tạo Danh sách Có Dấu đầu dòng trong Word">}}
        ```java {style=abap}
        // Chèn mẫu này vào trang tài liệu:
        // Các chỉ số hiệu suất của các quản lý
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Chỉ định đường dẫn mẫu
        String template = "Bulleted List Template.docx";

        // Đặt đường dẫn tệp đầu ra
        String result = "Result Report.docx"

        // Lấy dữ liệu của các quản lý từ nguồn JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Tạo báo cáo với dữ liệu đã được lấp đầy
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tạo Biểu đồ Bánh trong PPTX"
      content: |
        Sử dụng các mẫu và XML để thêm [biểu đồ bánh](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) vào các bài thuyết trình của bạn. Làm cho báo cáo của bạn hấp dẫn hơn bằng cách bao gồm biểu đồ bánh để trực quan hóa dữ liệu.
        {{< landing/code title="Tạo Biểu đồ Bánh trong PPTX">}}
        ```java {style=abap}   
        // Thêm mẫu tiêu đề biểu đồ vào bài thuyết trình:
        // Doanh thu của khách hàng <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Cũng bao gồm mẫu dữ liệu biểu đồ:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Chỉ định đường dẫn đến mẫu biểu đồ
        String template = "Pie Chart Template.pptx";

        // Đặt đường dẫn tệp đầu ra
        String result = "Result Report.pptx"

        // Lấy dữ liệu của khách hàng từ nguồn XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Tạo biểu đồ và lưu kết quả
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---