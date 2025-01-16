



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:02
draft: false
lang: zh
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在JavaScript中合并DOCX文档"
head_description: "使用JavaScript快速合并DOCX文件。GroupDocs.Assembly将文档合并简化为几个简单步骤。"

############################# Header ############################
title: "高效地合并DOCX文件中的内容" 
description: "借助GroupDocs.Assembly for Node.js via Java，将一个DOCX文件集成到另一个文件中既快速又准确。享受灵活可靠的工具，实现无缝合并。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载试用"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java概述"
    link: "/assembly/nodejs-java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)提供了一种强大的文档管理方式。快速且准确地将一个文件合并到另一个文件中，同时支持超过50种格式，如PDF和MS Office。自定义布局、编辑内容并按照您的需求组织文档。

############################# Steps ############################
steps:
    enable: true
    title: "如何将文档合并到DOCX文件中"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)使将一个DOCX文件插入到另一个文件中成为可能，提供可自定义的选项。
      
      1. 设计一个包含内容占位符的DOCX模板。
      2. 设置模板的文件路径。
      3. 提供要合并的文档的文件路径。
      4. 导出包含合并内容的最终文件。
   
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
        // 将此标签插入模板中以定义文档嵌入的位置
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 设置主模板的文件路径
        const template = "doc_template.docx";

        // 提供要合并文档的路径
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // 将最终输出文件保存为嵌入的文档
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "强大的文档集成工具"
  description: "GroupDocs.Assembly for Node.js via Java简化了跨各种格式嵌入文件的过程，并实现了完全自定义。每次都能提供一致且专业的结果。"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的主要特性"
  features:
    # feature loop
    - title: "使用业务数据生成报告"
      content: "从JSON、XML或CSV源提取数据，快速而准确地创建综合报告和文档。"

    # feature loop
    - title: "添加丰富的视觉元素"
      content: "GroupDocs.Assembly允许您在文本和超链接旁边包括表格、图表、列表、图像和条形码。"

    # feature loop
    - title: "精确的数据位置"
      content: "使用LINQ模板准确定位数据，处理数组等重复项，并轻松自定义样式。"

    # feature loop
    - title: "支持多种格式"
      content: "在PDF、MS Office文件、HTML和OpenOffice等格式之间无缝合并内容，为所有项目提供灵活性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "以编程方式将图像嵌入文档中"
      content: |
        此示例演示如何使用GroupDocs.Assembly将图像插入到DOCX文件中。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 在模板中添加图像的占位符
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 指定模板文件的路径
          const template = "template.docx";

          // 设置要嵌入的图像路径
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // 初始化DocumentAssembler对象
          const asm = new assemblyLib.DocumentAssembler();

          // 保存包含图像的文档
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "核心功能一览"
    exclude: "document"
    description: "探索GroupDocs.Assembly为高效和无缝文档合并提供的全面工具。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "合并多种格式的文档"
    exclude: "DOCX"
    description: "使用Node.js via Java在50多种文件格式中合并内容，确保专业和精致的结果。"
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