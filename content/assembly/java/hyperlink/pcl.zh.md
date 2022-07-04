---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/assembly/java/hyperlink/pcl/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "通过 Java API 将超链接添加到 Office PCL 文档和报告"
head_description: "GroupDocs.Assembl for Java 支持在 Java 应用程序中动态插入指向办公室和电子邮件文档的超链接，例如 PDF DOCX、RTF、XLSX、PPTX、EML、MSG 等。"

############################# Header ############################
title: "通过 Java API 为 Office 文档和电子邮件添加超链接"
description: "GroupDocs.Assembly Java API 允许软件专业人员以编程方式将超链接添加到电子邮件和 Office 文档，如 PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、MSG 等。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何使用 Java API 将超链接添加到 Office 和电子邮件文档？"
    content: |
       超链接是一个单词、短语或图像，您可以单击它来跳转到新文档或当前文档中的新部分。 超链接是万维网的主干，用于万维网上的许多必要功能。 GroupDocs.Assembly for Java 是一个文档自动化和报告生成 API，可帮助软件开发人员在其文档中动态插入超链接或轻松地报告。 该 API 非常稳定，完全支持与超链接管理相关的多项高级功能，例如向文档页面添加超链接、向演示幻灯片添加链接、向电子表格单元格添加超链接、修改超链接内容、从书签中动态插入链接、删除不需要的链接 链接，显示文本而不是超链接，等等。 完全支持一些非常常见的文档类型，如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿等。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 插入到文字处理文档的超链接"
      content_left: |
       GroupDocs.Assembly Java API 完全支持在各种常用文档格式中插入和编辑超链接。 下面的 Java 代码示例显示了如何在 Microsoft Word 文档中插入超链接。

      title_right: "通过 Java 在 PCL 文档中插入超链接"
      content_right: |
        * 设置源文档和目标文档
        * 设置 Uri 表达式以及显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 方法来组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "通过 Java 在电子表格中添加超链接"
      content_left: |
       GroupDocs.Assembly Java API 允许计算机程序员在其电子表格文档中轻松插入和修改超链接。 他们可以轻松访问、编辑其位置或将其替换为新位置。 以下 Java 代码演示了程序员如何轻松地在其电子表格中添加超链接。

      title_right: "如何插入超链接到 PCL 文件"
      content_right: |
        * 设置源和目标电子表格文件
        * 设置 Uri 表达式以及显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 方法来组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "通过 Java 将超链接插入到 PowerPoint 演示文稿"
      content_left: |
       GroupDocs.Assembly Java API 使程序员可以轻松处理与文档管理相关的任务。 这是一个 Java 代码示例，它展示了软件程序员如何轻松地访问他们的 PowerPoint 演示文稿文档并在其中添加超链接。

      title_right: "如何在演示文稿中插入超链接"
      content_right: |
        * 设置源和目标演示文件
        * 设置 Uri 并显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 方法来组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "使用 Java API 在电子邮件中添加超链接"
      content_left: |
       GroupDocs.Assembly for Java 使软件开发人员只需几行 Java 代码就可以轻松地将超链接添加到他们的电子邮件中。 以下示例演示了开发人员如何轻松地在其电子邮件文档中插入超链接并发送给他们自己的 Java 应用程序中的其他用户。

      title_right: "如何向电子邮件添加超链接"
      content_right: |
        * 设置源和目标电子表格文件
        * 设置 Uri 并显示文本表达式
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 方法来组装文档。 它支持
          * 流式读取模板文档。
          * Stream 写入生成的文档。
          * 文件加载和保存的附加选项。
          * 有关数据源对象的信息。

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

    - title_left: "系统要求"
      content_left: |
       所有主要平台和操作系统都支持 GroupDocs.Assembly Java API。 它可以生成 Microsoft Word、Excel、PowerPoint、Outlook、OpenOffice 和 50 多种其他格式的文档。 如需完整的系统要求指南，请访问 [系统要求](https://docs.groupdocs.com/assembly/java/system-requirements/) 在执行以下代码之前，请确保您已安装以下先决条件 系统：
         * 操作系统：Microsoft Windows、Linux、MacOS
         * Java 版本支持：J2SE 7.0 (1.7)、J2SE 8.0 (1.8) 或以上
         * 从 [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/) 获取最新版本的 GroupDocs.Assembly Java API
        
      title_right: "为什么使用"
      content_right: |
        * 从模板创建自定义文档。
        * 动态附加电子邮件附件。
        * 创建和自动化文档不需要额外的软件。
        * 根据数据源生成输出文档。
        * 在报表中动态插入文档内容
        * 在电子表格组装期间应用公式。
        * 支持多种数据格式
        * 顺序数据操作支持。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---