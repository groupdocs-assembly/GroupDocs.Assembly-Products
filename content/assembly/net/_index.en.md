---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: en
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET API for Document Automation, Assembly & Report Generation"
head_description: "C# .NET API for document automation, assembly, and report generation. Create PDF, Word, Excel, PPTX, HTML, and email documents from custom templates."

############################# Header ############################
title: ".NET Document Automation & Reporting API"
description: "Generate reports in .NET applications by defining templates and merging data."
words:
  for: "for"

actions:
  main: "Download Trial via Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Ready to Get Started?"
  description: "Try the features of GroupDocs.Assembly for free or request a license."

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Fill a Chart in DOCX Using C#"
  more: "More examples"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Path to the main template
    string template = "chart_template.docx";

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
  description: ".NET solution for automating document creation with advanced data integration."
  features:
    # feature loop
    - title: "Add Business Data to Document Templates with C#"
      content: "Report generation made easy: With GroupDocs.Assembly for .NET, you can effortlessly insert data from sources like JSON or XML into predefined templates."

    # feature loop
    - title: "Process Native Data Objects"
      content: "Supported document types include embedded objects like diagrams, charts, tables, and lists that can be populated automatically with data."

    # feature loop
    - title: "Additional Features"
      content: "GroupDocs.Assembly for .NET provides extensive customization options. Programmatically design data objects, generate barcodes, use online data sources via URLs, and save output in various formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Assembly for .NET is compatible with the following operating systems, frameworks, and package managers."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Assembly for .NET can process the following [file formats](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "GroupDocs.Assembly Features"
  description: "Create documents and reports using advanced data models."

  items:
    # feature loop
    - icon: "preview"
      title: "Advanced Data Representation"
      content: "Supports a wide range of data objects such as charts, lists, tables, images, and more."

    # feature loop
    - icon: "manipulate"
      title: "Data Manipulation"
      content: "Apply formulas and sequential operations to format and display data effectively."

    # feature loop
    - icon: "two_pages"
      title: "Wide Range of Supported Formats"
      content: "Work seamlessly with all common document formats for templates or output files."

    # feature loop
    - icon: "document_settings"
      title: "Rich Template Markup"
      content: "Leverage ordinal, cardinal, and alphabetic numeric formatting in templates."

    # feature loop
    - icon: "text"
      title: "Embed Barcodes"
      content: "Generate barcode images dynamically and insert them into your documents."

    # feature loop
    - icon: "add"
      title: "Data Formatting"
      content: "Format strings in templates as uppercase, lowercase, capitalized, or first-letter capital styles."

    # feature loop
    - icon: "manipulate"
      title: "Document Content Manipulation"
      content: "Dynamically insert content from external documents into your reports."

    # feature loop
    - icon: "convert"
      title: "Save in Multiple Formats"
      content: "Specify the output file format using file extensions or detailed configurations."

    # feature loop
    - icon: "update"
      title: "Flexible Data Processing"
      content: "Insert images and documents dynamically using Base64-encoded bytes."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Code snippets for typical GroupDocs.Assembly operations."
  items:
    # code sample loop
    - title: "Bulleted List in a Microsoft Word Document"
      content: |
        [Bulleted lists](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) are a common way to present business data. Here's an example of adding a list to a Word document using GroupDocs.Assembly.
        {{< landing/code title="How to Populate a List in Documents">}}
        ```csharp {style=abap}
        // Insert this template on a document page:
        // Managers' performance indicators
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Specify the template path
        string template = "Bulleted List Template.docx";

        // Set the output file path
        string result = "Result Report.docx"

        // Retrieve managers' data from a JSON source
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Generate the report with the filled data
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Pie Charts in PPTX Presentations"
      content: |
        You can create [Pie Charts](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) using templates and XML data. Enhance your reports with visually appealing data representations.
        {{< landing/code title="How to Represent Data in a Pie Chart">}}
        ```csharp {style=abap}
        // Add the chart title template to the presentation:
        // Customers' revenue <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Also include the chart data template:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Specify the chart template path
        string template = "Pie Chart Template.pptx";

        // Set the output file path
        string result = "Result Report.pptx"

        // Retrieve customers' data from an XML source
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Generate the chart and save the result
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---