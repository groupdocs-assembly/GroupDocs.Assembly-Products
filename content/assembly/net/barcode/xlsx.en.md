



---
############################# Static ############################
layout: "format"
date:  2024-12-02T19:05:17
draft: false
lang: en
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generate barcodes in XLSX Documents via C#"
head_description: "GroupDocs.Assembly for .NET API allows developers to dynamically generate & insert Barcode images to documents & Email messages with ease."

############################# Header ############################
title: "Insert generated Barcodes in XLSX Documents with our .NET API " 
description: "GroupDocs.Assembly for .NET provides complete support for dynamic Barcode image creation, editing and addition inside XLSX documents using C# API."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET overview"
    link: "/assembly/net/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) is designed in order to generate documents and reports by adding various data from wide range of data sources. Populate with textual or numeric data objects like charts, tables, lists. Insert images or barcodes generated on the fly. Use sophisticated mark-up to insert data in the right place of a document. Over 50 document formats like PDF, MS Office, emails, etc. are supported.

############################# Steps ############################
steps:
    enable: true
    title: "How to add generated barcode to XLSX document"
    content: |
      [GroupDocs.Assembly](/assembly/net/) allows to insert barcodes to many templates in popular formats like XLSX. More than 60 barcode types are supported. One and two-dimensional barcodes are ready for processing.
      
      1. Provide XLSX template with barcode markup.
      2. Get data from the any supported data source.
      3. Set up some additional properties like barcode dimensions or resolution.
      4. Save the template with barcode as a new document.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Sample document"
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
        // Use such template to insert a barcode to a document
        // <<barcode [barcode_expression] -barcode_type>>

        // Specify the template path
        string template = "barcode_template.docx";

        // Get data from the source
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Save result document with generated barcode
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Generate documents populating templates with data"
  description: "The GroupDocs.Assembly for .NET solution is engineered to provide service of documents generating across widely used formats. Add charts, lists, tables, hyper-links, images, barcodes using special markup and templates."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Assembly Features"
  features:
    # feature loop
    - title: "Construct reports based on business data"
      content: "Our API provides efficient algorithms to populate document of popular office formats with data from well-known data source formats like JSON, XML, CSV, etc."

    # feature loop
    - title: "Use visual object to represent your data"
      content: "GroupDocs.Assembly supports many native data objects such as lists, tables, charts in business documents. Text, hyper-links, images or on the spot generated barcodes are available."

    # feature loop
    - title: "Place data in any part of a document"
      content: "Use LINQ-based template syntax to insert data in a proper place. Data arrays may be placed with for-each syntax. It is possible to set up format (color, etc.) of data elements programmatically."

    # feature loop
    - title: "Wide range of supported formats"
      content: "We provide access to processing many popular formats like MS Office, Open Office, PDF, Html, various email formats. Some documents may be inserted into other ones."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to generate a barcode on the fly"
      content: |
        This example demonstrates how to embed a generated barcode to XLSX document.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Use such template to insert a barcode to a document
          // <<barcode [barcode_expression] -barcode_type>>

          // Specify the template path
          string template = "barcode_template.pptx";

          // Get data from the specific source
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Create data source object with only demanded data
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Instantiate DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Set up additional barcode properties
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // Save result document with barcode
          asm.AssembleDocument(template, "result.pptx", data);
          ```
        platform: "net"
        copy_title: "Copy"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/assembly/formats/assemblybarcode.xlsx"
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
  title: "Ready to get started?"
  description: "Try GroupDocs.Assembly features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Inspect our main features"
    exclude: "barcode"
    description: "We developed capable solution in order to help you with business documents"
    items: 
          
        # operation loop 1
        - name: "Create barcodes"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "Add generated on the fly barcodes to documents"

        # operation loop 2
        - name: "Represent data with diagrams"
          operation: "diagram"
          link: "/assembly/net/diagram/xlsx/"
          description: "Populate various types of diagrams with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "Insert one document content into another"

        # operation loop 4
        - name: "Use lists to show data"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "Create list with demanded data in a document"

        # operation loop 5
        - name: "Put data into table"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "Get data from any source and add to a table"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Generate reports of popular formats"
    exclude: "XLSX"
    description: ".NET supports reporting in more than 50 different formats. Effortlessly merge data and documents to have an excellent result."
    items: 
          
        # format loop 1
        - name: "Add barcode to PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add barcode to DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add barcode to PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Add barcode to XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---