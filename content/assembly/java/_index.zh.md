---
############################# Static ############################
layout: "landing"
date: 2025-03-17T13:11:11
draft: false

lang: zh
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "Java库用于文档创建、自动化和报告"
head_description: "Java库用于自动化文档创建和生成报告。使用自定义模板创建PDF、Word、Excel、PPTX、HTML和电子邮件文档。"

############################# Header ############################
title: "用于自动化报告和文档的Java API"
description: "通过将数据与模板合并简化Java中的报告生成。"
words:
  for: "用于"

actions:
  main: "通过Maven获取试用版"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "准备开始吗？"
  description: "免费试用GroupDocs.Assembly的功能或请求许可证。"

release:
  title: "版本 {0} 已发布"
  notes: "查看新功能"
  downloads: "下载"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "使用Java在DOCX中生成图表"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // 主模板的路径
    String template = "chart_template.docx";

    // 从源中检索管理者的生产力数据
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // 创建一个包含数据的 DataSourceInfo 实例
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // 使用另一个 DataSourceInfo 设置图表颜色
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // 用数据填充模板并保存到输出
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly 概述"
  description: "一个旨在自动化文档创建和无缝数据集成的Java库。"
  features:
    # feature loop
    - title: "使用Java将业务数据合并到模板"
      content: "轻松创建专业报告，通过使用GroupDocs.Assembly for Java将JSON、XML或其他源的数据嵌入到预设计的模板中。"

    # feature loop
    - title: "处理嵌入对象"
      content: "使用来自外部源的数据自动填充文档中的表格、图表和图示等元素。"

    # feature loop
    - title: "高级自定义"
      content: "GroupDocs.Assembly for Java 提供灵活的功能，如生成条形码、通过URL提取在线数据和以不同格式导出输出。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Assembly for Java 与流行的操作系统、开发框架和包管理器无缝协作。"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Assembly for Java 支持广泛的[文档格式](https://docs.groupdocs.com/assembly/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 格式
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### 图像及其他格式
        * **可移植:** PDF
        * **图像:** SVG, TIFF
        * **其他办公格式:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### 其他格式
        * **网络:** HTML, MHTML
        * **电子邮件:** EML, MSG, EMLX
        * **其他:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Assembly 的关键能力"
  description: "使用先进的数据处理创建专业文档和报告。"

  items:
    # feature loop
    - icon: "preview"
      title: "可视数据元素"
      content: "在文档中直接添加和格式化图表、表格、图像和列表等元素。"

    # feature loop
    - icon: "manipulate"
      title: "数据转换"
      content: "使用公式、排序和其他工具有效地组织和展示数据。"

    # feature loop
    - icon: "two_pages"
      title: "支持多种格式"
      content: "轻松处理常用文件类型，无论是模板还是输出文件。"

    # feature loop
    - icon: "document_settings"
      title: "增强的模板格式设置"
      content: "使用数字、字母和其他高级格式选项自定义模板。"

    # feature loop
    - icon: "text"
      title: "动态条形码生成"
      content: "迅速在需要时创建和插入条形码图像。"

    # feature loop
    - icon: "add"
      title: "灵活的文本样式"
      content: "在模板中应用文本转换，如大写、小写、首字母大写或其他样式。"

    # feature loop
    - icon: "manipulate"
      title: "导入外部内容"
      content: "在生成文档时动态嵌入来自外部文件的内容。"

    # feature loop
    - icon: "convert"
      title: "以多种格式导出"
      content: "使用指定的扩展名或配置保存最终文档。"

    # feature loop
    - icon: "update"
      title: "动态媒体嵌入"
      content: "在文档创建过程中使用Base64编码的数据插入图像或其他内容。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "探索GroupDocs.Assembly常见任务的示例代码。"
  items:
    # code sample loop
    - title: "在Word中创建项目符号列表"
      content: |
        了解如何在Word文档中添加[项目符号列表](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/)，以组织数据表示。 此示例展示如何使用GroupDocs.Assembly在Word中生成列表。
        {{< landing/code title="在Word中创建项目符号列表">}}
        ```java {style=abap}
        // 在文档页面插入此模板：
        // 管理者的绩效指标
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // 指定模板路径
        String template = "Bulleted List Template.docx";

        // 设置输出文件路径
        String result = "Result Report.docx"

        // 从JSON源中检索管理者的数据
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // 生成填充数据的报告
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "在PPTX中创建饼图"
      content: |
        使用模板和XML将[饼图](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/)添加到您的演示文稿中。 通过包含饼图以可视化数据，让您的报告更具吸引力。
        {{< landing/code title="在PPTX中创建饼图">}}
        ```java {style=abap}   
        // 将图表标题模板添加到演示文稿中：
        // 客户的收入 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 还要包括图表数据模板：
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 指定图表模板路径
        String template = "Pie Chart Template.pptx";

        // 设置输出文件路径
        String result = "Result Report.pptx"

        // 从XML源中检索客户的数据
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // 生成图表并保存结果
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---