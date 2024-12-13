



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:57
draft: false
lang: zh
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用C#在XLSX文档中创建表格"
head_description: "GroupDocs.Assembly for .NET API允许开发人员轻松地将数据从动态源添加并填充到文档和电子邮件中的表格。"

############################# Header ############################
title: "使用我们的.NET API生成XLSX文档中的数据表" 
description: "GroupDocs.Assembly for .NET使您能够动态地用来自各种源的数据填充XLSX文档中的表格。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载免费试用"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET概述"
    link: "/assembly/net/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)旨在通过用来自多个源的数据填充模板来创建文档和报告。轻松将结构化数据插入表格、列表和图表中，或动态嵌入图像。高级语法确保数据的准确放置。支持超过50种格式，包括PDF、MS Office文档和电子邮件文件。

############################# Steps ############################
steps:
    enable: true
    title: "如何在XLSX文档中填充表格"
    content: |
      [GroupDocs.Assembly](/assembly/net/)允许您在XLSX等格式的模板中动态填充表格。从各种源中插入数据到您的表格中。
      
      1. 创建一个带有表格占位符的XLSX模板。
      2. 从任何支持的源获取数据。
      3. 过滤数据以只包括所需的信息。
      4. 保存填充了表格的文档。
   
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
        // 将这些标签添加到模板表格行中
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // 设置模板的文件路径
        string template = "table_template.xlsx";

        // 从支持的源中获取数据
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // 保存填充数据的表格文档
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "生成动态表格的文档"
  description: "GroupDocs.Assembly for .NET通过自动填充表格和支持其他元素（如图表、列表和图像）的模板和高级标记简化了文档的创建。"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的关键特性"
  features:
    # feature loop
    - title: "从结构化数据创建报告"
      content: "API有效且准确地处理来自JSON、XML和CSV等源的数据，以填充办公文档中的表格。"

    # feature loop
    - title: "以可视化方式显示数据"
      content: "GroupDocs.Assembly支持创建表格、列表和图表，同时嵌入文本、链接和图像，以实现专业文档设计。"

    # feature loop
    - title: "精准定位表格数据"
      content: "使用基于LINQ的语法动态添加表格行和列。可以通过编程自定义样式，包括颜色和格式。"

    # feature loop
    - title: "支持广泛的格式"
      content: "轻松处理流行文件格式，如MS Office、OpenOffice、PDF和HTML。无缝地将填充的表格插入支持的文档类型中。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何动态填充数据表"
      content: |
        此示例演示了如何使用动态数据填充XLSX文档中的表格。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 准备一个带有表格占位符的模板
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // 指定模板的文件路径
          string template = "table_template.xlsx";

          // 从您选择的源检索数据
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 创建一个包含所需数据的数据源对象
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // 初始化DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // 保存填充了表格的完整文档
          asm.AssembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_table.xlsx"
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
    title: "探索关键特性"
    exclude: "table"
    description: "我们的解决方案通过动态填充表格和其他元素，简化了专业文档的创建。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "创建详细表格的报告"
    exclude: "XLSX"
    description: ".NET通过在超过50种支持的格式中用表格和其他数据元素填充模板，实现全面报告的生成。"
    items: 
          
        # format loop 1
        - name: "在PDF中添加表格"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中添加表格"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中添加表格"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中添加表格"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---