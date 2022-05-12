---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/assembly/net/barcode/ott/"
otherformats: DOC DOCX DOCM DOT DOTX DOTM RTF ODT 

############################# Head ############################
head_title: "通过 C#、ASP.NET 在文字处理文档中生成和编辑条码"
head_description: "GroupDocs.Assembly .NET API 允许开发人员在 Word（DOC、DOCX、DOCM、DOT、DOTX、RTF 和 ODT）文档中生成、插入和修改条形码图像。"

############################# Header ############################
title: "通过 .NET 在 Word OTT 文档中创建和使用条形码图像"
description: "使用 GroupDocs.Assembly .NET API 程序员可以在 C#、ASP.NET 和其他 .NET 应用程序内的 Word OTT 文档中动态创建和管理条码图像。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在文字处理文档中生成和插入条形码？"
    content: |
     此页面将帮助用户了解和了解如何在 C#、ASP.NET 和其他 .NET 相关应用程序中的文档和电子邮件消息中动态生成和插入条形码图像。 GroupDocs.Assembly .NET 是一个非常强大的 API，它使用户能够在自己的 .NET 应用程序中自动生成许多领先文件格式的报告，而无需任何外部依赖。 它支持一些非常常见的文件格式，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿和幻灯片。 它完全支持一些常见的线性和二维条码符号。 用户还可以轻松自定义条码图像大小、前后颜色、条码文本的字体和位置、设置条码图像分辨率等。 它还支持从模板创建自定义文档，并从各种来源（如数据库、XML、JSON、OData、对象等）获取数据。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "如何在 OTT 文档中创建条形码"
      content_left: |
       以下 .NET 代码示例显示了用户只需几行代码即可轻松地在自己的 Microsoft Word OTT 文档中动态生成和添加条形码图像。  

      title_right: "通过 .NET 在 OTT 文件中使用条形码图像"
      content_right: |
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 的实例
        * 使用以下参数调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 方法
          * 流以读取模板文档。
          * 流以写入结果文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

     
      gisthash: "50bb52b8877a109c9478bcd092a7ff4f"
      gistfile: "generate_barcodes_in_word_documents.cs"

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