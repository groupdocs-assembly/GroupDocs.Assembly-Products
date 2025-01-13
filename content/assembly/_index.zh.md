---
############################# Static ############################
layout: "family"
date:  2025-01-13T15:11:22
draft: false

product: "Assembly"
product_tag: "assembly"

lang: zh

############################# Head ############################
head_title: "GroupDocs的.NET、Java API和在线文档生成应用"
head_description: "获取针对.NET和Java应用的全能文档自动化与报告解决方案。根据自定义模板和数据生成所有常见文档。"

############################# Header ############################
title: "文档自动化和报告解决方案"
description:  |
  使用我们的跨平台应用和API，通过模板和数据源轻松生成详细报告。

  使用具有灵活标记的模板生成Word、Excel、演示文稿等格式的报告。

  使用来自JSON、XML、CSV等源的数据填充图表、条形码、表格和其他元素。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "选择您的平台"
  title: "平台独立性"
  description: "GroupDocs.Assembly 兼容以下操作系统和框架："
  details_link_title: "了解更多"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 任何其他文本编辑器
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Assembly 的主要特点"
  description: "该解决方案帮助您在流行的文档格式中创建报告，自动填充您的业务数据。自动化您的文档生成任务。"

  items:
    # items loop
    - icon: "additional"
      title: "用数据填充模板"
      content: "使用来自支持来源的数据填充报告。"

    # items loop
    - icon: "manipulate"
      title: "灵活的标记"
      content: "以可定制的方式向文档添加数据。"

    # items loop
    - icon: "structure"
      title: "本地文档功能"
      content: "使用表格、图表和条形码显示数据。"

    # items loop
    - icon: "merge"
      title: "所有流行格式"
      content: "支持所有常用文档格式。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "生成定制良好的报告"
  description: "GroupDocs.Assembly 代码示例"
  items:
    # code sample loop
    - title: "使用生成的条形码"
      content: |
       GroupDocs.Assembly 允许在报告模板中使用条形码标记。在创建报告时，基于标记和提供的数据生成条形码。指定包含文本、数据对象和标记的模板路径。同时，指定数据源以填充条形码内容。
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // 创建 DocumentAssembler 类的实例
            DocumentAssembler assembler = new DocumentAssembler();

            //指定模板的路径
            var tmp_path = "barcode_template.docx";

            //指定结果文档的路径
            var res_path = "result.docx";

            //创建数据源的实例
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //调用 AssembleDocument 生成报告
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // 创建 DocumentAssembler 类的实例
            DocumentAssembler assembler = new DocumentAssembler();
            
            //指定模板的路径
            String tmp_path = "barcode_template.docx";

            //指定结果文档的路径
            String res_path = "result.docx";

            //创建数据源的实例
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // 调用 AssembleDocument 生成报告
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // 创建 DocumentAssembler 类的实例
            const assembler = new assemblyLib.DocumentAssembler();
            
            //指定模板的路径
            const tmp_path = "barcode_template.docx";

            //指定结果文档的路径
            const res_path = "result.docx";

            //创建数据源的实例
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // 调用 AssembleDocument 生成报告
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "支持50多种文件格式"
  description: "GroupDocs.Assembly 可以处理几乎所有流行的文件格式。"

############################# Metrics ###############################
metrics:
  enable: true
  title: "我们的产品统计数据"
  description: "探索产品指标，以获取我们进展、影响和增长的见解。"

  items:
    # items loop
    - number: "50+"
      title: "支持的格式"
      content: "我们支持50多种最常用的文档格式。"

    # items loop
    - number: "650k"
      title: "NuGet 下载"
      content: "GroupDocs.Assembly for .NET 是一个流行的库，在NuGet上有超过650,000次下载。"

    # items loop
    - number: "18k"
      title: "Maven 下载"
      content: "Java开发者在Maven上下载了GroupDocs.Assembly超过18,000次。"

    # items loop
    - number: "150+"
      title: "满意客户"
      content: "我们的产品受到全球各地的个人开发者和领先公司的信任，以创建创新解决方案。"


############################# Customers ###############################
customers:
  enable: true
  title: "我们的满意客户"
  description: "GroupDocs库被全球一些最著名和备受尊敬的品牌使用。"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "准备开始吗？"
  description: "在您的平台上免费测试GroupDocs.Assembly的功能。"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "常见问题"
  description: "浏览我们的常见问题。"

  items:
    # items loop
    - question: "GroupDocs.Assembly 是否需要任何外部库来进行文档构建？"
      answer: "不，GroupDocs.Assembly 独立工作，不需要像Adobe Acrobat或Microsoft Office这样的第三方库。"

    # items loop
    - question: "我可以在购买之前测试GroupDocs.Assembly的功能吗？"
      answer: "可以！GroupDocs.Assembly 提供免费试用。安装并探索其功能。试用版本会在您的文档中添加“试用标签”，并仅处理前3页。要获得完整体验，请获取免费的30天临时许可证以访问所有功能。有关更多细节，请查看[临时许可证](https://purchase.groupdocs.com/temporary-license/)。"

    # items loop
    - question: "有哪些类型的许可证可用？"
      answer: "您在寻找GroupDocs.Assembly许可证吗？我们提供多种选项以满足您的需求。根据团队规模、部署位置（单个办公室或远程）以及您是否需要与客户共享SDK/API进行分发进行选择。或者，选择按月计费的使用许可证，仅为您使用的部分付费。您可以在[定价](https://purchase.groupdocs.com/pricing/assembly/net/)下找到适合您的最佳选项。"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Assembly 低代码 API"
  description: "通过我们的基于云的REST API使用您的应用生成文档。"
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "使用cURL RESTful API将数据添加到Word、Excel、PowerPoint和其他许多模板中。"
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "通过云SDK增强您的.NET应用程序。以您的自定义格式显示业务数据。"
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK为Java应用程序提供不同的选项，以生成各种类型的文档。"
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Assembly 网络应用"
  description: "GroupDocs.Assembly 提供免费的网络应用程序以生成文档。您可以直接在浏览器中处理50多种流行的文件格式，完全免费。"

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "直接从您的网页浏览器生成Excel、Word、PowerPoint等文件类型的报告。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "从模板和数据源创建Microsoft Word文档。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "上传模板和数据源免费生成Excel报告。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---