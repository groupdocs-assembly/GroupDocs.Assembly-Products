



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: zh
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用Java将一个文档插入另一个PPTX中"
head_description: "使用Java轻松组合PPTX文件。GroupDocs.Assembly简化了仅需几行代码即可合并文档的过程。"

############################# Header ############################
title: "轻松将内容嵌入PPTX文件" 
description: "使用GroupDocs.Assembly for Java无缝地将一个PPTX文档插入到另一个文档中。借助灵活和可靠的工具获得准确的结果。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java是什么？"
    link: "/assembly/java/"
    link_title: "了解更多"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)是一个处理文档的多功能解决方案。它使您能够轻松将一个文档集成到另一个文档中，支持超过50种格式，如PDF和MS Office文件。通过合并、编辑和组织内容来量身定制输出，完全符合您的需求。

############################# Steps ############################
steps:
    enable: true
    title: "将文档插入PPTX文件的步骤"
    content: |
      [GroupDocs.Assembly](/assembly/java/)使将一个PPTX文档嵌入到另一个文档中变得简单且可定制。
      
      1. 准备一个具有嵌入内容占位符的PPTX模板。
      2. 指定模板的文件路径。
      3. 提供要嵌入的文档的文件路径。
      4. 保存带有合并内容的输出文件。
   
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
        // 在模板中使用此标签标记嵌入文档的位置
        // <<doc [doc_expression]>>

        // 设置主模板的文件路径
        String template = "doc_template.pptx";

        // 提供要插入的文档的路径
        DataSourceInfo data 
            = new DataSourceInfo("insert.pptx", "doc_expression");

        // 保存带有嵌入内容的最终文件
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "简化文档集成的高级工具"
  description: "使用GroupDocs.Assembly for Java，无论文件类型如何，嵌入文档都简单且可定制。在您的项目中实现干净且一致的结果。"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assembly的亮点"
  features:
    # feature loop
    - title: "使用业务数据创建报告"
      content: "快速可靠地填写来自JSON、XML或CSV等来源的数据，优化您的工作流程。"

    # feature loop
    - title: "用视觉内容增强文档"
      content: "GroupDocs.Assembly允许您将表格、图表和列表与文本、超链接、图像甚至动态条形码一并插入。"

    # feature loop
    - title: "将数据准确定位"
      content: "LINQ模板帮助您精确定位数据，处理数组等重复元素，并轻松应用自定义样式。"

    # feature loop
    - title: "兼容多种文件格式"
      content: "跨各种格式合并文档，包括PDF、HTML、MS Office文件和OpenOffice，为您的项目确保灵活性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何以编程方式将图像插入文档中"
      content: |
        此示例展示了如何使用GroupDocs.Assembly将图像嵌入到PPTX文件中。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 在模板文件中添加占位符标签
          // <<image [expression]>>

          // 定义模板的路径
          String template = "template.pptx";

          // 指定图像的路径
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // 初始化DocumentAssembler实例
          DocumentAssembler asm = new DocumentAssembler();

          // 保存带有嵌入图像的文件
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "关键功能一览"
    exclude: "document"
    description: "了解GroupDocs.Assembly提供的广泛功能，使文档的嵌入与合并高效且无烦恼。"
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
    title: "在不同文档类型之间合并"
    exclude: "PPTX"
    description: "借助Java，您可以在50多种文件格式之间嵌入和组合内容。无缝添加文件以创建专业结果。"
    items: 
          
        # format loop 1
        - name: "在PDF中嵌入文档"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中嵌入文档"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中嵌入文档"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中嵌入文档"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---