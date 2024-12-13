



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: en
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generate lists in DOCX documents with C#"
head_description: "GroupDocs.Assembly for .NET API enables developers to dynamically create and embed data-filled lists into documents and templates with ease."

############################# Header ############################
title: "Add data-driven lists to DOCX documents using our .NET API" 
description: "GroupDocs.Assembly for .NET offers powerful tools to dynamically generate and embed lists in DOCX documents."
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
    title: "Overview of GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) is designed to streamline the creation of documents and reports by seamlessly integrating data from various sources. Populate templates with lists, charts, tables, barcodes, or text, and place content precisely using advanced markup. With support for over 50 formats—including PDFs, MS Office files, and emails—it's ideal for automating document workflows.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to add a data-filled list to a DOCX document"
    content: |
      [GroupDocs.Assembly](/assembly/net/) makes it simple to insert data-driven lists into DOCX templates. Create and customize lists with ease.
      
      1. Prepare a DOCX template with placeholders for the list.
      2. Set path to the template.
      3. Retrieve data from supported sources like JSON or XML.
      4. Save the final document with the embedded list.
   
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
        // Add this tag to your template to mark where the list will appear
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Specify the path to the template file
        string template = "list_template.docx";

        // Retrieve data from your chosen source
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Save the document with the generated list
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Create documents by filling templates with structured data"
  description: "GroupDocs.Assembly for .NET simplifies building data-driven documents. Add lists, tables, barcodes, charts, images, and other elements dynamically with advanced templates."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly Features"
  features:
    # feature loop
    - title: "Generate reports from business data"
      content: "The API populates documents in popular formats using data from sources like JSON, XML, CSV, etc. with accuracy and efficiency."

    # feature loop
    - title: "Use lists and other elements to present data"
      content: "GroupDocs.Assembly enables you to embed lists, tables, and charts along with text, barcodes, hyperlinks, and images to create well-structured documents."

    # feature loop
    - title: "Insert data precisely where needed"
      content: "Leverage LINQ-based syntax to position lists and other data elements with precision. Use loops to populate lists dynamically and apply custom formatting programmatically."

    # feature loop
    - title: "Supports multiple document formats"
      content: "Generate and manage documents in various formats such as MS Office, OpenOffice, PDF, HTML, and email files. Easily integrate multiple documents into one."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to generate a list dynamically"
      content: |
        This example demonstrates how to embed a dynamically generated list into a DOCX document.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Add a placeholder tag to your template for the list
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Specify the path to the template file
          string template = "numlist_template.docx";

          // Retrieve the data to populate the list
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Create a data source object with the necessary information
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Initialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Save the final document with the generated list
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "Explore key capabilities"
    exclude: "list"
    description: "Our platform is built to simplify the creation and integration of data-driven document content."
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
    title: "Create structured documents in popular formats"
    exclude: "DOCX"
    description: ".NET supports over 50 formats, allowing you to seamlessly merge data and templates to produce polished, structured results."
    items: 
          
        # format loop 1
        - name: "Create a list in a PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Create a list in a DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Create a list in a PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Create a list in an XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---