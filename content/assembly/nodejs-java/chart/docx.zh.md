



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:00
draft: false
lang: zh
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在DOCX文件中插入图表，使用JavaScript"
head_description: "借助GroupDocs.Assembly for Node.js via Java，开发人员可以快速创建和嵌入动态图表到文档中，并使用实时数据源。"

############################# Header ############################
title: "使用Node.js轻松将图表添加到DOCX文件中" 
description: "GroupDocs.Assembly for Node.js via Java简化了将图表集成到含有实时数据输入的DOCX文档中的过程。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即免费开始"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java概述"
    link: "/assembly/nodejs-java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)是一个强大的解决方案，用于创建自动化文档和报告。精确和简便地向文件中添加图表、表格、图像、条形码和列表。这个多功能平台支持超过50种格式，包括PDF、Office文档和电子邮件。

############################# Steps ############################
steps:
    enable: true
    title: "将图表添加到DOCX文档的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)使将图表添加到DOCX文件变得简单。选择条形图、折线图或饼图等图表类型。
      
      1. 设计一个带有图表占位符的DOCX模板。
      2. 从支持的来源加载数据。
      3. 配置图表选项，包括类型、颜色和标签。
      4. 导出带有嵌入图表的文档。
   
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
        // 在模板中包含此标签以生成图表
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 指定模板文件路径
        const template = "chart_template.docx";

        // 从源系统提取数据
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // 保存最终文档并嵌入图表
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "轻松在文档中嵌入图表"
  description: "GroupDocs.Assembly for Node.js via Java使您能够在流行文件类型中生成功能丰富的文档。使用模板向文档中添加图表、表格、条形码、列表、图像等，并提供实时数据更新。"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的主要功能"
  features:
    # feature loop
    - title: "将数据转换为专业图表"
      content: "将来自JSON、XML或CSV等源的数据转换为可以直接嵌入文档的高质量图表。"

    # feature loop
    - title: "创建令人惊叹的视觉效果"
      content: "生成与其他文档元素（如图像、表格和条形码）无缝配合的条形图、饼图和折线图。"

    # feature loop
    - title: "灵活的图表样式和布局"
      content: "使用LINQ模板来控制图表的位置和样式，包括颜色、布局和标签，实现精美的展示效果。"

    # feature loop
    - title: "支持多种文件格式"
      content: "生成MS Office、PDF、OpenOffice和HTML等格式的文档，其中图表完美嵌入，展现专业的效果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "动态生成和插入图表"
      content: |
        本示例展示如何通过编程方式创建并嵌入图表到DOCX文件中。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 建立一个带有图表占位符的模板
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 定义模板文件的路径
          const template = "table_template.docx";

          // 从选定的来源检索数据
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // 准备一个包含图表信息的数据对象
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // 选择图表类型并自定义其外观
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // 初始化DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // 保存包含嵌入图表的更新文档
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "发现高级功能"
    exclude: "chart"
    description: "该平台通过旨在数据可视化和无缝集成的工具简化了文档的创建过程。"
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
    title: "生成多种文件格式的报告"
    exclude: "DOCX"
    description: "Node.js via Java支持超过50种格式，轻松将模板与数据结合以制作精美文件。"
    items: 
          
        # format loop 1
        - name: "在PDF中插入图表"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中插入图表"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中插入图表"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中插入图表"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---