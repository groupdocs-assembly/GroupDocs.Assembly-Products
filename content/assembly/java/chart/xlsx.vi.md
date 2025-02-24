



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: vi
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tạo biểu đồ trong tài liệu XLSX sử dụng Java"
head_description: "API GroupDocs.Assembly for Java cho phép các nhà phát triển tạo và chèn biểu đồ hoặc đồ thị động vào tài liệu một cách liền mạch, được cung cấp bởi dữ liệu trực tiếp."

############################# Header ############################
title: "Thêm biểu đồ vào tài liệu XLSX với API Java" 
description: "GroupDocs.Assembly for Java đơn giản hóa quy trình nhúng biểu đồ vào tài liệu XLSX bằng cách sử dụng dữ liệu theo thời gian thực."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu miễn phí"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) là một giải pháp linh hoạt cho việc tự động hóa việc tạo tài liệu và báo cáo. Nó cho phép bạn thêm biểu đồ, bảng, danh sách, mã vạch và hình ảnh trực tiếp vào tệp của bạn, với các công cụ tiên tiến để định dạng chính xác và tích hợp dữ liệu. Nền tảng này hỗ trợ hơn 50 định dạng, bao gồm PDF, tệp Microsoft Office và email.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để nhúng một biểu đồ vào tài liệu XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) đơn giản hóa quy trình chèn các biểu đồ vào các mẫu XLSX. Chọn từ một loạt các phong cách biểu đồ, bao gồm biểu đồ thanh, biểu đồ tròn, và biểu đồ đường.
      
      1. Tạo một mẫu XLSX với các vị trí giữ chỗ cho biểu đồ.
      2. Tải dữ liệu của bạn từ một nguồn tương thích.
      3. Đặt các tùy chọn biểu đồ, chẳng hạn như loại, nhãn và màu sắc.
      4. Lưu tài liệu với biểu đồ được bao gồm.
   
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
        // Thêm thẻ này vào mẫu của bạn để bao gồm một biểu đồ
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Cung cấp đường dẫn tệp đến mẫu của bạn
        String template = "chart_template.xlsx";

        // Trích xuất dữ liệu cần thiết từ nguồn của bạn
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Lưu tài liệu cuối cùng với biểu đồ được nhúng
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Nhanh chóng nhúng biểu đồ động vào tài liệu của bạn"
  description: "GroupDocs.Assembly for Java cung cấp một cách đơn giản để xây dựng tài liệu phong phú dữ liệu ở các định dạng phổ biến. Sử dụng mẫu để chèn biểu đồ, bảng, mã vạch, danh sách, liên kết và hình ảnh với cập nhật động từ dữ liệu của bạn."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Biến dữ liệu thành biểu đồ"
      content: "Sử dụng API để chuyển đổi dữ liệu từ JSON, XML, CSV hoặc các nguồn khác thành các biểu đồ chuyên nghiệp cho tài liệu của bạn."

    # feature loop
    - title: "Tạo nội dung trực quan ấn tượng"
      content: "GroupDocs.Assembly hỗ trợ nhiều định dạng hình ảnh khác nhau, bao gồm đồ thị thanh, biểu đồ tròn và biểu đồ đường, có thể được kết hợp với bảng, mã vạch, hình ảnh, và nhiều hơn nữa để tạo ra các báo cáo được cải tiến."

    # feature loop
    - title: "Tùy chỉnh vị trí và phong cách biểu đồ"
      content: "Với cú pháp dựa trên LINQ, bạn có thể tạo và định vị các biểu đồ một cách động trong tài liệu, đồng thời điều chỉnh phong cách, màu sắc và bố cục để đáp ứng nhu cầu thiết kế của bạn."

    # feature loop
    - title: "Hỗ trợ nhiều định dạng tài liệu"
      content: "Tạo tài liệu ở các định dạng như MS Office, PDF, OpenOffice và HTML. Các biểu đồ tích hợp mượt mà vào bất kỳ định dạng nào được hỗ trợ để có kết quả chuyên nghiệp."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tạo và nhúng biểu đồ chương trình"
      content: |
        Ví dụ này minh họa cách tạo và nhúng một biểu đồ vào tài liệu XLSX một cách chương trình.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Chuẩn bị một mẫu với một vị trí giữ chỗ cho biểu đồ
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Chỉ định đường dẫn tệp đến mẫu
          String template = "table_template.xlsx";

          // Tải dữ liệu từ nguồn bạn chọn
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Tạo một đối tượng dữ liệu với thông tin liên quan
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Cấu hình loại và diện mạo của biểu đồ
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Khởi tạo DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Lưu tài liệu hoàn chỉnh với biểu đồ được nhúng
          asm.assembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Khám phá các khả năng mạnh mẽ"
    exclude: "chart"
    description: "Nền tảng này đơn giản hóa quy trình thiết kế tài liệu tập trung vào dữ liệu, hấp dẫn về mặt trực quan, phù hợp với nhu cầu của bạn."
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
    title: "Tạo báo cáo toàn diện trong nhiều định dạng"
    exclude: "XLSX"
    description: "Java cho phép bạn tạo tài liệu với các biểu đồ tích hợp qua hơn 50 định dạng tệp, đảm bảo sự kết hợp liền mạch giữa các mẫu và dữ liệu."
    items: 
          
        # format loop 1
        - name: "Biểu đồ trong PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Biểu đồ trong DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Biểu đồ trong PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Biểu đồ trong XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---