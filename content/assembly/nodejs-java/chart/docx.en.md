



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:00
draft: false
lang: en
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Insert Charts in DOCX Files with JavaScript"
head_description: "With GroupDocs.Assembly for Node.js via Java, developers can quickly create and embed dynamic charts into documents using live data sources."

############################# Header ############################
title: "Easily Add Charts to DOCX Files Using Node.js" 
description: "GroupDocs.Assembly for Node.js via Java streamlines the process of integrating charts into DOCX documents with real-time data input."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Start Free Today"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) is a robust solution for creating automated documents and reports. Add charts, tables, images, barcodes, and lists to files with precision and ease. This versatile platform supports over 50 formats, including PDFs, Office documents, and emails.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to Add a Chart to a DOCX Document"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) makes adding charts to DOCX files easy. Choose from chart types like bar, line, or pie charts.
      
      1. Design a DOCX template with placeholders for charts.
      2. Load data from a supported source.
      3. Configure chart options, including type, colors, and labels.
      4. Export the document with the embedded chart.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Example document"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Include this tag in your template to generate a chart
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specify the template file path
        const template = "chart_template.docx";

        // Extract data from your source system
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Save the final document with the embedded chart
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Embed Charts Effortlessly in Your Documents"
  description: "GroupDocs.Assembly for Node.js via Java makes it simple to generate feature-rich documents in popular file types. Use templates to add charts, tables, barcodes, lists, images, and more with real-time data updates."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Top Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Transform Data into Professional Charts"
      content: "Convert data from sources like JSON, XML, or CSV into high-quality charts that can be directly embedded into documents."

    # feature loop
    - title: "Create Stunning Visuals"
      content: "Generate bar charts, pie graphs, and line charts that work seamlessly with other document elements like images, tables, and barcodes."

    # feature loop
    - title: "Flexible Chart Styling and Placement"
      content: "Use LINQ templates to control chart positioning and styling, including colors, layouts, and labels, for a polished presentation."

    # feature loop
    - title: "Supports Many File Formats"
      content: "Generate documents in formats like MS Office, PDF, OpenOffice, and HTML, with charts perfectly integrated for a professional finish."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dynamically Generate and Insert Charts"
      content: |
        This example illustrates how to create and embed charts into DOCX files programmatically.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Set up a template with a placeholder for the chart
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Define the path to the template file
          const template = "table_template.docx";

          // Retrieve data from a chosen source
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Prepare a data object containing the chart information
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Choose the chart type and customize its appearance
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Initialize DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Save the updated document with the chart embedded
          asm.assembleDocument(template, "result.docx", data, design);
          ```
        platform: "java"
        copy_title: "Copy"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Ready to begin?"
  description: "Explore GroupDocs.Assembly features for free or request a license"
  items:
    #  loop
    - title: "Download from NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Learn about licensing"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Discover Advanced Features"
    exclude: "chart"
    description: "This platform simplifies document creation with tools designed for data visualization and seamless integration."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Generate Reports in Multiple File Formats"
    exclude: "DOCX"
    description: "Node.js via Java supports over 50 formats, making it easy to combine templates with data to produce polished documents."
    items: 
          
        # format loop 1
        - name: "Charts in PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Charts in DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Charts in PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Charts in XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---