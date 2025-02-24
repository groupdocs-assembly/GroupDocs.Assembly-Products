



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: zh
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用C#生成PPTX文档中的列表"
head_description: "GroupDocs.Assembly for .NET API使开发人员能够动态创建并嵌入数据填充的列表到文档和模板中。"

############################# Header ############################
title: "使用我们的.NET API将数据驱动的列表添加到PPTX文档中" 
description: "GroupDocs.Assembly for .NET提供强大的工具，以动态生成并嵌入列表到PPTX文档中。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载试用"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET概述"
    link: "/assembly/net/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)旨在通过无缝集成来自各种源的数据来简化文档和报告的创建。使用列表、图表、表格、条形码或文本填充模板，并利用高级标记精确放置内容。支持超过50种格式，包括PDF、MS Office文件和电子邮件，非常适合自动化文档工作流。

############################# Steps ############################
steps:
    enable: true
    title: "将数据填充的列表添加到PPTX文档的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/net/)使得将数据驱动的列表插入到PPTX模板中变得简单。创建并自定义列表。
      
      1. 准备一个包含列表占位符的PPTX模板。
      2. 设置模板的路径。
      3. 从支持的源中检索数据，如JSON或XML。
      4. 保存包含嵌入列表的最终文档。
   
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
        // 将此标签添加到您的模板中，以标记列表将出现的位置
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // 指定模板文件的路径
        string template = "list_template.pptx";

        // 从您选择的源中检索数据
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 保存生成列表的文档
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过用结构化数据填充模板来创建文档"
  description: "GroupDocs.Assembly for .NET简化了构建数据驱动文档的过程。动态地添加列表、表格、条形码、图表、图像和其他元素，使用高级模板。"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 特性"
  features:
    # feature loop
    - title: "从业务数据生成报表"
      content: "该API使用JSON、XML、CSV等来源的数据，以精准和高效的方式填充流行格式的文档。"

    # feature loop
    - title: "使用列表和其他元素展示数据"
      content: "GroupDocs.Assembly使您能够嵌入列表、表格和图表，结合文本、条形码、超链接和图像，创建结构良好的文档。"

    # feature loop
    - title: "精确插入所需数据"
      content: "利用基于LINQ的语法精确定位列表和其他数据元素。使用循环动态填充列表，并以编程方式应用自定义格式。"

    # feature loop
    - title: "支持多种文档格式"
      content: "生成和管理多种格式的文档，如MS Office、OpenOffice、PDF、HTML和邮件文件。轻松将多个文档合并为一个。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何动态生成列表"
      content: |
        此示例演示如何将动态生成的列表嵌入到PPTX文档中。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 为列表在模板中添加占位符标签
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // 指定模板文件的路径
          string template = "numlist_template.pptx";

          // 检索数据以填充列表
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // 创建一个包含必要信息的数据源对象
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // 初始化DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // 保存生成列表的最终文档
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    exclude: "list"
    description: "我们的平台旨在简化创建和集成数据驱动文档内容的过程。"
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
    title: "在流行格式中创建结构化文档"
    exclude: "PPTX"
    description: ".NET支持超过50种格式，使您能够无缝合并数据和模板，以生成洗练且结构良好的结果。"
    items: 
          
        # format loop 1
        - name: "在PDF中创建列表"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中创建列表"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中创建列表"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中创建列表"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---