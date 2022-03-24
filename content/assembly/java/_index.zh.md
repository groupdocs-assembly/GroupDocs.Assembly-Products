---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 文档自动化组装和动态报告生成器 API"
head_description: "用于文档自动化、组装和报告的 Java API。从自定义模板创建报告。从 DB、JSON、OData 和 XML 数据源组装 PDF Word Excel PPTX HTML."

############################# Header ############################
title: "用于自动化文档和报告的 Java API"
description: "构建文档自动化应用程序以获取数据；将其放入可定制的模板并通过 Java API 生成动态报告."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "/border/groupdocs-assembly-java.svg"
        product: "GroupDocs.Assembly"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java API 可帮助您在 Java 中快速开发文档自动化和报告应用程序，以从模板生成自定义报告，而无需安装任何外部软件。报告生成引擎从模板文档中获取数据，将其组装并根据定义的语法以指定的输出格式生成报告。它允许您动态配置和插入模板元素的格式属性，并支持各种数据源（JSON、XML、OData、数据库、CSV、电子表格作为数据表、字处理表作为数据表和数据库）从中检索数据。

      文档组装库可识别多种文档格式，并允许您以所有支持的文件类型创建模板，例如 PDF、HTML、Outlook 电子邮件、微软办公软件 Word、Excel 工作表、PowerPoint 演示文稿和文本。它支持基于 LINQ 的模板语法，用户还可以动态配置和插入模板元素的格式属性。

      GroupDocs.Assembly for Java 很容易与新的或现有的 Java 应用程序集成。它与所有 Java 版本高度兼容，并支持能够运行 Java 运行时的流行操作系统（Windows、Linux、MacOS）。
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 Java 的 GroupDocs.Assembly 的概述：

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
          下面列出了 Java 文档生成 API 支持的 [文档文件格式](https://docs.groupdocs.com/assembly/java/supported-document-formats/)。

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
          GroupDocs.Assembly for Java 支持以下框架、框架和管理:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * Java 7 (1.7) 及更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "开发环境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "构建自动化工具"
              content: |
                * Maven

############################# 特征 ############################
features:
    enable: true
    title: "用于 Java 功能的 GroupDocs.Assembly"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "在保持图像比例的同时调整 Word、Excel、演示文稿和电子邮件文本框中的图像"

      # feature loop
      - icon: "fas fa-eye"
        content: "使用公式并执行顺序数据操作 - 在电子表格组装期间应用公式"

      # feature loop
      - icon: "fas fa-bolt"
        content: "对模板语法中的字符串应用大写、小写、大写、FirstCap 格式"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "模板语法支持序数、基数、字母数字性质的格式"

      # feature loop
      - icon: "fas fa-code"
        content: "在模板语法标签中支持带有自定义变量和文本注释的模板文档"

      # feature loop
      - icon: "fas fa-cloud"
        content: "在报表中动态插入文档内容"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "动态配置 HTML 文档的背景颜色并在报告中生成条码"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "在报告中动态插入超链接并将属性应用于电子邮件正文"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "在文字处理文档组装期间动态附加电子邮件附件和更新字段"

      # feature loop
      - icon: "fas fa-border-all"
        content: "支持 Microsoft Word 的 NEXT Field Analogue"

      # feature loop
      - icon: "fas fa-wrench"
        content: "为文档格式动态添加链接和书签并命名 Excel 电子表格的单元格范围"

      # feature loop
      - icon: "fas fa-columns"
        content: "加载和保存组装的 POT 和 OTP 演示文档格式"

      # feature loop
      - icon: "fas fa-file-word"
        content: "数字、文本、图像、日期时间、图表元素的模板格式"

      # feature loop
      - icon: "fas fa-envelope"
        content: "从 Base64 编码字节动态插入图像和文档"

      # feature loop
      - icon: "fas fa-print"
        content: "基于 LINQ 的模板语法"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "使用显式规范或文件扩展名更改组合文件的格式"

      # feature loop
      - icon: "fas fa-lock"
        content: "Markdown 支持有序列表 - 将新组装的电子邮件和 Word 文档保存到 Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "生成各种报告类型，例如图表、图像、表格、列表等"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "生成的文档中的内联模板语法错误，而不是抛出异常"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "动态重新启动 Word 文档中的编号列表以及带有 HTML 和 RTF 正文的电子邮件"

      # feature loop
      - icon: "fas fa-heading"
        content: "支持组合 Markdown 文档的表格、自动链接、内联链接和图像"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "生成条码 （GS1-128 AI 8102 Coupon Extended 和 UPCA & GS1 Databar Coupon)"

      # feature loop
      - icon: "fas fa-cube"
        content: "使用资源从 HTML 加载模板文档，并使用资源将组装的 Word、Excel、PowerPoint 和电子邮件保存到 HTML"

    more_feature:
      # more_feature_loop
      - title: "操作模板元素"
        content: |
          使用 GroupDocs.Assembly for Java API 操作大量模板元素。您可以使用的模板元素包括文本块、图像、超链接、HTML 块、条形码（通过条形码字体）和图表。您还可以为列表项和表格行应用重复块和条件块。基于具有 HTML 和 RTF 正文的文档、演示文稿、电子表格和电子邮件的模板表达式，动态合并包含相同文本的表格单元格。
      
      # more_feature_loop
      - title: "处理列表报告"
        content: |
          使用 GroupDocs.Assembly for Java API，支持以下类型的列表报告：

          * 项目符号列表
          * 编号列表
          * Colored 编号列表

      # more_feature_loop
      - title: "处理图表报告"
        content: |
          GroupDocs.Assembly for Java 支持以下类型的图表报告：

          * 气泡图，显示数据的三个维度
          * 柱形图
          * 饼形图
          * 散点图
          * 系列图表（彩色）

      # more_feature_loop
      - title: "处理表格报告"
        content: |
          GroupDocs.Assembly for Java 支持以下类型的表格报告：

          * 主从表
          * 带有突出显示的行的表
          * 具有替代内容的表格
          * 具有过滤、分组和排序的表

          您还可以在表格行中使用数据带。

      # more_feature_loop
      - title: "处理图表报告"
        content: |
          将 Java API 的 GroupDocs.Assembly 与您的 Java 应用程序集成是一件轻而易举的事。以下是使用 Java 生成 OpenDocument 格式报告的示例代码块： 

          ```java
          // 即时 DocumentAssembler 类
          DocumentAssembler assembler = new DocumentAssembler();
          // 调用 AssembleDocument 生成报告
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          // 请参阅 https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java 上的新 DataStorage () 方法详细信息
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
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "/border/groupdocs-assembly-net.svg"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---