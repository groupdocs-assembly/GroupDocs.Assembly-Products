



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: vi
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tạo danh sách trong tài liệu XLSX bằng Java"
head_description: "Thiết kế và nhúng danh sách động vào các mẫu XLSX của bạn với API GroupDocs.Assembly for Java."

############################# Header ############################
title: "Thêm danh sách động vào tệp XLSX với API Java của chúng tôi" 
description: "GroupDocs.Assembly for Java cung cấp các công cụ linh hoạt để tạo và chèn các danh sách chứa dữ liệu trực tiếp vào tài liệu XLSX."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Thử miễn phí"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java là gì?"
    link: "/assembly/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) giúp bạn thiết kế tài liệu chuyên nghiệp bằng cách kéo dữ liệu từ nhiều nguồn khác nhau. Sử dụng nó để tạo danh sách, bảng, biểu đồ hoặc văn bản, và đặt các phần tử này chính xác ở nơi cần thiết với các tính năng mẫu nâng cao. Với hỗ trợ cho hơn 50 định dạng, bao gồm PDF, tệp MS Office và tài liệu email, nó giúp tự động hóa và tối ưu hóa quy trình làm việc của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Cách thêm danh sách dựa trên dữ liệu vào tài liệu XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) cho phép bạn nhanh chóng chèn các danh sách chứa dữ liệu vào mẫu XLSX. Tùy chỉnh và tổ chức nội dung một cách dễ dàng.
      
      1. Tạo một mẫu XLSX và đánh dấu các vị trí giữ chỗ cho danh sách.
      2. Xác định đường dẫn tệp đến mẫu.
      3. Lấy dữ liệu từ các định dạng được hỗ trợ như JSON hoặc XML.
      4. Lưu tài liệu cuối cùng với danh sách đã được thêm vào.
   
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
        // Thêm thẻ này vào mẫu của bạn nơi danh sách nên xuất hiện
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Xác định đường dẫn tệp của mẫu
        String template = "list_template.xlsx";

        // Kéo dữ liệu từ nguồn bạn đã chọn
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Lưu tài liệu với danh sách đã nhúng
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Tạo tài liệu từ các mẫu với tích hợp dữ liệu"
  description: "GroupDocs.Assembly for Java đơn giản hóa việc thêm các danh sách động, bảng, biểu đồ và các thành phần khác vào các mẫu tài liệu."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Xây dựng báo cáo với dữ liệu từ nhiều nguồn khác nhau"
      content: "Sử dụng dữ liệu từ các định dạng như JSON, XML và CSV để điền các danh sách và các thành phần khác một cách hiệu quả."

    # feature loop
    - title: "Thêm danh sách và các yếu tố dữ liệu khác một cách liền mạch"
      content: "GroupDocs.Assembly cho phép nhúng danh sách, biểu đồ, bảng và nhiều hơn nữa, bên cạnh văn bản, hình ảnh và liên kết để tạo tài liệu hoàn thiện."

    # feature loop
    - title: "Kiểm soát chính xác vị trí xuất hiện của dữ liệu"
      content: "Các mẫu dựa trên LINQ cho phép bạn xác định chính xác các vị trí cho danh sách và dữ liệu của bạn. Sử dụng vòng lặp để tự động tạo danh sách chi tiết và áp dụng định dạng tùy chỉnh."

    # feature loop
    - title: "Hỗ trợ nhiều định dạng tài liệu"
      content: "Tạo hoặc chỉnh sửa tệp ở các định dạng như MS Office, PDF, OpenOffice, HTML và email. Hợp nhất nội dung từ nhiều tài liệu khi cần thiết."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách tạo danh sách một cách lập trình"
      content: |
        Ví dụ này cho thấy cách thêm một danh sách một cách động vào tệp XLSX bằng GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Thêm một thẻ giữ chỗ trong mẫu của bạn cho danh sách
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Cung cấp đường dẫn tệp đến mẫu của bạn
          String template = "numlist_template.xlsx";

          // Lấy dữ liệu cần thiết để điền vào danh sách
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Chuẩn bị nguồn dữ liệu với các thông tin cần thiết
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Khởi tạo DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tài liệu xuất ra với danh sách đã hoàn thành
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "Khám phá những gì GroupDocs.Assembly có thể làm"
    exclude: "list"
    description: "Tạo và thiết kế tài liệu giàu nội dung dễ dàng với các công cụ tích hợp dữ liệu nâng cao."
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
    title: "Sản xuất tài liệu ở nhiều định dạng khác nhau"
    exclude: "XLSX"
    description: "Java hỗ trợ hơn 50 định dạng, cho phép bạn tạo các tài liệu có cấu trúc bằng cách kết hợp dữ liệu và mẫu."
    items: 
          
        # format loop 1
        - name: "Tạo danh sách trong PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Tạo danh sách trong DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Tạo danh sách trong PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Tạo danh sách trong XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---