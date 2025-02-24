---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: zh
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js 工具包用于构建、自动化和定制文档"
head_description: "Node.js 库用于自动化文档工作流程。从模板生成 PDF、Word、Excel、PowerPoint、HTML 和电子邮件文件。"

############################# Header ############################
title: "Node.js API 简化文档和报告自动化"
description: "通过将您的数据与预构建模板合并，简化 JavaScript 报告生成。"
words:
  for: "用于"

actions:
  main: "在 NPM 开始您的试用"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "准备开始吗？"
  description: "免费试用GroupDocs.Assembly的功能或请求许可证。"

release:
  title: "版本 {0} 已发布"
  notes: "查看新功能"
  downloads: "下载"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "使用 Node.js 在 Word 文档中创建图表"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // 主模板的路径
    const template = "chart_template.docx";

    // 从源中检索管理者的生产力数据
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // 创建一个包含数据的 DataSourceInfo 实例
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // 使用另一个 DataSourceInfo 设置图表颜色
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // 用数据填充模板并保存到输出
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly 概述"
  description: "一个专为使用数据处理集成编程创建文档的 Node.js 库。"
  features:
    # feature loop
    - title: "使用 JavaScript 将业务数据集成到模板中"
      content: "通过将 JSON、XML 或其他数据嵌入模板中，生成精美的报告。"

    # feature loop
    - title: "管理嵌入内容"
      content: "使用外部数据自动填充文档中的表格、图表和其他可视元素。"

    # feature loop
    - title: "可定制的选项"
      content: "GroupDocs.Assembly for Node.js via Java 允许您添加条形码、从 URL 获取数据，并以多种格式导出文件。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Assembly for Node.js via Java 与领先的操作系统、框架和包管理器无缝集成。"
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
    GroupDocs.Assembly for Node.js via Java 支持多种 [文档格式](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/)。
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
  title: "GroupDocs.Assembly 的核心功能"
  description: "通过强大的数据管理工具创建动态文档和报告。"

  items:
    # feature loop
    - icon: "preview"
      title: "丰富的数据可视化"
      content: "将图表、表格、图像和列表轻松插入文档中，完全自定义。"

    # feature loop
    - icon: "manipulate"
      title: "转换您的数据"
      content: "利用公式和排序等工具有效地结构化和展示信息。"

    # feature loop
    - icon: "two_pages"
      title: "广泛的格式兼容性"
      content: "与流行文件格式无缝协作，用于模板和输出。"

    # feature loop
    - icon: "document_settings"
      title: "高级模板定制"
      content: "使用数字、字母及其他样式选项格式化模板。"

    # feature loop
    - icon: "text"
      title: "动态生成条形码"
      content: "按需创建并嵌入条形码图像到文档中。"

    # feature loop
    - icon: "add"
      title: "灵活的文本样式"
      content: "轻松在模板中应用文本样式，如大写或标题样式。"

    # feature loop
    - icon: "manipulate"
      title: "动态内容插入"
      content: "在文档生成过程中，动态包括外部文件中的内容。"

    # feature loop
    - icon: "convert"
      title: "导出到多种格式"
      content: "根据您的指定配置将文档保存为多种格式。"

    # feature loop
    - icon: "update"
      title: "动态嵌入媒体"
      content: "在创建文档时，使用 Base64 数据插入图像或其他元素。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "发现如何使用 GroupDocs.Assembly 进行常见任务的实用示例。"
  items:
    # code sample loop
    - title: "在 Word 文档中添加项目符号列表"
      content: |
        了解如何在 Word 文档中创建 [项目符号列表](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/)，有效组织数据。 此示例演示如何使用 GroupDocs.Assembly 生成项目符号列表。
        {{< landing/code title="在 Word 文档中添加项目符号列表">}}
        ```javascript {style=abap}
        // 在文档页面插入此模板：
        // 管理者的绩效指标
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 指定模板路径
        const template = "Bulleted List Template.docx";

        // 设置输出文件路径
        const result = "Result Report.docx"

        // 从JSON源中检索管理者的数据
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // 生成填充数据的报告
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "在 PowerPoint 中插入饼图"
      content: |
        了解如何使用模板和 XML 在演示文稿中添加 [饼图](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/)。 通过饼图增强您的报告，以清晰直观地呈现数据。
        {{< landing/code title="在 PowerPoint 中插入饼图">}}
        ```javascript {style=abap} 
        // 将图表标题模板添加到演示文稿中：
        // 客户的收入 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 还要包括图表数据模板：
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 指定图表模板路径
        const template = "Pie Chart Template.pptx";

        // 设置输出文件路径
        const result = "Result Report.pptx"

        // 从XML源中检索客户的数据
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // 生成图表并保存结果
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---