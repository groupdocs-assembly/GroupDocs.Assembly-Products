



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:05
draft: false
lang: zh
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在PDF文档中插入表格，使用JavaScript"
head_description: "利用GroupDocs.Assembly for Node.js via Java快速在文档或电子邮件中嵌入表格，从各种数据源提取数据。"

############################# Header ############################
title: "轻松添加表格到PDF文件，使用Node.js" 
description: "借助GroupDocs.Assembly for Node.js via Java，在PDF文档中填充表格变得简便，可以从多个数据源获取数据。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "开始您的免费试用"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java简介"
    link: "/assembly/nodejs-java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) 是一个强大的文档创建自动化工具。它允许您精确地在模板中插入表格、图表、列表和图像，支持超过50种文件格式，包括PDF、Word和电子邮件，简化报告生成及其他任务。

############################# Steps ############################
steps:
    enable: true
    title: "如何在PDF中向表格添加数据"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)使您能够快速使用动态数据源填充PDF文件的表格模板。
      
      1. 创建一个含有表格占位符的模板（不支持PDF模板）。
      2. 从支持的源加载数据，如JSON或CSV。
      3. 根据需要组织和格式化数据。
      4. 将填充的表格导出为PDF文件的文档。
   
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
        // 在您的模板的表格行占位符中包含这些标签
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 指定模板文件路径
        // 目前不支持PDF模板。
        const template = "table_template.docx";

        // 从选定的源加载数据
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // 保存包含完整表格的最终文档
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "轻松将数据驱动的表格添加到文档中"
  description: "GroupDocs.Assembly for Node.js via Java允许用户自动创建表格，同时使用基于模板的工作流程嵌入图表、图像和列表。"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的主要特点"
  features:
    # feature loop
    - title: "从结构化数据生成表格"
      content: "从JSON、XML、CSV等格式提取数据，自动填充文档表格。"

    # feature loop
    - title: "创建精美的视觉内容"
      content: "使用GroupDocs.Assembly设计专业表格、图表和列表，并为文档添加链接、图像和文本，以提升文档外观。"

    # feature loop
    - title: "动态表格内容布局"
      content: "使用基于LINQ的模板程序化添加行和列，并自定义字体、颜色和对齐等样式。"

    # feature loop
    - title: "在多种格式中无缝工作"
      content: "轻松在MS Office、OpenOffice、PDF、HTML等格式中创建或编辑表格，按需将其合并到文件中。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何程序化填充表格"
      content: |
        此示例演示如何从外部源填充PDF文档中的表格。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 设计一个含有表格占位符的模板
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 指定模板的文件路径
          // 目前不支持PDF模板。
          const template = "table_template.docx";

          // 从源加载所需的数据
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // 组织数据成必要结构
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // 初始化DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // 保存包含完整表格的输出文档
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    exclude: "table"
    description: "我们的API自动化表格创建，使用多功能工具和模板增强文档生成。"
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
    title: "在各种格式中生成表格"
    exclude: "PDF"
    description: "使用Node.js via Java，填充模板并在超过50种支持的文件类型中创建全面的表格。"
    items: 
          
        # format loop 1
        - name: "在PDF中添加表格"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中添加表格"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中添加表格"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中添加表格"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---