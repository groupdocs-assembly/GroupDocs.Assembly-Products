



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: zh
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "利用 C# API 将一个文档嵌入到另一个 DOCX 中"
head_description: "使用 C# 合并 DOCX 文档。有了 GroupDocs.Assembly，只需几个步骤即可无缝组合文件。"

############################# Header ############################
title: "在 DOCX 格式中合并文档" 
description: "使用 GroupDocs.Assembly for .NET，您可以快速将一个 DOCX 文档嵌入到另一个文档中。该 API 提供强大的工具来实现精确的文档合并。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET 是什么？"
    link: "/assembly/net/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) 是一种强大的文档组合和处理工具。它允许用户将一个文档嵌入到另一个文档中，从而实现内容的无缝合并。支持超过 50 种格式，包括 PDF、MS Office 文件等，您可以组织、编辑并自定义最终输出以满足您的需求。

############################# Steps ############################
steps:
    enable: true
    title: "如何将文档合并到 DOCX 文件中"
    content: |
      [GroupDocs.Assembly](/assembly/net/) 允许您轻松将一个文档嵌入到另一个 DOCX 文件中。合并并自定义内容。
      
      1. 设计一个 DOCX 模板，包含用于嵌入文档的占位符。
      2. 定义模板的文件路径。
      3. 指定要嵌入的文档的文件路径。
      4. 保存最终文件，包含嵌入的内容。
   
    code:
      platform: "net"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "示例文档"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // 在模板中添加此标签以标记插入点
        // <<doc [doc_expression]>>

        // 指定模板的文件路径
        string template = "doc_template.docx";

        // 提供要嵌入文档的路径
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // 保存合并后的文档
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "利用高级工具简化文档合并"
  description: "GroupDocs.Assembly for .NET 库简化了将一个文档嵌入到另一个文档中的过程，支持多种文件格式并提供无缝集成的自定义选项。"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 的主要特性"
  features:
    # feature loop
    - title: "根据业务数据生成报告"
      content: "自动使用来自 JSON、XML、CSV 或其他来源的数据填充文档，确保工作流的准确性和高效性。"

    # feature loop
    - title: "为文档增添视觉元素"
      content: "GroupDocs.Assembly 允许您包含表格、图表和列表，以及文本、链接、图像和动态生成的条形码。"

    # feature loop
    - title: "精确放置和格式化数据"
      content: "基于 LINQ 的模板让您控制数据的放置，处理数组循环，并允许颜色等样式的自定义。"

    # feature loop
    - title: "支持多种文件格式"
      content: "轻松地在 MS Office、PDF、HTML、OpenOffice 等格式之间嵌入文档。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何以编程方式将图像嵌入文档"
      content: |
        此示例演示如何使用 GroupDocs.Assembly 将图像插入到 DOCX 文档中。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 在模板中添加一个占位符标签
          // <<image [expression]>>

          // 指定模板的文件路径
          string template = "template.docx";

          // 设置图像文件的路径
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // 初始化一个 DocumentAssembler 实例
          DocumentAssembler asm = new DocumentAssembler();

          // 保存包含嵌入图像的文档
          asm.AssembleDocument(template, "result.docx", data);
          ```
        platform: "net"
        copy_title: "复制"
        install:
          command: "dotnet add package GroupDocs.Assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费探索GroupDocs.Assembly的功能或请求许可证"
  items:
    #  loop
    - title: "从Nuget下载"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "了解许可证信息"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "发现我们强大的工具"
    exclude: "document"
    description: "探索 GroupDocs.Assembly 提供的精准嵌入和合并文档的功能。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "合并多种格式的文档"
    exclude: "DOCX"
    description: "使用 .NET API，您可以在超过 50 种支持的格式之间合并文档。轻松将文件或部分嵌入到最终文档中。"
    items: 
          
        # format loop 1
        - name: "在PDF中嵌入文档"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中嵌入文档"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中嵌入文档"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中嵌入文档"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---