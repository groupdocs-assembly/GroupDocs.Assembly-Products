---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/assembly/net/barcode/xlsx"
otherformats: XLS XLT XLSM XLTX XLTM XLSB ODS 

############################# Head ############################
head_title: "如何通过 C#、ASP.NET 在 Excel 电子表格中生成和添加条码"
head_description: "GroupDocs.Assembly .NET API 支持在 Excel 电子表格（XLS、XLT、XLSX、XLSM、XLTX、XLTM 和 XLSB）文档中创建和插入条形码图像。"

############################# Header ############################
title: "通过 .NET API 在 XLSX  电子表格中创建和管理条码"
description: "使用 GroupDocs.Assembly .NET API 软件开发人员可以在 C#、ASP.NET 应用程序内的 Excel XLSX  电子表格文档中动态创建和管理条码图像。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何为电子表格添加条码生成？"
    content: |
      此页面提供有关如何使用 .NET API 在 Excel 电子表格中生成条形码的信息。 条形码是存储机器可读信息的数字代码，通常用于快速识别大量物品。 它为您的系统带来速度和准确性，从而自动减少操作时间。 GroupDocs.Assembly 是一个功能强大的 .NET API，它允许软件开发人员以编程方式在特定位置的 Microsoft Excel 电子表格中使用自定义文本、外观和不同编码类型绘制大量 1D 和 2D 条形码图像。 该 API 还可以轻松管理条码图像大小、前景色和背景色、字体大小、图像分辨率、文本自动更正等。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET 在 XLSX  电子表格中生成条码"
      content_left: |
       GroupDocs.Assembly .NET 完全支持在 XLSX  电子表格中添加和管理条码。 以下 C# .NET 代码示例演示了如何在 Microsoft Excel 电子表格文档中生成和插入条形码图像。 

      title_right: "如何在 XLSX 中使用条形码图像"
      content_right: |
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 的实例
        * 使用以下参数调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法
          * 流以读取模板文档。
          * 流以写入结果文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "8576f622912b355ce69966077033dcac"
      gistfile: "generate_barcodes_in_spreadsheets.cs"

    - title_left: "系统要求"
      content_left: |
        所有主要平台和操作系统都支持 GroupDocs.Assembly .NET API。 如需完整的系统要求指南，请访问 [系统要求](https://docs.groupdocs.com/assembly/net/system-requirements/) 在执行以下代码之前，请确保您已安装以下先决条件 系统：
        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Visual Studio、Xamarin、MonoDevelop 等。
        * 框架：.NET Framework、.NET Standard、.NET Core、Mono
        * 从 [NuGet](https://www.nuget.org/packages/GroupDocs.Assembly/) 获取最新版本的 GroupDocs.Assembly .NET API
        
      title_right: "为什么使用 GroupDocs.Assembly"
      content_right: |
        * 允许用户从模板创建自定义文档。
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