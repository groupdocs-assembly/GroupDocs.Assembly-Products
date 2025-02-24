



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: zh
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 在 PPTX 文档中生成图表"
head_description: "GroupDocs.Assembly for Java API 使开发人员能够无缝地创建并插入动态图表或图形到文档中，依赖于实时数据。"

############################# Header ############################
title: "使用 Java API 将图表添加到 PPTX 文档中" 
description: "GroupDocs.Assembly for Java 通过利用实时数据简化了将图表嵌入 PPTX 文档的过程。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费开始"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) 是一个多功能解决方案，用于自动化文档和报告的创建。它使您能够将图表、表格、列表、条形码和图像直接添加到文件中，并提供用于精准格式化和数据集成的高级工具。该平台支持超过 50 种格式，包括 PDF、Microsoft Office 文件和电子邮件。

############################# Steps ############################
steps:
    enable: true
    title: "将图表嵌入 PPTX 文档的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/java/) 简化了在 PPTX 模板中插入图表的过程。可选择多种图表样式，包括条形图、饼图和折线图。
      
      1. 创建一个包含图表占位符的 PPTX 模板。
      2. 从兼容的源加载数据。
      3. 设置图表选项，例如类型、标签和颜色。
      4. 保存包含图表的文档。
   
    code:
      platform: "java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "示例文档"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // 在模板中添加此标签以包括图表
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // 提供模板的文件路径
        String template = "chart_template.pptx";

        // 从源中提取必要的数据
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // 保存包含嵌入图表的最终文档
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "轻松地在文档中嵌入动态图表"
  description: "GroupDocs.Assembly for Java 提供了一种便捷的方式来构建数据丰富的流行格式文档。使用模板插入图表、表格、条形码、列表、链接和图像，并利用实时数据进行动态更新。"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 的关键特点"
  features:
    # feature loop
    - title: "简单将数据转换为图表"
      content: "使用 API 将来自 JSON、XML、CSV 或其他源的数据转换为干净专业的图表，以便插入您的文档。"

    # feature loop
    - title: "创建视觉冲击力强的内容"
      content: "GroupDocs.Assembly 支持多种视觉格式，包括条形图、饼图和折线图，可以与表格、条形码、图像等结合使用，以增强报告的效果。"

    # feature loop
    - title: "可自定义的图表位置和样式"
      content: "借助基于 LINQ 的语法，您可以动态生成并定位文档中的图表，同时轻松调整样式、颜色和布局以满足设计需求。"

    # feature loop
    - title: "支持多种文档格式"
      content: "生成 MS Office、PDF、OpenOffice 和 HTML 格式的文档。所生成的图表可以无缝整合到任何受支持的格式中，以获得专业的效果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "以编程方式生成并嵌入图表"
      content: |
        该示例演示了如何以编程方式创建并嵌入图表到 PPTX 文档中。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 准备一个模板，其中包含图表的占位符
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // 指定模板的文件路径
          String template = "table_template.pptx";

          // 从所选源加载数据
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 创建一个包含相关信息的数据对象
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // 配置图表的类型和外观
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // 初始化 DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // 保存完成的文档，其中包含嵌入的图表
          asm.assembleDocument(template, "result.pptx", data, design);
          ```
        platform: "java"
        copy_title: "复制"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费探索GroupDocs.Assembly的功能或请求许可证"
  items:
    #  loop
    - title: "从Maven下载"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "了解许可证信息"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "探索强大的功能"
    exclude: "chart"
    description: "该平台简化了设计以数据为中心、视觉吸引人的文档的过程，满足您的需求。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在多种格式中生成综合报告"
    exclude: "PPTX"
    description: "Java 允许您在超过 50 种文件格式中创建集成图表的文档，确保模板和数据的无缝合并。"
    items: 
          
        # format loop 1
        - name: "在PDF中插入图表"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中插入图表"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中插入图表"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中插入图表"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---