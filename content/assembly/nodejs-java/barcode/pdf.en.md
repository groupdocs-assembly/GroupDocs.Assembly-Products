



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:13
draft: false
lang: en
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add Barcodes to PDF Files Using JavaScript"
head_description: "Easily generate and embed barcodes in your documents and emails with the GroupDocs.Assembly for Node.js via Java API."

############################# Header ############################
title: "Create Barcodes for PDF Files Using Node.js" 
description: "With GroupDocs.Assembly for Node.js via Java, you can dynamically generate, customize, and embed barcodes into PDF documents."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get Started"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction to GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) allows you to create professional documents by combining data from multiple sources. Add charts, tables, lists, images, and barcodes to your files with ease. Use templates to organize content exactly where it belongs. Works with more than 50 formats, including PDFs, Office documents, and emails.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to Add a Barcode in PDF Files"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) makes it easy to embed barcodes in PDF documents. It supports over 60 barcode types, including 1D and 2D formats.
      
      1. Design a template with barcode placeholders (PDF templates are not supported).
      2. Retrieve data from a compatible source.
      3. Set barcode options such as size and resolution.
      4. Export the document with the barcode as a PDF file.
   
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
        // Use this tag in the template to include a barcode in the output document
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specify the path to the template file
        // Note: PDF templates are currently unsupported.
        const template = "barcode_template.docx";

        // Load the required data from your source
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Export the document with the barcode as a PDF file.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Generate Documents with Data-Driven Templates"
  description: "With GroupDocs.Assembly for Node.js via Java, you can create professional files in popular formats by seamlessly embedding charts, tables, lists, links, images, and barcodes."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Core Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Build Reports with Business Data"
      content: "Use the API to populate templates with data from formats like JSON, XML, and CSV quickly and accurately."

    # feature loop
    - title: "Add Visual Elements"
      content: "GroupDocs.Assembly supports inserting elements such as charts, tables, lists, text, links, images, and barcodes in real time."

    # feature loop
    - title: "Control Data Placement"
      content: "With LINQ-based templates, you can precisely position data, loop through arrays, and apply custom formatting programmatically."

    # feature loop
    - title: "Compatible with Many Formats"
      content: "Work with files like MS Office documents, PDFs, HTML, OpenOffice files, and emails. Merge multiple documents when needed."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Example: Generate a Barcode Programmatically"
      content: |
        This example demonstrates how to programmatically generate and insert a barcode into a PDF document.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Design a template with a barcode placeholder
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Specify the template file's path
          // Note: PDF templates are currently unsupported.
          const template = "barcode_template.docx";

          // Retrieve data from your source
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Create a data source object with the required details
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Initialize an instance of DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Set up the barcode configuration
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Save the document with the barcode included
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "Explore Key Features"
    exclude: "barcode"
    description: "Simplify document processing with advanced tools and automation capabilities."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Supported File Formats for Report Creation"
    exclude: "PDF"
    description: "Node.js via Java handles over 50 file types, making it simple to merge data and process templates for high-quality results."
    items: 
          
        # format loop 1
        - name: "Add a barcode to a PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add a barcode to a DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add a barcode to a PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Add a barcode to an XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---