



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:15
draft: false
lang: zh
format: Xlsx
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
    link_title: "了解更多"
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
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "示例文档"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "doc_template.xlsx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo("insert.xlsx", "doc_expression");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_document.webp" # 500x500 px
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
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          const template = "template.xlsx";

          // {code_1.comment_3}
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // {code_1.comment_4}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_5}
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "复制"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.xlsx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费探索GroupDocs.Assembly的功能或请求许可证"
  items:
    #  loop
    - title: "从NPM下载"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "了解许可证信息"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "document"
    description: ""
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "XLSX"
    description: ""
    items: 
          
        # format loop 1
        - name: "在PDF中嵌入文档"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中嵌入文档"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中嵌入文档"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中嵌入文档"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---