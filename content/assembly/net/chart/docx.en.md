



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: en
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Create charts in DOCX files with C#"
head_description: "The GroupDocs.Assembly for .NET API makes it easy for developers to generate and insert charts or graphs into documents dynamically using real-time data."

############################# Header ############################
title: "Embed charts in DOCX files with .NET API" 
description: "GroupDocs.Assembly for .NET provides a powerful way to populate DOCX files with dynamic data and integrate charts effortlessly."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try Free"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) is a tool designed to streamline the creation of documents and reports by integrating data from various sources. Easily generate charts, tables, lists, barcodes, and images dynamically. Advanced formatting options allow precise placement and customization of your content. It supports over 50 file formats, including PDFs, MS Office documents, and emails.

############################# Steps ############################
steps:
    enable: true
    title: "How to add a chart to a DOCX document"
    content: |
      [GroupDocs.Assembly](/assembly/net/) makes it simple to generate and embed charts into your DOCX templates. Supports a variety of chart types, such as bar, pie, and line charts.
      
      1. Design a DOCX template with placeholders for the charts.
      2. Retrieve your data from a compatible source.
      3. Define chart options like type, labels, and color scheme.
      4. Save the updated file with the chart embedded.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Example document"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Include this tag in your template to generate a chart
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Specify the file path for your template
        string template = "chart_template.docx";

        // Load data from your preferred source
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Save the document with the chart embedded
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Add dynamic charts to your documents effortlessly"
  description: "GroupDocs.Assembly for .NET simplifies the creation of data-driven documents in widely-used formats. Use templates to insert charts, tables, barcodes, lists, hyperlinks, and images with advanced, dynamic data integration."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Convert data into professional charts"
      content: "Turn data from JSON, XML, CSV, and other sources into visually appealing charts with just a few steps using our API."

    # feature loop
    - title: "Create visually engaging content"
      content: "GroupDocs.Assembly supports multiple chart types like bar graphs, pie charts, and line graphs. Combine these with tables, barcodes, images, and other elements to create professional reports."

    # feature loop
    - title: "Precisely position and customize charts"
      content: "With LINQ syntax, you can dynamically generate and place charts exactly where needed. Easily customize styles, colors, and layout to match your requirements."

    # feature loop
    - title: "Works with various file formats"
      content: "Produce documents in popular formats like MS Office, PDF, OpenOffice, and HTML. Embed charts seamlessly into any supported format with full compatibility."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Create a chart programmatically"
      content: |
        This example demonstrates how to dynamically create and embed a chart into a DOCX document.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepare a template with a placeholder for the chart
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Provide the path to the template file
          string template = "table_template.docx";

          // Retrieve the data from your source
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Build a data object with the necessary information
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Set up chart properties such as type and appearance
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Initialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Export the document with the chart included
          asm.AssembleDocument(template, "result.docx", data, design);
          ```
        platform: "net"
        copy_title: "Copy"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download the result"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.docx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to begin?"
  description: "Explore GroupDocs.Assembly features for free or request a license"
  items:
    #  loop
    - title: "Download from Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Learn about licensing"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Discover key capabilities"
    exclude: "chart"
    description: "Our platform helps you create compelling, data-driven documents tailored to your needs."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Create visually rich reports in multiple formats"
    exclude: "DOCX"
    description: ".NET allows you to generate documents with integrated charts across 50+ supported formats, combining templates with your data seamlessly."
    items: 
          
        # format loop 1
        - name: "Charts in PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Charts in DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Charts in PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Charts in XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---