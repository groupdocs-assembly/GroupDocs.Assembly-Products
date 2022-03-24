---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API 用于文档自动化、组装和报告生成"
head_description: "C# .NET 文档自动化、程序集和报告生成 API。从自定义模板创建 PDF Word Excel PPTX HTML 和电子邮件文档."

############################# Header ############################
title: ".NET 文档自动化和报告 API"
description: "通过定义模板和合并数据在 .NET 应用程序中生成报告."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "/border/groupdocs-assembly-net.svg"
        product: "GroupDocs.Assembly"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概述"

            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/assembly"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for .NET API 可帮助您构建强大的文档自动化和报告生成应用程序，并能够从 C#、ASP.NET 和其他 .NET 相关应用程序中的自定义模板生成报告。只需几行代码，.NET 报告库就可以智能地从定义的文档模板中组装给定的数据，并通过从各种数据源（数据库、XML、JSON、ODATA、CSV、自定义 .NET 对象）。

      它支持基于 LINQ 的模板语法，用户可以轻松生成所有常用业务文件格式的输出文档，例如 PDF、HTML、Outlook 电子邮件、微软办公软件 Word、Excel 工作表、PowerPoint 演示文稿和幻灯片。模板元素的格式属性也可以通过操作文本、HTML 和条件块、图像、图表、条形码、超链接、数据透视表等来配置。

      GroupDocs.Assembly for .NET 可用于在任何面向 .NET 平台的开发环境中开发应用程序。它与所有基于 .NET 的语言兼容，并支持可以安装 Mono 或 .NET 框架（包括 .NET Core）的流行操作系统（Windows、Linux、MacOS）。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 .NET 的 GroupDocs.Assembly 的概述：
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "概述"
          content: |
            * 数据制定
            * 数据格式化
            * 数据自动化
            * 创建模板
            * 模板元素格式
            * 报告生成
      
      ## TAB TWO ##
      tab_two:
        description: |
          下面列出了 .NET 文档生成 API 支持的 [文档文件格式](https://docs.groupdocs.com/assembly/net/supported-document-formats/)。

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公格式"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            # table loop
            - title: "支持的数据源"
              content: |
                * 数据库
                * XML
                * OData
                * JSON
                * CSV
                * 自定义 .NET 对象
                * 电子表格作为数据表
                * 文字处理表作为数据表

        right:
          enable: true
          table:
            # table loop
            - title: "其他格式"
              content: |
                * **OpenOffice Document Formats**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **Markdown 文档 File**: MD
                * **Other**: TXT

            # table loop
            - title: "格式间汇编支持"
              content: |
                * Word Processing **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Spreadsheet **TO** Spreadsheet, HTML, PDF, XPS, TIFF, MHTML
                * Presentation **TO** Presentation, HTML, PDF, XPS, TIFF
                * Email **TO** Word Processing, Email, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML & TXT **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Assembly for .NET 支持以下作品，Frameworks & 包管理器:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * .NET Framework 2.0 或更高版本
                * Mono 框架 1.2 或更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "包管理器"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "开发环境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Assembly 用于 .NET 功能"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "适用于多种数据格式"

      # feature loop
      - icon: "fas fa-eye"
        content: "能够使用公式和顺序数据操作来操作数据"

      # feature loop
      - icon: "fas fa-bolt"
        content: "将模板语法中的字符串格式化为 Upper、Lower、Capital、FirstCap"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "在模板语法中执行序数、基数、字母数字格式"

      # feature loop
      - icon: "fas fa-code"
        content: "在模板文档中定义变量并支持模板语法标签中的文本注释"

      # feature loop
      - icon: "fas fa-cloud"
        content: "将外部文档的内容动态插入到您的报告中"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "在报告中动态生成条码图像并为 HTML 文档设置背景颜色"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "为电子邮件消息正文动态分配属性并在报告中插入超链接"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "动态构建电子邮件附件"

      # feature loop
      - icon: "fas fa-border-all"
        content: "支持 Microsoft Word NEXT 字段的类比"

      # feature loop
      - icon: "fas fa-wrench"
        content: "组装文字处理文档时更新字段"

      # feature loop
      - icon: "fas fa-columns"
        content: "组装电子表格文档时计算公式"

      # feature loop
      - icon: "fas fa-file-word"
        content: "格式化模板的数字、文本、图像、图表、日期时间元素"

      # feature loop
      - icon: "fas fa-envelope"
        content: "加载和保存组装的 POT 和 OTP 演示文档格式"

      # feature loop
      - icon: "fas fa-print"
        content: "对模板使用基于 LINQ 的语法并执行模板元素的条件文本格式设置"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "使用文件扩展名或显式规范更改组装文档的文件格式"

      # feature loop
      - icon: "fas fa-lock"
        content: "Markdown 支持有序列表 - 将新组装的电子邮件和 Word 文档保存到 Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "支持多种类型的报告，例如图表、列表、表格、图像等"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "生成的文档中的内联模板语法错误，而不是抛出异常"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "使用资源从 HTML 加载模板文档，并使用资源将组装的 Word、Excel、PowerPoint 和电子邮件保存到 HTML"

      # feature loop
      - icon: "fas fa-heading"
        content: "在 Word 文档格式和带有 HTML 和 RTF 正文的电子邮件中动态添加重启列表编号"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Base64 编码 字节 动态插件 图像和文档 调整Word文档复选框值设置"

      # feature loop
      - icon: "fas fa-cube"
        content: "在保持图像比例的同时，在 Word、Excel、演示文稿和电子邮件的文本框中拉伸图像"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "为文档格式动态添加链接和书签并命名 Excel 电子表格的单元格范围"

    more_feature:
      # more_feature_loop
      - title: "支持模板元素"
        content: |
          GroupDocs.Assembly for .NET API 让您可以控制使用大量模板元素。您可以使用格式化的文本块、HTML 块、图像、图表、超链接和条形码（通过条形码字体）。还支持重复块和条件块，包括列表项和表格行。您还可以根据电子表格、演示文稿、文档和电子邮件的模板表达式动态合并包含相同文本的表格单元格，并带有 HTML 和 RTF 正文。

      # more_feature_loop
      - title: "使用列表报告"
        content: |
          使用 GroupDocs.Assembly for .NET API，您可以使用以下三种类型的列表报告：

          * 项目符号列表
          * 编号列表
          * Colored 编号列表

      # more_feature_loop
      - title: "使用图表报告"
        content: |
          GroupDocs.Assembly for .NET 支持以下类型的图表报告：

          * 气泡图，显示数据的三个维度
          * 柱形图
          * 饼形图
          * 散点图
          * 系列图表（彩色）

      # more_feature_loop
      - title: "使用表格报告"
        content: |
          GroupDocs.Assembly for .NET 支持以下类型的表格报告：

          * 主从表
          * 带有突出显示的行的表
          * 具有替代内容的表格
          * 具有过滤、分组和排序的表
          
          您还可以在表格行中使用数据带。

      # more_feature_loop
      - title: "易于集成"
        content: |
          只需几行代码，您就可以轻松地将 GroupDocs.Assembly for .NET API 与您的 .NET 应用程序集成。以下是在打开文档中生成报告的示例代码 format:

          ```cs
          // 即时 DocumentAssembler 类
          DocumentAssembler assembler = new DocumentAssembler();
          // 调用 AssembleDocument 生成报告
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
          // 请参阅 https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET 上的 DataLayer.GetCustomerData () 方法详细信息
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Assembly 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Assembly for Java"
          image: "/border/groupdocs-assembly-java.svg"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
