



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:17
draft: false
lang: vi
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: ""
head_description: ""

############################# Header ############################
title: "" 
description: ""
subtitle: "" 

header_actions:
  enable: true
  items:
    #  loop
    - title: ""
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: ""
    link: "/assembly/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {steps.content.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {steps.content.step_4}
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Tài liệu mẫu"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Nhiều ví dụ hơn"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "list_template.docx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "{more_features.image_description}"
  features:
    # feature loop
    - title: "{more_features.feature_1.title}"
      content: "{more_features.feature_1.content}"

    # feature loop
    - title: "{more_features.feature_2.title}"
      content: "{more_features.feature_2.content}"

    # feature loop
    - title: "{more_features.feature_3.title}"
      content: "{more_features.feature_3.content}"

    # feature loop
    - title: "{more_features.feature_4.title}"
      content: "{more_features.feature_4.content}"
      
  code_samples_ext:
    # code sample ext loop
    - title: "{code_1.title}"
      content: |
        {code_1.content}
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // {code_1.comment_1}
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          const template = "numlist_template.docx";

          // {code_1.comment_3}
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // {code_1.comment_4}
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // {code_1.comment_5}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.docx", data);
          ```
        platform: "java"
        copy_title: "Sao chép"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.docx"
        links:
          #  loop
          - title: "Nhiều ví dụ hơn"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Tài liệu"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu chưa?"
  description: "Khám phá các tính năng của GroupDocs.Assembly miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống từ NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Tìm hiểu về giấy phép"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "list"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Tạo và thêm mã vạch vào tài liệu một cách động"

        # operation loop 2
        - name: "Trực quan hóa dữ liệu với biểu đồ"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Điền dữ liệu vào nhiều loại biểu đồ khác nhau"

        # operation loop 3
        - name: "Gộp tài liệu"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Kết hợp nội dung của một tài liệu vào tài liệu khác"

        # operation loop 4
        - name: "Hiển thị dữ liệu với danh sách"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Tạo danh sách trong tài liệu bằng dữ liệu cụ thể"

        # operation loop 5
        - name: "Tổ chức dữ liệu trong bảng"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Truy xuất dữ liệu từ bất kỳ nguồn nào và điền vào bảng"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "DOCX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Tạo danh sách trong PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Tạo danh sách trong DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Tài liệu mở XML của Microsoft Word"
          
        # format loop 3
        - name: "Tạo danh sách trong PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Bài thuyết trình mở XML của PowerPoint"
          
        # format loop 4
        - name: "Tạo danh sách trong XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Bảng tính mở XML của Microsoft Excel"


          

---