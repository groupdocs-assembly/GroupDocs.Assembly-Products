---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/assembly/java/barcode/tiff/"
otherformats: PDF HTML XPS MHTML TXT XAML EPUB SVG PS PCL XML OXPS MD EML EMLX MSG 

############################# Head ############################
head_title: "用于生成条码图像文档和电子邮件消息的 Java API"
head_description: "GroupDocs.Assembly Java API 使程序员能够在文档（PDF、DOC、DOCX、RTF、XLSX、CSV、PPTX）和电子邮件（EML EMLX MSG）消息中创建和添加条码。"

############################# Header ############################
title: "Java Barcodes Generator API - 在 TIFF 文档中创建一维和二维条码"
description: "GroupDocs.Assembly Java API 允许在 PDF HTML、XPS、PS、TXT、EPUB、PCL、SVG、文档和电子邮件（EML、EMLX、MSG）消息中生成和添加一维和二维条码图像。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在文档和电子邮件中生成和插入条形码？"
    content: |
      条码越来越流行，如今无处不在。它于 1970 年代中期开始出现在杂货店中，如今可以在书籍、门票、跟踪药物的医院、汽车零部件商店等中找到。该网页将解释如何在 Java 应用程序中的文档和电子邮件中动态创建和添加条形码图像。 GroupDocs.Assembly for Java 是一个非常有用的 API，可帮助软件开发人员创建强大的文档自动化和报告应用程序。它支持处理许多流行的文档格式，例如 PDF、HTML、XPS、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿、Outlook 电子邮件等等。 Java API 使得在文档和电子邮件消息中创建和插入条形码图像变得很容易，只需几行代码。它还支持修改条码图像属性，例如缩放条码图像、更改前后颜色、更改条码图像分辨率、条码文本位置、更改字体等。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 在 TIFF 文档中创建条码"
      content_left: |
       GroupDocs.Assembly Java 包含用于在 TIFF 文档中插入和编辑条形码的完整功能。 以下 Java 代码示例演示了如何通过几行代码在 TIFF 文档中创建和使用条形码图像。 

      title_right: "如何在 TIFF 文件中添加条形码？"
      content_right: |
       * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)  的实例
       * 创建示例数据源对象
       * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.DataSourceInfo...-) 具有以下参数的方法
           * 从流中读取模板文档。
           * Stream 写入生成的文档。
           *文档加载和保存选项。
           * 详细信息 有关要使用的数据源对象的信息。

      gisthash: "ebb6d8215f329f457f843e9a9fc48c9c"
      gistfile: "generate_barcodes_in_presentations.java"     

    - title_left: "系统要求"
      content_left: |
        所有主要平台和操作系统都支持 GroupDocs.Assembly Java API。 它可以生成 Microsoft Word、Excel、PowerPoint、Outlook、OpenOffice 和 50 多种其他格式的文档。 如需完整的系统要求指南，请访问 [系统要求](https://docs.groupdocs.com/assembly/java/system-requirements/) 在执行以下代码之前，请确保您已安装以下先决条件 系统：
         * 操作系统：Microsoft Windows、Linux、MacOS
         * Java 版本支持：J2SE 7.0 (1.7)、J2SE 8.0 (1.8) 或以上
         * 从 [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/) 获取最新版本的 GroupDocs.Assembly Java API
        
      title_right: "为什么使用 GroupDocs.Assembly"
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