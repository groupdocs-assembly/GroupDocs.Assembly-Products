



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:09
draft: false
lang: zh
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用Java在PPTX文档中创建列表"
head_description: "使用GroupDocs.Assembly for Java API设计和嵌入动态列表到您的PPTX模板中。"

############################# Header ############################
title: "通过我们的Java API向PPTX文件添加动态列表" 
description: "GroupDocs.Assembly for Java提供灵活的工具，可以直接在PPTX文档中生成和插入数据丰富的列表。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费试用"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java是什么？"
    link: "/assembly/java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)使通过从多个来源提取数据来设计专业文档变得简便。使用它创建列表、表格、图表或文本，并使用高级模板功能将这些元素放置在所需位置。支持包括PDF、MS Office文件和电子邮件文档在内的50种以上格式，有助于自动化和简化您的工作流程。

############################# Steps ############################
steps:
    enable: true
    title: "如何将数据驱动的列表添加到PPTX文档中"
    content: |
      [GroupDocs.Assembly](/assembly/java/)使您能够快速将数据丰富的列表插入到PPTX模板中。自定义和组织内容轻松便捷。
      
      1. 创建一个PPTX模板，并标记列表的占位符位置。
      2. 设置模板的文件路径。
      3. 从支持的格式（如JSON或XML）中获取数据。
      4. 保存添加了列表的最终文档。
   
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
        // 在模板中包含此标签以指示列表应出现的位置
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // 定义模板的文件路径
        String template = "list_template.pptx";

        // 从您选择的来源提取数据
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 将文档保存为嵌入列表的文件
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "通过数据集成从模板生成文档"
  description: "GroupDocs.Assembly for Java简化了向文档模板中添加动态列表、表格、图表和其他组件的过程。"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的关键特性"
  features:
    # feature loop
    - title: "利用多种来源的数据构建报告"
      content: "使用JSON、XML和CSV等格式的数据高效填充列表和其他组件。"

    # feature loop
    - title: "无缝添加列表和其他数据元素"
      content: "GroupDocs.Assembly支持将列表、图表、表格等嵌入文本、图像和链接中，以创建精美的文档。"

    # feature loop
    - title: "精准控制数据出现的位置"
      content: "基于LINQ的模板允许您定义列表和数据的确切位置。使用循环自动创建详细列表，并应用自定义格式。"

    # feature loop
    - title: "支持多种文档格式"
      content: "创建或编辑MS Office、PDF、OpenOffice、HTML和电子邮件等格式的文件。根据需要合并来自多个文档的内容。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何通过编程创建列表"
      content: |
        此示例展示了如何使用GroupDocs.Assembly动态添加列表到PPTX文件中。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 在模板中添加列表的占位符标签
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // 提供模板的文件路径
          String template = "numlist_template.pptx";

          // 提取所需数据以填充列表
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // 准备包含必要详细信息的数据源
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // 初始化DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // 保存包含完整列表的输出文档
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "发现GroupDocs.Assembly的功能"
    exclude: "list"
    description: "使用先进的数据集成工具轻松设计和生成内容丰富的文档。"
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
    title: "在多种格式中生成文档"
    exclude: "PPTX"
    description: "Java支持超过50种格式，使您能够通过结合数据和模板创建结构化文档。"
    items: 
          
        # format loop 1
        - name: "在PDF中创建列表"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中创建列表"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中创建列表"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中创建列表"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---