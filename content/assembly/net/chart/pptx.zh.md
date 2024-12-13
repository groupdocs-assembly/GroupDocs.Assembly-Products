



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: zh
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用 C# 在 PPTX 文件中创建图表"
head_description: "GroupDocs.Assembly for .NET API 使开发人员能够动态地使用实时数据生成并插入图表或图形到文档中。"

############################# Header ############################
title: "通过 .NET API 在 PPTX 文件中嵌入图表" 
description: "GroupDocs.Assembly for .NET 提供了一种强大的方法可以用动态数据填充 PPTX 文件，并轻松集成图表。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费试用"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "什么是 GroupDocs.Assembly for .NET？"
    link: "/assembly/net/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) 是一种旨在通过整合来自各种来源的数据来简化文档和报告创建的工具。动态生成图表、表格、列表、条形码和图像。先进的格式选项允许准确定位和自定义内容。它支持超过 50 种文件格式，包括 PDF、MS Office 文档和电子邮件。

############################# Steps ############################
steps:
    enable: true
    title: "如何向 PPTX 文档添加图表"
    content: |
      [GroupDocs.Assembly](/assembly/net/) 使生成并嵌入图表到您的 PPTX 模板中变得简单。支持多种图表类型，如条形图、饼图和折线图。
      
      1. 设计一个 PPTX 模板，留出图表的位置。
      2. 从兼容的来源获取数据。
      3. 定义图表选项，如类型、标签和配色方案。
      4. 保存更新后的文件，并嵌入图表。
   
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
        // 在您的模板中包含此标签以生成图表
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // 指定您的模板文件路径
        string template = "chart_template.pptx";

        // 从您首选的来源加载数据
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // 保存嵌入图表的文档
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "轻松向文档添加动态图表"
  description: "GroupDocs.Assembly for .NET 简化了在广泛使用的格式中创建数据驱动文档的过程。使用模板插入图表、表格、条形码、列表、超链接和图像，进行高级动态数据集成。"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 的主要功能"
  features:
    # feature loop
    - title: "将数据转换为专业图表"
      content: "借助我们的 API，只需几个步骤即可将来自 JSON、XML、CSV 和其他源的数据转换为视觉吸引力十足的图表。"

    # feature loop
    - title: "创建视觉上吸引人的内容"
      content: "GroupDocs.Assembly 支持多种图表类型，如条形图、饼图和折线图。将这些与表格、条形码、图像和其他元素结合，创建专业报告。"

    # feature loop
    - title: "精确定位和自定义图表"
      content: "使用 LINQ 语法，可以动态生成并在所需位置放置图表。轻松自定义样式、颜色和布局，以满足您的需求。"

    # feature loop
    - title: "支持多种文件格式"
      content: "生成流行格式的文档，如 MS Office、PDF、OpenOffice 和 HTML。无缝嵌入图表到任何受支持的格式中，确保完全兼容。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "以编程方式创建图表"
      content: |
        此示例演示了如何动态创建并将图表嵌入到 PPTX 文档中。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 准备一个带有图表占位符的模板
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // 提供模板文件的路径
          string template = "table_template.pptx";

          // 从您的数据源获取数据
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 构建一个包含必要信息的数据对象
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // 设置图表属性，如类型和外观
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // 初始化 DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // 导出包含图表的文档
          asm.AssembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "探索关键功能"
    exclude: "chart"
    description: "我们的平台帮助您创建引人注目的、数据驱动的文档，满足您的需求。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "以多种格式创建视觉丰富的报告"
    exclude: "PPTX"
    description: ".NET 允许您在超过 50 种支持的格式中生成带有集成图表的文档，完美结合模板和您的数据。"
    items: 
          
        # format loop 1
        - name: "在PDF中插入图表"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中插入图表"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中插入图表"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中插入图表"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---