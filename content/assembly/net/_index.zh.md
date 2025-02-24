---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: zh
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

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
head_title: ".NET文档自动化、组装和报告生成API"
head_description: "C# .NET API用于文档自动化、组装和报告生成。根据自定义模板创建PDF、Word、Excel、PPTX、HTML和电子邮件文档。"

############################# Header ############################
title: ".NET文档自动化和报告API"
description: "通过定义模板和合并数据来在.NET应用程序中生成报告。"
words:
  for: "用于"

actions:
  main: "通过Nuget下载试用版"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "准备开始吗？"
  description: "免费试用GroupDocs.Assembly的功能或请求许可证。"

release:
  title: "版本 {0} 已发布"
  notes: "查看新功能"
  downloads: "下载"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "使用C#填充DOCX中的图表"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // 主模板的路径
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly 概述"
  description: ".NET解决方案用于自动化文档创建及高级数据集成。"
  features:
    # feature loop
    - title: "使用C#将业务数据添加到文档模板"
      content: "报告生成变得容易：使用GroupDocs.Assembly for .NET，您可以轻松将来自JSON或XML等源的数据插入到预定义模板中。"

    # feature loop
    - title: "处理本地数据对象"
      content: "支持的文档类型包括可以用数据自动填充的嵌入对象，如图示、图表、表格和列表。"

    # feature loop
    - title: "其他功能"
      content: "GroupDocs.Assembly for .NET 提供广泛的自定义选项。可以通过编程设计数据对象，生成条形码，通过URL使用在线数据源，以及以多种格式保存输出。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Assembly for .NET 兼容以下操作系统、框架和包管理器。"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Assembly for .NET 可以处理以下[文件格式](https://docs.groupdocs.com/assembly/net/supported-document-formats/)。
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
  title: "GroupDocs.Assembly 功能"
  description: "使用高级数据模型创建文档和报告。"

  items:
    # feature loop
    - icon: "preview"
      title: "高级数据表示"
      content: "支持多种数据对象，如图表、列表、表格、图像等。"

    # feature loop
    - icon: "manipulate"
      title: "数据处理"
      content: "应用公式和顺序操作以有效格式化和显示数据。"

    # feature loop
    - icon: "two_pages"
      title: "广泛支持的格式范围"
      content: "与所有常用文档格式无缝协作，无论是模板还是输出文件。"

    # feature loop
    - icon: "document_settings"
      title: "丰富的模板标记"
      content: "在模板中利用序数、基数和字母数字格式。"

    # feature loop
    - icon: "text"
      title: "嵌入条形码"
      content: "动态生成条形码图像并将其插入到文档中。"

    # feature loop
    - icon: "add"
      title: "数据格式化"
      content: "以大写、小写、大写或首字母大写样式格式化模板中的字符串。"

    # feature loop
    - icon: "manipulate"
      title: "文档内容处理"
      content: "动态将外部文档中的内容插入到您的报告中。"

    # feature loop
    - icon: "convert"
      title: "多种格式保存"
      content: "通过文件扩展名或详细配置指定输出文件格式。"

    # feature loop
    - icon: "update"
      title: "灵活的数据处理"
      content: "使用Base64编码的字节动态插入图像和文档。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "典型GroupDocs.Assembly操作的代码片段。"
  items:
    # code sample loop
    - title: "在Microsoft Word文档中插入项目符号列表"
      content: |
        [项目符号列表](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/)是展示商业数据的常见方式。 以下示例展示如何使用GroupDocs.Assembly将列表添加到Word文档中。
        {{< landing/code title="如何在文档中填充列表">}}
        ```csharp {style=abap}
        // 在文档页面插入此模板：
        // 管理者的绩效指标
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // 指定模板路径
        string template = "Bulleted List Template.docx";

        // 设置输出文件路径
        string result = "Result Report.docx"

        // 从JSON源中检索管理者的数据
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // 生成填充数据的报告
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "在PPTX演示文稿中插入饼图"
      content: |
        您可以使用模板和XML数据创建[饼图](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/)。 通过直观的数据表现增强您的报告。
        {{< landing/code title="如何在饼图中表示数据">}}
        ```csharp {style=abap}
        // 将图表标题模板添加到演示文稿中：
        // 客户的收入 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 还要包括图表数据模板：
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 指定图表模板路径
        string template = "Pie Chart Template.pptx";

        // 设置输出文件路径
        string result = "Result Report.pptx"

        // 从XML源中检索客户的数据
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // 生成图表并保存结果
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---