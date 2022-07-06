---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/assembly/net/document/xlt/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "通过 .NET API 将外部文档的内容插入电子邮件和 XLT 文件"
head_description: "GroupDocs.Assembly .NET API 使程序员能够将外部文档的内容动态插入 PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、EML、MSG 和其他文件格式。"

############################# Header ############################
title: "通过 .NET API 将外部文档的内容插入到 Office 文件和电子邮件中"
description: "GroupDocs.Assembly .NET API 完全支持将外部文档内容动态插入报告、电子邮件和 Office 文档，如 PDF DOCX、XLSX、CSV、PPTX、MSG 等。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何通过 .NET 将外部文档的内容插入到其他文件、报告和电子邮件中？"
    content: |
       文档或文档文件是指用户可以在稍后阶段检索的数字和非数字信息集。计算机或数字文档是由软件应用程序创建的文件，可以存储在计算机系统中。通常使用文字处理器或文本编辑器在计算机系统上创建电子文档。 GroupDocs.Assembly for .NET 是一个非常有用的 API，可帮助软件开发人员创建功能强大的应用程序软件，这些软件可用于轻松创建和管理他们的文档。它允许软件开发人员将外部文档的内容动态插入到报告、电子邮件和 Office 文档中。它支持一些非常常用的文档类型，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿等等。此外，完全支持与文档内容插入和编辑相关的一些高级功能，例如将内容插入文档页面、插入电子表格单元格、编辑或替换内容、将内容插入演示幻灯片等等。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET 将外部文档内容插入 Word 文件"
      content_left: |
       GroupDocs.Assembly .NET API 使软件开发人员能够轻松地将外部文档的内容插入到各种类型的文档和电子邮件中。 下面的 .NET 代码示例展示了如何将外部文档的内容插入到 Word 处理文档中，只需几行代码。

      title_right: "如何将文档的内容添加到 XLT 文件"
      content_right: |
        * 设置源打开文档模板
        * 设置目的地打开文档报告
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) 方法生成开放文档格式的报告。 它支持
          * 从指定的源路径加载模板文档
          * 使用来自指定的单个或多个源的数据填充模板文档
          * 使用给定的 LoadSaveOptions 将结果文档存储到目标路径。
          * 有关数据源对象的信息。

      gisthash: "c4dc0be4f8ab8c2ba4ee6a78673ca1cd"
      gistfile: "dynamic_documents_insertion_to_word_processing.cs"

    - title_left: "通过 .NET 将外部文档的内容插入电子邮件"
      content_left: |
       GroupDocs.Assembly .NET API 允许在文档中添加和管理各种文档类型和内容。 它允许将外部文档的内容动态插入到各种文档类型和电子邮件文件格式中。 以下 C# 代码显示了用户如何轻松地将外部文档的内容插入到他们自己的 .NET 应用程序中的文档和电子邮件中。 

      title_right: "通过 C# 将文档的内容添加到电子邮件中"
      content_right: |
        * 设置源打开文档模板
        * 设置目的地打开文档报告
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) 方法生成开放文档格式的报告。 它支持
          * 从指定的源路径加载模板文档
          * 使用来自指定的单个或多个源的数据填充模板文档
          * 使用给定的 LoadSaveOptions 将结果文档存储到目标路径。
          * 有关数据源对象的信息。 

      gisthash: "8fe014550c5f05467da6910a7ee16f18"
      gistfile: "dynamic_documents_insertion_to_emails_dotnet.cs"

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