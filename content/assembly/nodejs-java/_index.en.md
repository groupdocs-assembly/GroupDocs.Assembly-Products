---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: en
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Toolkit for Building, Automating, and Customizing Documents"
head_description: "Node.js library for automating document workflows. Generate PDF, Word, Excel, PowerPoint, HTML, and email files from your templates."

############################# Header ############################
title: "Node.js API for Simplified Document and Report Automation"
description: "Streamline JavaScript report generation by merging your data with pre-built templates."
words:
  for: "for"

actions:
  main: "Start Your Trial on NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Ready to Get Started?"
  description: "Try the features of GroupDocs.Assembly for free or request a license."

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Create a Chart in a Word Document Using Node.js"
  more: "More examples"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Path to the main template
    const template = "chart_template.docx";

    // Retrieve managers' productivity data from the source
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Create an instance of DataSourceInfo with the data
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Set chart colors using another DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Fill the template with data and save it to the output
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly Overview"
  description: "A Node.js library built for creating documents programmatically with integrated data handling."
  features:
    # feature loop
    - title: "Integrate Business Data into Templates with JavaScript"
      content: "Generate polished reports by embedding JSON, XML, or other data into templates with GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Manage Embedded Content"
      content: "Automatically populate tables, charts, and other visuals in your documents using external data."

    # feature loop
    - title: "Customizable Options"
      content: "GroupDocs.Assembly for Node.js via Java allows you to add features like barcodes, fetch data from URLs, and export files in various formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Assembly for Node.js via Java integrates smoothly with leading operating systems, frameworks, and package managers."
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
    GroupDocs.Assembly for Node.js via Java supports a broad array of [document formats](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "Core Features of GroupDocs.Assembly"
  description: "Create dynamic documents and reports with powerful data management tools."

  items:
    # feature loop
    - icon: "preview"
      title: "Rich Data Visuals"
      content: "Easily insert charts, tables, images, and lists into your documents with full customization."

    # feature loop
    - icon: "manipulate"
      title: "Transform Your Data"
      content: "Leverage tools like formulas and sorting to structure and display information effectively."

    # feature loop
    - icon: "two_pages"
      title: "Wide Format Compatibility"
      content: "Work seamlessly with popular file formats for templates and outputs."

    # feature loop
    - icon: "document_settings"
      title: "Advanced Template Customization"
      content: "Format templates with numeric, alphabetic, and other styling options."

    # feature loop
    - icon: "text"
      title: "Generate Barcodes Dynamically"
      content: "Create and embed barcode images directly into your documents on demand."

    # feature loop
    - icon: "add"
      title: "Flexible Text Styling"
      content: "Easily apply text styles like capitalization or title case in your templates."

    # feature loop
    - icon: "manipulate"
      title: "Dynamic Content Insertion"
      content: "Include content from external files dynamically during document generation."

    # feature loop
    - icon: "convert"
      title: "Export to Various Formats"
      content: "Save documents in multiple formats with your specified configurations."

    # feature loop
    - icon: "update"
      title: "Embed Media Dynamically"
      content: "Insert images or other elements using Base64 data when creating documents."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Discover practical examples of how to use GroupDocs.Assembly for common tasks."
  items:
    # code sample loop
    - title: "Add a Bulleted List in Word Documents"
      content: |
        See how to create [bulleted lists](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) in Word documents to organize data effectively. This example demonstrates how to generate a bulleted list using GroupDocs.Assembly.
        {{< landing/code title="Add a Bulleted List in Word Documents">}}
        ```javascript {style=abap}
        // Insert this template on a document page:
        // Managers' performance indicators
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specify the template path
        const template = "Bulleted List Template.docx";

        // Set the output file path
        const result = "Result Report.docx"

        // Retrieve managers' data from a JSON source
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Generate the report with the filled data
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Insert Pie Charts into PowerPoint"
      content: |
        Learn how to use templates and XML to add [pie charts](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) in your presentations. Enhance your reports with pie charts to present data visually and clearly.
        {{< landing/code title="Insert Pie Charts into PowerPoint">}}
        ```javascript {style=abap} 
        // Add the chart title template to the presentation:
        // Customers' revenue <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Also include the chart data template:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specify the chart template path
        const template = "Pie Chart Template.pptx";

        // Set the output file path
        const result = "Result Report.pptx"

        // Retrieve customers' data from an XML source
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Generate the chart and save the result
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---