---
############################# Static ############################
layout: "landing"
date: 2024-11-28T14:09:03
draft: false

lang: en
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "Java Library for Document Creation, Automation & Reporting"
head_description: "Java library for automating document creation and generating reports. Create PDF, Word, Excel, PPTX, HTML, and email documents using custom templates."

############################# Header ############################
title: "Java API for Automating Reports and Documents"
description: "Simplify report generation in Java by merging data with templates."
words:
  for: "for"

actions:
  main: "Get Trial via NuGet"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Ready to Get Started?"
  description: "Try the features of GroupDocs.Assembly for free or request a license."

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Generate a Chart in DOCX with Java"
  more: "More examples"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    String template = "chart_template.docx";

    // Retrieve managers' productivity data from the source
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Create an instance of DataSourceInfo with the data
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Set chart colors using another DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Fill the template with data and save it to the output
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly Overview"
  description: "A Java library designed for automated document creation and seamless data integration."
  features:
    # feature loop
    - title: "Merge Business Data into Templates with Java"
      content: "Easily create professional reports by embedding data from JSON, XML, or other sources into pre-designed templates using GroupDocs.Assembly for Java."

    # feature loop
    - title: "Work with Embedded Objects"
      content: "Automatically populate elements like tables, charts, and diagrams in documents using data from external sources."

    # feature loop
    - title: "Advanced Customization"
      content: "GroupDocs.Assembly for Java offers flexible features like generating barcodes, pulling online data through URLs, and exporting output in different formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Assembly for Java works seamlessly with popular operating systems, development frameworks, and package managers."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Assembly for Java supports a wide range of [document formats](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formats
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Images & Other Formats
        * **Portable:** PDF
        * **Images:** SVG, TIFF
        * **Other office formats:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Other formats
        * **Web:** HTML, MHTML
        * **Emails:** EML, MSG, EMLX
        * **Other:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Key Capabilities of GroupDocs.Assembly"
  description: "Create professional documents and reports with advanced data handling."

  items:
    # feature loop
    - icon: "preview"
      title: "Visual Data Elements"
      content: "Add and format elements like charts, tables, images, and lists directly in your documents."

    # feature loop
    - icon: "manipulate"
      title: "Data Transformation"
      content: "Use formulas, sorting, and other tools to organize and present your data effectively."

    # feature loop
    - icon: "two_pages"
      title: "Support for Multiple Formats"
      content: "Easily work with common file types for both templates and output files."

    # feature loop
    - icon: "document_settings"
      title: "Enhanced Template Formatting"
      content: "Customize templates with numeric, alphabetic, and other advanced formatting options."

    # feature loop
    - icon: "text"
      title: "Dynamic Barcode Generation"
      content: "Quickly create and insert barcode images into documents as needed."

    # feature loop
    - icon: "add"
      title: "Flexible Text Styling"
      content: "Apply text transformations like uppercase, lowercase, title case, or other styles in templates."

    # feature loop
    - icon: "manipulate"
      title: "Import External Content"
      content: "Embed content from external files dynamically while generating documents."

    # feature loop
    - icon: "convert"
      title: "Export in Multiple Formats"
      content: "Save final documents in various file formats using specified extensions or configurations."

    # feature loop
    - icon: "update"
      title: "Dynamic Media Embedding"
      content: "Insert images or other content using Base64-encoded data during document creation."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Explore sample code for common tasks with GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Create a Bulleted List in Word"
      content: |
        Learn how to add [bulleted lists](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) to Word documents for organized data representation. This example shows how to generate a list in Word using GroupDocs.Assembly.
        {{< landing/code title="Create a Bulleted List in Word">}}
        ```java {style=abap}
        // Insert this template on a document page:
        // Managers' performance indicators
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Specify the template path
        String template = "Bulleted List Template.docx";

        // Set the output file path
        String result = "Result Report.docx"

        // Retrieve managers' data from a JSON source
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Generate the report with the filled data
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Create Pie Charts in PPTX"
      content: |
        Use templates and XML to add [pie charts](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) to your presentations. Make your reports more engaging by including pie charts to visualize data.
        {{< landing/code title="Create Pie Charts in PPTX">}}
        ```java {style=abap}   
        // Add the chart title template to the presentation:
        // Customers' revenue <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Also include the chart data template:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Specify the chart template path
        String template = "Pie Chart Template.pptx";

        // Set the output file path
        String result = "Result Report.pptx"

        // Retrieve customers' data from an XML source
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Generate the chart and save the result
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---