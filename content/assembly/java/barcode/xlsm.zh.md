---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/assembly/java/barcode/xlsm/"
otherformats: XLS XLT XLSX XLTX XLTM XLSB ODS 

############################# Head ############################
head_title: "通过 Java API 生成条形码图像并将其插入 Excel 电子表格"
head_description: "GroupDocs.Assembly Java API 使程序员能够在 Excel（XLS、XLT、XLSX、XLSM、XLTX、XLTM 和 XLSB）电子表格文档中生成和添加条形码图像。"

############################# Header ############################
title: "通过 Java API 在 Excel 电子表格文档中创建和管理条形码"
description: "GroupDocs.Assembly Java API 使软件开发人员能够以编程方式在 Java 和 JSP 应用程序内的 Excel 电子表格文档中生成和管理条形码。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在电子表格中生成条形码图像？"
    content: |
      电子表格软件程序是一个有用的工具，允许用户存储、分析和报告大量数据。 GroupDocs.Assembly 是一个很棒的 Java API，它使软件开发人员可以轻松地在 Excel 电子表格中创建、组织和打印条形码图像。 条形码是存储机器可读信息的数字代码，可为库存系统带来速度和准确性。 使用 GroupDocs.Assembly Java API，您可以在 Microsoft Excel 电子表格中以编程方式绘制具有个性化文本、外观和不同编码类型的大量 1D 和 2D 条形码图像。 该 API 还使用户可以轻松管理他们的条码，并且不需要安装任何外部软件或第三方工具。 它支持修改条码图像大小、设置前景色和背景色、调整字体大小、条码图像分辨率调整、条码文本自动更正等功能。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 在 XLSM 电子表格中创建条形码"
      content_left: |
       GroupDocs.Assembly Java 完全支持在 XLSM 电子表格中创建和管理条形码。 以下 Java 代码演示了如何在 Microsoft Excel 电子表格文档中创建和插入条形码图像。

      title_right: "如何在 XLSM 文件中添加条形码图像"
      content_right: |
       * 创建 [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 的实例
       * 创建示例数据源对象
       * 调用 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.DataSourceInfo...-) 具有以下参数的方法
           * 从流中读取模板文档。
           * Stream 写入生成的文档。
           *文档加载和保存选项。
           * 详细信息 有关要使用的数据源对象的信息。

      gisthash: "d597241fa3f68e3945a19ef3231070eb"
      gistfile: "create_barcodes_in_spreadsheet_file.java"

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