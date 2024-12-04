



---
############################# Static ############################
layout: "format"
date:  2024-12-04T15:35:32
draft: false
lang: en
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Create tables in PDF documents with C#"
head_description: "The GroupDocs.Assembly for .NET API allows developers to effortlessly add and populate tables in documents and emails with data from dynamic sources."

############################# Header ############################
title: "Generate data tables in PDF documents using our .NET API" 
description: "GroupDocs.Assembly for .NET makes it easy to dynamically fill tables in PDF documents with data from various sources."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Free Trial"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET Overview"
    link: "/assembly/net/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) is built to create documents and reports by filling templates with data from multiple sources. Effortlessly insert structured data into tables, lists, and charts, or embed images dynamically. Advanced syntax ensures accurate data placement. Supports over 50 formats, including PDFs, MS Office documents, and email files.

############################# Steps ############################
steps:
    enable: true
    title: "How to populate a table in a PDF document"
    content: |
      [GroupDocs.Assembly](/assembly/net/) lets you dynamically populate tables in templates for formats like PDF. Insert data from various sources into your tables.
      
      1. Create a PDF template with table placeholders.
      2. Fetch data from any supported source.
      3. Filter the data to include only the required information.
      4. Save the document with the populated table.
   
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
        // Add these tags into a template table row
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Set the file path for the template
        string template = "table_template.pdf";

        // Fetch data from a supported source
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Save the document with the table filled with data
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Generate documents with dynamic tables"
  description: "GroupDocs.Assembly for .NET streamlines document creation by automating table population and supporting additional elements like charts, lists, and images through templates and advanced markup."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Create reports from structured data"
      content: "The API processes data from sources such as JSON, XML, and CSV to populate tables in office documents efficiently and accurately."

    # feature loop
    - title: "Display data visually"
      content: "GroupDocs.Assembly enables the creation of tables, lists, and charts, along with embedding text, links, and images for professional document design."

    # feature loop
    - title: "Precisely position table data"
      content: "Use LINQ-based syntax to dynamically add table rows and columns. Customize styles, including colors and formatting, programmatically."

    # feature loop
    - title: "Supports a wide range of formats"
      content: "Easily handle popular file formats like MS Office, OpenOffice, PDF, and HTML. Seamlessly insert populated tables into supported document types."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to dynamically populate a data table"
      content: |
        This example demonstrates how to fill a table in a PDF document using dynamic data.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepare a template with a placeholder for the table
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Specify the file path to the template
          string template = "table_template.pdf";

          // Retrieve data from your chosen source
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Create a data source object with the necessary data
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Initialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Save the completed document with the populated table
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    title: "Explore key features"
    exclude: "table"
    description: "Our solution simplifies the creation of professional documents with dynamically populated tables and additional elements."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "diagram"
          link: "/assembly/net/diagram/pdf/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Create reports with detailed tables"
    exclude: "PDF"
    description: ".NET enables the creation of comprehensive reports by filling templates with tables and other data elements in over 50 supported formats."
    items: 
          
        # format loop 1
        - name: "Add a table to a PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add a table to a DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add a table to a PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Add a table to an XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---