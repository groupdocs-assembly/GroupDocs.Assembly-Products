---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/assembly/net/text/xlt/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: ".NET API 在 XLT 文档中动态插入超链接"
head_description: "GroupDocs.Assembly .NET API 允许开发人员动态地将超链接插入到电子邮件、报告或文档，如 PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、EML、MSG 等。"

############################# Header ############################
title: "通过 .NET API 动态插入指向 XLT 文档和报告的超链接"
description: "GroupDocs.Assembly .NET API 使程序员能够动态插入超链接到报告、电子邮件和 Office 文档，如 PDF DOC、DOCX、RTF、XLSX、CSV、PPT、PPTX、EML、HTML、MSG 等。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在报表、电子邮件和各种文档中动态插入超链接？"
    content: |
       该网页将解释用户如何在他们自己的 .NET 应用程序中动态插入指向他们的报告、电子邮件消息和各种文档类型的超链接。 超链接是万维网的支柱，可用于链接不同的页面、文档或单击以跳转到当前文档中的新部分。 GroupDocs.Assembly .NET 是一个非常强大的 API，它可以帮助软件开发人员通过几行代码在他们的文档或报告中动态添加超链接。 它包括对一些非常流行的文档类型的支持，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿等等。 它支持一些高级功能，例如插入文档页面的链接、插入单元格的链接、编辑超链接、显示文本而不是超链接、动态插入书签中的链接、插入演示幻灯片的超链接等等。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET 将超链接插入到文字处理文档"
      content_left: |
       GroupDocs.Assembly .NET API 为在各种类型的文档中插入和编辑超链接提供了完整的支持。 以下 C# .NET 代码示例展示了如何在 Word 文档中轻松添加超链接。 

      title_right: "如何在 Word 文件中添加超链接"
      content_right: |
        * 设置源文档和目标文档
        * 设置 Uri 表达式以及显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "f4a8031406d44941d400088b718f7730"
      gistfile: "insert_hyperlinks_to_word_document.cs"

    - title_left: "通过 .NET 在电子表格中动态插入超链接"
      content_left: |
       GroupDocs.Assembly .NET API 完全支持在电子表格文件中添加和处理超链接。 您可以轻松地编辑它的位置或将其替换为新位置。 下面的 C# 代码显示了用户在他们自己的 .NET 应用程序中的电子表格文件中插入超链接是多么容易。

      title_right: "将超链接添加到电子表格文档"
      content_right: |
        * 设置源和目标电子表格文件
        * 设置 Uri 表达式以及显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "c2f9cd8bb06f9a7a2c444621ebf82696"
      gistfile: "insert_hyperlinks_in_spreadsheet_documents.cs"

    - title_left: "通过 .NET API 将超链接添加到 PowerPoint 演示文稿"
      content_left: |
       GroupDocs.Assembly for .NET 帮助软件专业人员构建用于管理各种类型文档的应用程序。 下面的代码示例演示了软件开发人员如何在其 PowerPoint 演示文稿文档中添加超链接。

      title_right: "如何在演示文稿中添加超链接"
      content_right: |
        * 设置源和目标演示文件
        * 设置 Uri 并显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "49e1ca9eccc41942372c23c14f98ecef"
      gistfile: "insert_hyperlinks_in_presentation_documents.cs"

    - title_left: ".NET API 在电子邮件中插入超链接"
      content_left: |
       GroupDocs.Assembly .NET API 允许软件专业人员在他们的电子邮件文档中插入超链接。 下面的 .NET 代码演示了程序员如何轻松地将超链接添加到他们的电子邮件消息并从他们自己的 .NET 应用程序中发送给其他用户。

      title_right: "向电子邮件文档添加超链接"
      content_right: |
        * 设置源和目标电子表格文件
        * 设置 Uri 并显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。 

      gisthash: "8c119b4faa0334179854e164d87d3e7b"
      gistfile: "insert_hyperlinks_in_email_documents.cs"  

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
        * 完全支持多种数据格式
        * 动态电子邮件附件支持

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---