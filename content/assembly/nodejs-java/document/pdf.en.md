



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:15
draft: false
lang: en
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Merge Documents in PDF with JavaScript"
head_description: "Easily combine PDF files using JavaScript. GroupDocs.Assembly streamlines document merging in just a few simple steps."

############################# Header ############################
title: "Effortlessly Combine Content in PDF Files" 
description: "With GroupDocs.Assembly for Node.js via Java, integrating one PDF file into another is quick and precise. Enjoy flexible, reliable tools for seamless merging."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try It Free"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) offers a powerful way to manage documents. Merge one file into another with ease while supporting over 50 formats, such as PDF and MS Office. Customize layouts, edit content, and organize documents exactly how you need.

############################# Steps ############################
steps:
    enable: true
    title: "How to Merge a Document into a PDF File"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) makes it easy to insert one PDF file into another with customizable options.
      
      1. Design a template with placeholders for embedded content (PDF templates are unsupported).
      2. Set the file path for the template.
      3. Provide the file path for the document to merge.
      4. Save the completed document with the merged content as a PDF file.
   
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
        // Insert this tag into your template to define where the document will be embedded
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Set the file path for the main template
        // Currently, PDF templates are not supported.
        const template = "doc_template.docx";

        // Provide the path for the document you wish to merge
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // Save the final output with the embedded document
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Powerful Tools for Document Integration"
  description: "GroupDocs.Assembly for Node.js via Java makes embedding files across various formats easy and fully customizable. Deliver consistent, professional results every time."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Generate Reports with Business Data"
      content: "Pull data from JSON, XML, or CSV sources to create comprehensive reports and documents quickly and accurately."

    # feature loop
    - title: "Add Rich Visual Elements"
      content: "GroupDocs.Assembly enables you to include tables, charts, lists, images, and barcodes alongside text and hyperlinks."

    # feature loop
    - title: "Precise Data Placement"
      content: "Use LINQ templates to position data exactly where it belongs, handle repeating items like arrays, and customize styles effortlessly."

    # feature loop
    - title: "Works with a Variety of Formats"
      content: "Merge content seamlessly across formats like PDFs, MS Office files, HTML, and OpenOffice, offering flexibility for all projects."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Embed an Image into a Document Programmatically"
      content: |
        This example demonstrates how to insert an image into a PDF file using GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Add a placeholder in the template for the image
          // <<image [expression]>>

          // Specify the path to the template file
          // Currently, PDF templates are not supported.
          String template = "template.docx";
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Set the path to the image you want to embed
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Initialize the DocumentAssembler object
          const asm = new assemblyLib.DocumentAssembler();

          // Save the document with the image included
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    exclude: "document"
    description: "Explore the comprehensive tools GroupDocs.Assembly offers for efficient and seamless document merging."
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
    title: "Combine Documents in Many Formats"
    exclude: "PDF"
    description: "Use Node.js via Java to merge content across over 50 file formats, ensuring professional and polished results."
    items: 
          
        # format loop 1
        - name: "Embed a document in a PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Embed a document in a DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Embed a document in a PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Embed a document in an XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---