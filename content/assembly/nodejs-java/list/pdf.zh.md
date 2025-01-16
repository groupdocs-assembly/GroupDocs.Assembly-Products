



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: zh
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用JavaScript在PDF中创建动态列表"
head_description: "使用GroupDocs.Assembly for Node.js via Java API 轻松设计和插入列表到PDF模板中。"

############################# Header ############################
title: "在PDF文件中嵌入数据驱动的列表，使用Node.js" 
description: "GroupDocs.Assembly for Node.js via Java提供强大的工具，将灵活的数据驱动列表添加到PDF文档中。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费开始使用"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "关于GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)通过从各种数据源提取数据并嵌入到模板中，简化了文档创建。使用它构建列表、表格、图表及其他元素，具有精确的放置和格式选项。支持50多种格式，包括PDF、MS Office和电子邮件，帮助您自动化文档生成过程。

############################# Steps ############################
steps:
    enable: true
    title: "在PDF文件中插入列表的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)使您可以轻松地将详细的数据驱动列表添加到您的PDF模板中。
      
      1. 设计一个带有列表占位符的模板（PDF模板不受支持）。
      2. 提供模板的文件路径。
      3. 从支持的源（如JSON或XML）加载数据。
      4. 将带有列表的完成文档导出为PDF文件。
   
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
        // 在模板中放置此标签以标记列表的位置
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 设置模板的文件路径
        // 当前不支持PDF模板。
        const template = "list_template.docx";

        // 从所需的数据源获取数据
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // 保存带有嵌入列表的文件
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "轻松生成带有集成数据的文档"
  description: "使用GroupDocs.Assembly for Node.js via Java，您可以将列表、表格、图表及其他元素嵌入到模板中，节省时间和精力。"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 的亮点"
  features:
    # feature loop
    - title: "从多个数据源生成报告"
      content: "从JSON、XML、CSV等格式导入数据，以高效填充列表和其他组件。"

    # feature loop
    - title: "添加列表和其他视觉元素"
      content: "GroupDocs.Assembly 允许您与文本、图像和链接无缝嵌入列表、表格、图表等，达到精美效果。"

    # feature loop
    - title: "精确放置和样式化数据"
      content: "基于LINQ的模板让您可以精确控制列表和其他数据的位置，使用循环处理重复项，并根据需求自定义样式。"

    # feature loop
    - title: "跨多种格式工作"
      content: "创建MS Office、PDF、OpenOffice、HTML及电子邮件等格式的文档。将来自多个源的内容合并到单一文件中。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "以编程方式在文档中创建列表"
      content: |
        此示例演示如何使用GroupDocs.Assembly动态添加列表到PDF文档中。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 在模板中为列表添加占位符
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 指定模板的文件路径
          // 当前不支持PDF模板。
          const template = "numlist_template.docx";

          // 加载数据以填充列表
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // 准备包含所需详情的数据源
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // 初始化DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // 保存包含列表的最终文档
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "探索GroupDocs.Assembly的功能"
    exclude: "list"
    description: "利用强大的集成工具，轻松设计和生成数据丰富的文档。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "以多种格式创建文档"
    exclude: "PDF"
    description: "Node.js via Java支持50多种文件格式，方便将模板和数据合并成专业的结果。"
    items: 
          
        # format loop 1
        - name: "在PDF中创建列表"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中创建列表"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中创建列表"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中创建列表"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---