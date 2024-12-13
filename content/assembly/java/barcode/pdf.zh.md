



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:52
draft: false
lang: zh
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "在 PDF 文件中嵌入条形码，使用 Java"
head_description: "GroupDocs.Assembly for Java API 使您能够实时创建和插入条形码图像到文档和电子邮件中。"

############################# Header ############################
title: "使用我们的 Java API 为 PDF 文件生成条形码" 
description: "GroupDocs.Assembly for Java 提供全面的工具，以动态创建、自定义并嵌入条形码到 PDF 文件中。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即下载"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java 是什么？"
    link: "/assembly/java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) 帮助您通过从多个来源添加数据来生成和自定义文档。插入文本、数字、图表、表格、列表、图像和条形码。使用高级模板确保数据准确显示在您想要的位置。支持超过 50 种格式，包括 PDF、Office 文件和电子邮件。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 PDF 文档中嵌入条形码"
    content: |
      [GroupDocs.Assembly](/assembly/java/) 允许您将条形码插入流行格式如 PDF 的模板中。支持超过 60 种类型，包括 1D 和 2D 条形码。
      
      1. 准备一个带有条形码占位符的模板（不支持 PDF 模板）。
      2. 从支持的源中获取数据。
      3. 调整条形码设置，如大小和分辨率。
      4. 将添加条形码的文档保存为 PDF 文件。
   
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
        // 在模板中使用此标签以在输出文档中创建条形码
        // <<barcode [barcode_expression] -barcode_type>>

        // 设置模板的文件路径
        // 目前不支持 PDF 模板。
        String template = "barcode_template.docx";

        // 从您的数据源获取数据
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 将添加条形码的文档保存为 PDF 文件。
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "使用数据驱动的模板构建文档"
  description: "GroupDocs.Assembly for Java 简化了流行文件类型的文档创建。使用模板无缝添加图表、表格、列表、链接、图像和条形码。"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 的功能"
  features:
    # feature loop
    - title: "使用业务数据生成报告"
      content: "API 能够高效且准确地使用 JSON、XML 和 CSV 等格式中的数据填充文档。"

    # feature loop
    - title: "使用内置元素可视化数据"
      content: "GroupDocs.Assembly 支持本地元素，如表格、图表和列表，以及文本、链接、图像和实时条形码生成。"

    # feature loop
    - title: "将数据插入所需位置"
      content: "通过基于 LINQ 的模板，您可以精准放置数据，使用循环添加数组，并以编程方式定制格式（如颜色）。"

    # feature loop
    - title: "与文件类型兼容性广泛"
      content: "处理 MS Office 文档、PDF、HTML、OpenOffice 和电子邮件等文件。您还可以将一个文档合并到另一个文档中。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何动态创建条形码"
      content: |
        此示例演示了如何动态生成并将条形码添加到 PDF 文档中。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 准备一个带有条形码占位符的模板
          // <<barcode [barcode_expression] -barcode_type>>

          // 设置模板文件的路径
          // 目前不支持 PDF 模板。
          String template = "barcode_template.docx";

          // 从特定源加载数据
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // 构建一个包含必要数据的数据源对象
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // 创建 DocumentAssembler 实例
          DocumentAssembler asm = new DocumentAssembler();

          // 自定义条形码设置
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // 保存更新的文档并包含条形码
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "发现关键特性"
    exclude: "barcode"
    description: "我们的平台通过强大的工具和自动化，简化了文档处理。"
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "以各种格式创建报告"
    exclude: "PDF"
    description: "Java 支持超过 50 种文件类型，使数据合并和模板处理变得轻松，从而实现专业的结果。"
    items: 
          
        # format loop 1
        - name: "在PDF中添加条形码"
          format: "PDF"
          link: "/assembly/java/barcode/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中添加条形码"
          format: "DOCX"
          link: "/assembly/java/barcode/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中添加条形码"
          format: "PPTX"
          link: "/assembly/java/barcode/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中添加条形码"
          format: "XLSX"
          link: "/assembly/java/barcode/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---