---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/assembly/net/barcode/svg/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB PS PCL XML OXPS MD EML EMLX MSG 

############################# Head ############################
head_title: "通过 .NET 在文档和电子邮件中创建和添加条码图像"
head_description: "GroupDocs.Assembly .NET API 允许开发人员轻松地在文档（PDF DOC、DOCX、RTF、XLSX、CSV、PPTX）和电子邮件消息中动态生成和插入条形码图像。"

############################# Header ############################
title: "通过 .NET API 在 SVG 文档中生成和插入条形码图像"
description: "GroupDocs.Assembly .NET 完全支持使用 C# 和 VB.NET API 在 SVG 文档中创建、编辑和添加动态条码图像。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在文档中生成条码图像？"
    content: |
      此页面将帮助用户了解和了解如何在 C#、ASP.NET 和其他 .NET 相关应用程序中的文档和电子邮件消息中动态生成和插入条形码图像。 GroupDocs.Assembly .NET 是一个非常强大的 API，它使用户能够在自己的 .NET 应用程序中自动生成许多领先文件格式的报告，而无需任何外部依赖。 它支持一些非常常见的文件格式，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿和幻灯片。 它完全支持一些常见的线性和二维条码符号。 您还可以轻松自定义条码图像大小、前后颜色、条码文本的字体和位置、设置条码图像分辨率等。 它还支持从模板创建自定义文档，并从各种来源（如数据库、XML、JSON、OData、对象等）获取数据。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET 在 SVG 文档中生成条码"
      content_left: |
       GroupDocs.Assembly .NET 完全支持在 SVG 文档中添加和管理条码。 以下 C# .NET 代码示例演示了如何在 BARCODE 文档中生成和插入条形码图像。 

      title_right: "如何在 SVG 中使用条形码图像"
      content_right: |
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 的实例
        * 使用以下参数调用 [AssembleDocument]( https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法
          * 流以读取模板文档。
          * 流以写入结果文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "8576f622912b355ce69966077033dcac"
      gistfile: "generate_barcodes_in_spreadsheets.cs"

    - title_left: "通过 .NET 在 SVG 中设置条码图像分辨率"
      content_left: |
       GroupDocs.Assembly .NET 完全支持在 SVG 文档中添加和管理条码。 您只需几行代码即可轻松设置条形码分辨率。 以下代码允许用户将水平和垂直分辨率设置为 300 DPI。

      title_right: "BARCODE 中增强的条码分辨率"
      content_right: |
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 的实例
        * 调用 BarcodeSettings.Resolution 方法将条码图像的分辨率设置为 300 DPI。

      gisthash: "9d8d743bd67b4bce5a4a7f1250deef26"
      gistfile: "set_barcode_image_resolution.cs"
      

    - title_left: "系统要求"
      content_left: |
        所有主要平台和操作系统都支持 GroupDocs.Assembly .NET API。 如需完整的系统要求指南，请访问 [系统要求](https://docs.groupdocs.com/assembly/net/system-requirements/) 在执行以下代码之前，请确保您已安装以下先决条件 系统：
        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Visual Studio、Xamarin、MonoDevelop 等
        * 框架：.NET Framework、.NET Standard、.NET Core、Mono
        * 从 [NuGet](https://www.nuget.org/packages/GroupDocs.Assembly/) 获取最新版本的 GroupDocs.Assembly .NET API
        
      title_right: "为什么使用 GroupDocs.Assembly"
      content_right: |
       * 允许用户从模板创建自定义文档。
       * 无需其他软件即可创建和自动化文档
       * 能够根据数据源生成输出文档
       * 在报表中动态插入文档内容
       * 动态附加电子邮件附件并在报告中插入超链接
       * 自动删除空段落
       * 全面支持多种数据格式
       * 动态电子邮件附件支持

demos:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---