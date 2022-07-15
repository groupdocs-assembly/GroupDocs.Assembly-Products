---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/assembly/java/document/ps"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Java API：将外部文档的内容添加到 PS 文件格式"
head_description: "GroupDocs.Assembly Java API 允许将外部文档的内容动态插入各种文件格式，如 PDF、DOCX、RTF、XLSX、CSV、PPTX、EML、MSG 等。"

############################# Header ############################
title: "Java API 将外部文档的内容插入其他支持的文件格式"
description: "GroupDocs.Assembly for Java 提供了将外部文档内容插入报告、电子邮件和各种支持的文件格式（如 PDF、DOC、DOCX、XLSX、CSV、PPTX、EML、MSG 等）的功能。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何通过 Java 将外部文档的内容插入其他流行的文件格式？"
    content: |
       文档或文件是包含信息的电子副本或硬拷贝，用户可以在以后的某个阶段检索这些信息。根据 Wikipedia，文档可以是结构化的，例如表格文档、列表、表格或科学图表，也可以是半结构化的，例如书籍或报纸文章，或者是非结构化的，例如手写笔记。 GroupDocs.Assembly for Java 是一个非常有用的 API，它使软件开发人员能够为文档自动化和报告构建强大的应用程序。它完全支持识别和处理多种文档格式，例如 PDF、Microsoft Word、Excel 工作表、PowerPoint、HTML、Outlook 电子邮件等等。它支持许多用于处理报告的高级功能，例如操作模板元素、列表报告、图表报告、表格报告等。此外，该 API 还完全支持与文档内容添加和修改相关的多项高级功能，例如向文档页面添加内容、向电子表格单元格插入数据、内容替换、向演示幻灯片添加内容等等。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 将外部文件内容添加到 Word 文档"
      content_left: |
       GroupDocs.Assembly Java API 帮助计算机程序员在他们自己的 Java 应用程序中处理文档操作任务。 它完全支持外部文档的文件内容到各种类型的文档类型。 下面的 Java 代码示例展示了如何仅用几行代码将外部文件的内容添加到文字处理文档中。

      title_right: "如何将文档内容插入 PS 文件"
      content_right: |
        * 设置源文档模板
        * 设置目标文件报告
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 方法来组装文档。 它支持
           * 从中读取模板文档的流。
           * 写入结果文档的流。
           * 指定文件加载和保存的附加选项。
           * 提供有关要使用的数据源对象的信息。

      gisthash: "abb65f9e514add59870865121ed3c526"
      gistfile: "insert_documents_to_word_processing.java"

    - title_left: "通过 Java 将外部文件的内容添加到电子邮件中"
      content_left: |
       GroupDocs.Assembly Java API 包含将动态外部文档的内容插入到几种流行的文档文件格式和电子邮件消息的功能。 下面的 java 代码展示了程序员如何在没有任何外部应用程序的情况下将外部文档的内容添加到他们的电子邮件文档中。

      title_right: "如何将文件内容添加到 PS 文档"
      content_right: |
        * 设置源文档模板
        * 设置目标文件报告
        * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 类的实例
        * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 方法来组装文档。 它支持
          * 从中读取模板文档的流。
          * 写入结果文档的流。
          * 指定文件加载和保存的附加选项。
          * 提供有关要使用的数据源对象的信息。

      gisthash: "b72d7608548993ffbe62f97c798ba021"
      gistfile: "Insert_dynamic_documents_to_emails.java"

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