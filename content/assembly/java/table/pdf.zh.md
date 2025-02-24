



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: zh
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用Java向PDF文档添加表格"
head_description: "借助GroupDocs.Assembly for Java，开发人员可以快速将表格集成到文档和电子邮件中，从动态数据源中提取数据。"

############################# Header ############################
title: "使用我们的Java API 轻松填充PDF文件中的表格" 
description: "GroupDocs.Assembly for Java简化了从各种输入填充PDF文档中表格的过程。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即获取免费试用"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java是什么？"
    link: "/assembly/java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)是一种通过自动将数据插入预设计模板来生成文档和报告的工具。您可以轻松添加表格、列表、图表和图片。其先进的功能使您能够精确放置文档中的内容。兼容超过50种文件类型，包括PDF、MS Office和电子邮件格式。

############################# Steps ############################
steps:
    enable: true
    title: "将数据插入PDF表格的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/java/)帮助您为PDF和其他格式填充表格模板。使用来自您的源的动态数据创建表格。
      
      1. 设计一个带有表格占位符的模板（目前不支持PDF模板）。
      2. 从任何支持的输入源提取数据。
      3. 过滤或预处理数据以符合您的需求。
      4. 将文档保存为填充了表格的PDF文件。
   
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
        // 在模板中的表格行占位符中使用这些标签
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // 定义模板文件的路径
        // 目前不支持PDF模板。
        String template = "table_template.docx";

        // 从所选源加载数据
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // 将输出文件保存为填充后的表格
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "创建包含数据填充表格的文档"
  description: "GroupDocs.Assembly for Java使自动创建文档中的表格变得简单。它还支持使用模板添加图表、列表和图像等元素。"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的主要特性"
  features:
    # feature loop
    - title: "从多种数据格式生成报告"
      content: "该API与JSON、XML、CSV和其他格式无缝协作，以便用有序数据填充文档中的表格。"

    # feature loop
    - title: "以视觉方式呈现信息"
      content: "GroupDocs.Assembly帮助您构建专业的表格、列表和图表，以及插入链接、文本和图像，使外观更加美观。"

    # feature loop
    - title: "精确放置表格内容"
      content: "使用灵活的基于LINQ的语法动态添加行和列。通过编程自定义外观，例如字体样式和颜色。"

    # feature loop
    - title: "兼容多种格式"
      content: "与MS Office、OpenOffice、PDF、HTML等格式兼容。可轻松将表格合并到任何支持的文件格式中。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "动态创建数据填充表格"
      content: |
        本示例展示了如何使用动态输入数据填充PDF文档中的表格。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 设计一个带有表格占位符的模板
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // 设置模板文件位置
          // 目前不支持PDF模板。
          String template = "table_template.docx";

          // 从您首选的源加载数据
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 准备一个包含所需字段的数据对象
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // 创建DocumentAssembler的实例
          DocumentAssembler asm = new DocumentAssembler();

          // 保存填充了表格的文档
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    title: "功能一览"
    exclude: "table"
    description: "我们的API通过自动化表格内容填充以及其他强大组件，简化了专业文档的创建。"
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
    title: "以多种格式生成详细表格"
    exclude: "PDF"
    description: "通过Java，您可以使用数据填充模板，并在超过50种文件类型中生成详细报告。"
    items: 
          
        # format loop 1
        - name: "在PDF中添加表格"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中添加表格"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中添加表格"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中添加表格"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---