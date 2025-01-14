



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:18
draft: false
lang: en
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Insert Tables into DOCX Documents with JavaScript"
head_description: "Use GroupDocs.Assembly for Node.js via Java to quickly embed tables in documents or emails, pulling data from various sources."

############################# Header ############################
title: "Effortlessly Add Tables to DOCX Files with Node.js" 
description: "With GroupDocs.Assembly for Node.js via Java, filling tables in DOCX documents is simple, using data from multiple sources."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Start Your Free Trial"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction to GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) is a powerful tool for automating document creation. It lets you easily insert tables, charts, lists, and images into templates, with precise content placement. Supporting over 50 file formats, including PDF, Word, and email, it streamlines report generation and other tasks.

############################# Steps ############################
steps:
    enable: true
    title: "How to Add Data to a Table in DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) enables you to quickly populate table templates for DOCX files using dynamic data sources.
      
      1. Create a DOCX template with placeholders for table rows and columns.
      2. Load data from a supported source like JSON or CSV.
      3. Organize and format the data as needed.
      4. Generate the document with the completed table.
   
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
        // Include these tags in the table row placeholders of your template
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specify the template file path
        const template = "table_template.docx";

        // Load your data from a chosen source
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Save the final document with the completed table
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Easily Add Data-Driven Tables to Documents"
  description: "GroupDocs.Assembly for Node.js via Java allows users to create tables automatically, while also embedding charts, images, and lists using template-based workflows."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Top Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Generate Tables from Structured Data"
      content: "Fetch data from JSON, XML, CSV, and other formats to automatically populate document tables."

    # feature loop
    - title: "Create Polished Visual Content"
      content: "Use GroupDocs.Assembly to design professional tables, charts, and lists, and to add links, images, and text for a refined document appearance."

    # feature loop
    - title: "Dynamic Table Content Placement"
      content: "Add rows and columns programmatically using LINQ-based templates, and customize styles like fonts, colors, and alignment."

    # feature loop
    - title: "Works Seamlessly Across Formats"
      content: "Easily create or edit tables in MS Office, OpenOffice, PDF, HTML, and other formats, merging them into files as needed."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to Programmatically Populate a Table"
      content: |
        This example demonstrates filling a table in a DOCX document with data from an external source.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Design a template with placeholders for the table
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Specify the file path to the template
          const template = "table_template.docx";

          // Load the required data from your source
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Organize the data into the necessary structure
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Initialize DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Save the output document with the completed table
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    title: "Core Features at a Glance"
    exclude: "table"
    description: "Our API automates table creation and enhances document generation with versatile tools and templates."
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
    title: "Generate Tables in a Variety of Formats"
    exclude: "DOCX"
    description: "With Node.js via Java, populate templates and create comprehensive tables across more than 50 supported file types."
    items: 
          
        # format loop 1
        - name: "Add a table to a PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add a table to a DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add a table to a PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Add a table to an XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---