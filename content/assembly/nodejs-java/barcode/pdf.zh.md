



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: zh
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用 JavaScript 在 PDF 文件中添加条形码"
head_description: "使用 GroupDocs.Assembly for Node.js via Java API 轻松生成并嵌入条形码到您的文档和电子邮件中。"

############################# Header ############################
title: "使用 Node.js 创建 PDF 文件的条形码" 
description: "借助 GroupDocs.Assembly for Node.js via Java，您可以动态生成、定制并嵌入条形码到 PDF 文档中。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "开始使用"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Assembly for Node.js via Java 的介绍"
    link: "/assembly/nodejs-java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) 允许您通过结合多个来源的数据来创建专业文档。将图表、表格、列表、图像和条形码添加到您的文件中。使用模板将内容组织到恰当的位置。支持超过 50 种格式，包括 PDF、Office 文档和电子邮件。

############################# Steps ############################
steps:
    enable: true
    title: "在 PDF 文件中添加条形码的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) 使得在 PDF 文档中嵌入条形码变得简单。它支持超过 60 种条形码类型，包括 1D 和 2D 格式。
      
      1. 设计一个带有条形码占位符的模板（PDF 模板不受支持）。
      2. 从兼容的源获取数据。
      3. 设置条形码选项，如大小和分辨率。
      4. 将文档导出为带有条形码的 PDF 文件。
   
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
        // 在模板中使用此标签以在输出文档中包含条形码
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 指定模板文件的路径
        // 注意：当前不支持 PDF 模板。
        const template = "barcode_template.docx";

        // 从源获取所需数据
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // 将文档导出为带有条形码的 PDF 文件。
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "使用数据驱动的模板生成文档"
  description: "借助 GroupDocs.Assembly for Node.js via Java，您可以通过无缝嵌入图表、表格、列表、链接、图像和条形码，以专业的格式创建文件。"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 的核心功能"
  features:
    # feature loop
    - title: "使用业务数据生成报告"
      content: "使用 API 快速准确地用 JSON、XML 和 CSV 等格式的数据填充模板。"

    # feature loop
    - title: "添加视觉元素"
      content: "GroupDocs.Assembly 支持实时插入图表、表格、列表、文本、链接、图像和条形码等元素。"

    # feature loop
    - title: "控制数据位置"
      content: "使用基于 LINQ 的模板，您可以精确定位数据，循环处理数组，并以编程方式应用自定义格式。"

    # feature loop
    - title: "兼容多种格式"
      content: "处理如 MS Office 文档、PDF、HTML、OpenOffice 文件和电子邮件等文件。按需合并多个文档。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "示例：以编程方式生成条形码"
      content: |
        此示例演示如何以编程方式生成并插入条形码到 PDF 文档中。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 设计一个带有条形码占位符的模板
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 指定模板文件的路径
          // 注意：当前不支持 PDF 模板。
          const template = "barcode_template.docx";

          // 从您的源获取数据
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // 创建一个包含所需详细信息的数据源对象
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // 初始化 DocumentAssembler 的实例
          const asm = new assemblyLib.DocumentAssembler();

          // 设置条形码配置
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // 保存包含条形码的文档
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "探索主要功能"
    exclude: "barcode"
    description: "通过先进的工具和自动化功能简化文档处理。"
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
    title: "报告创建支持的文件格式"
    exclude: "PDF"
    description: "Node.js via Java 处理超过 50 种文件类型，使得合并数据和处理模板以获得高质量结果变得简单。"
    items: 
          
        # format loop 1
        - name: "在PDF中添加条形码"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中添加条形码"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中添加条形码"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中添加条形码"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---