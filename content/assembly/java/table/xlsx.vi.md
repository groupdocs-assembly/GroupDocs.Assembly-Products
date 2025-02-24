



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: vi
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Thêm bảng vào tài liệu XLSX bằng Java"
head_description: "Với GroupDocs.Assembly for Java, các nhà phát triển có thể nhanh chóng tích hợp bảng vào tài liệu và email, kéo dữ liệu từ các nguồn động."

############################# Header ############################
title: "Dễ dàng điền bảng vào tệp XLSX với API Java của chúng tôi" 
description: "GroupDocs.Assembly for Java đơn giản hóa quy trình điền bảng trong tài liệu XLSX bằng dữ liệu từ nhiều nguồn khác nhau."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nhận Bản Dùng Thử Miễn Phí"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java là gì?"
    link: "/assembly/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) là một công cụ tạo tài liệu và báo cáo bằng cách tự động chèn dữ liệu vào các mẫu đã thiết kế sẵn. Bạn có thể dễ dàng thêm bảng, danh sách, biểu đồ và hình ảnh. Các tính năng tiên tiến cho phép bạn đặt nội dung chính xác trong tài liệu của mình. Tương thích với hơn 50 định dạng tệp, bao gồm PDF, MS Office và các định dạng email.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để chèn dữ liệu vào bảng XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) giúp bạn điền các mẫu bảng cho XLSX và các định dạng khác. Sử dụng dữ liệu động từ các nguồn của bạn để tạo bảng một cách hiệu quả.
      
      1. Thiết lập một mẫu XLSX với các vị trí giữ chỗ cho hàng và cột bảng.
      2. Kéo dữ liệu từ bất kỳ nguồn đầu vào nào được hỗ trợ.
      3. Lọc hoặc xử lý trước dữ liệu để phù hợp với nhu cầu của bạn.
      4. Tạo tài liệu cuối cùng với bảng đã hoàn thành.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Tài liệu mẫu"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Nhiều ví dụ hơn"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Sử dụng các thẻ này trong một vị trí hàng bảng trong mẫu của bạn
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Xác định đường dẫn đến tệp mẫu
        String template = "table_template.xlsx";

        // Tải dữ liệu từ nguồn bạn chọn
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Lưu tệp đầu ra với bảng đã được điền
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Tạo tài liệu với bảng đã điền dữ liệu"
  description: "GroupDocs.Assembly for Java giúp việc tự động hóa tạo bảng trong tài liệu của bạn trở nên đơn giản. Nó cũng hỗ trợ thêm các phần tử như biểu đồ, danh sách và hình ảnh bằng cách sử dụng các mẫu."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Các Tính Năng Chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tạo báo cáo từ nhiều định dạng dữ liệu"
      content: "API hoạt động liền mạch với JSON, XML, CSV và các định dạng khác để điền bảng trong tài liệu của bạn với dữ liệu có tổ chức."

    # feature loop
    - title: "Trình bày thông tin một cách trực quan"
      content: "GroupDocs.Assembly giúp bạn xây dựng bảng, danh sách và biểu đồ chuyên nghiệp, cũng như chèn liên kết, văn bản và hình ảnh, để có cái nhìn tinh tế."

    # feature loop
    - title: "Đặt nội dung bảng một cách chính xác"
      content: "Sử dụng cú pháp linh hoạt dựa trên LINQ để thêm hàng và cột một cách động. Tùy chỉnh giao diện, chẳng hạn như kiểu và màu sắc phông chữ, một cách lập trình."

    # feature loop
    - title: "Tương thích với nhiều định dạng"
      content: "Làm việc với MS Office, OpenOffice, PDF, HTML và nhiều định dạng khác. Gộp bảng vào bất kỳ định dạng tệp nào được hỗ trợ một cách dễ dàng."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tạo bảng điền dữ liệu một cách động"
      content: |
        Ví dụ này cho thấy cách điền một bảng trong tài liệu XLSX sử dụng dữ liệu đầu vào động.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Thiết kế một mẫu với một vị trí giữ chỗ cho bảng
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Đặt vị trí tệp mẫu
          String template = "table_template.xlsx";

          // Tải dữ liệu từ nguồn ưa thích của bạn
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Chuẩn bị một đối tượng dữ liệu chứa các trường cần thiết
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Tạo một phiên bản của DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tài liệu với bảng đã được điền
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Sao chép"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.xlsx"
        links:
          #  loop
          - title: "Nhiều ví dụ hơn"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Tài liệu"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu chưa?"
  description: "Khám phá các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống từ Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Tìm hiểu về giấy phép"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Các tính năng chính trong tầm nhìn"
    exclude: "table"
    description: "API của chúng tôi đơn giản hóa việc tạo tài liệu chuyên nghiệp bằng cách tự động hóa việc điền bảng cùng với các thành phần mạnh mẽ khác."
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tạo bảng chi tiết trong nhiều định dạng"
    exclude: "XLSX"
    description: "Với Java, bạn có thể điền dữ liệu vào các mẫu và tạo báo cáo chi tiết trong hơn 50 định dạng tệp."
    items: 
          
        # format loop 1
        - name: "Thêm bảng vào PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm bảng vào DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Thêm bảng vào PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Thêm bảng vào XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---