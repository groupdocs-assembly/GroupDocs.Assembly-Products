---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
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
head_title: "{index-content-nodejs-java.head_title}"
head_description: "{index-content-nodejs-java.head_description}"

############################# Header ############################
title: "{index-content-nodejs-java.title}"
description: "{index-content-nodejs-java.description}"
words:
  for: "cho"

actions:
  main: "{index-content-nodejs-java.actions_main}"
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
  title: "{index-content-nodejs-java.code_title}"
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
  description: "{index-content-nodejs-java.overview_description}"
  features:
    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_1.title}"
      content: "{index-content-nodejs-java.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_2.title}"
      content: "{index-content-nodejs-java.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_3.title}"
      content: "{index-content-nodejs-java.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "Tính độc lập của nền tảng"
  description: "{index-content-nodejs-java.platforms_description}"
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
    {index-content-nodejs-java.formats_description}
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
  title: "{index-content-nodejs-java.features.title}"
  description: "{index-content-nodejs-java.features.description}"

  items:
    # feature loop
    - icon: "preview"
      title: "{index-content-nodejs-java.features.feature_1.title}"
      content: "{index-content-nodejs-java.features.feature_1.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_2.title}"
      content: "{index-content-nodejs-java.features.feature_2.content}"

    # feature loop
    - icon: "two_pages"
      title: "{index-content-nodejs-java.features.feature_3.title}"
      content: "{index-content-nodejs-java.features.feature_3.content}"

    # feature loop
    - icon: "document_settings"
      title: "{index-content-nodejs-java.features.feature_4.title}"
      content: "{index-content-nodejs-java.features.feature_4.content}"

    # feature loop
    - icon: "text"
      title: "{index-content-nodejs-java.features.feature_5.title}"
      content: "{index-content-nodejs-java.features.feature_5.content}"

    # feature loop
    - icon: "add"
      title: "{index-content-nodejs-java.features.feature_6.title}"
      content: "{index-content-nodejs-java.features.feature_6.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_7.title}"
      content: "{index-content-nodejs-java.features.feature_7.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-nodejs-java.features.feature_8.title}"
      content: "{index-content-nodejs-java.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-nodejs-java.features.feature_9.title}"
      content: "{index-content-nodejs-java.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
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
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
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