



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: en
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Embed one document into another in PPTX with C# API"
head_description: "Easily merge PPTX documents using C#. With GroupDocs.Assembly, combine files seamlessly in just a few steps."

############################# Header ############################
title: "Combine documents in PPTX format" 
description: "With GroupDocs.Assembly for .NET, you can quickly embed one PPTX document into another. This API provides robust tools for precise document merging."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) is a powerful tool for document composition and manipulation. It allows users to embed one document into another, enabling seamless merging of content. With support for over 50 formats—including PDFs, MS Office files, and more—you can organize, edit, and customize the final output to meet your requirements.

############################# Steps ############################
steps:
    enable: true
    title: "How to merge a document into a PPTX file"
    content: |
      [GroupDocs.Assembly](/assembly/net/) allows you to embed one document into another PPTX file effortlessly. Merge and customize content with ease.
      
      1. Design a PPTX template with placeholders for the embedded document.
      2. Define the file path for the template.
      3. Specify the file path of the document to embed.
      4. Save the final file with the embedded content.
   
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
        // Add this tag to your template to mark the insertion point
        // <<doc [doc_expression]>>

        // Specify the file path for the template
        string template = "doc_template.pptx";

        // Provide the path of the document to be embedded
        DataSourceInfo data 
            = new DataSourceInfo("insert.pptx", "doc_expression");

        // Save the merged document
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Streamline document merging with advanced tools"
  description: "The GroupDocs.Assembly for .NET library simplifies embedding one document into another, supporting various file formats and offering customization for seamless integration."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Generate reports from your business data"
      content: "Automatically populate documents with data from JSON, XML, CSV, or other sources, ensuring accurate and efficient workflows."

    # feature loop
    - title: "Enrich documents with visual elements"
      content: "GroupDocs.Assembly allows you to include tables, charts, and lists, as well as text, links, images, and dynamically generated barcodes."

    # feature loop
    - title: "Precisely place and format data"
      content: "LINQ-based templates give you control over data placement, let you handle loops for arrays, and allow styling such as color customization."

    # feature loop
    - title: "Works with multiple file formats"
      content: "Easily embed documents into one another across formats like MS Office, PDFs, HTML, OpenOffice, and more."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to embed an image into a document programmatically"
      content: |
        This example demonstrates how to insert an image into a PPTX document using GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Add a placeholder tag in your template
          // <<image [expression]>>

          // Specify the file path for the template
          string template = "template.pptx";

          // Set the path to the image file
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Initialize an instance of DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Save the document with the embedded image
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
          - title: "Download the result"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Discover our powerful tools"
    exclude: "document"
    description: "Explore the features GroupDocs.Assembly offers for embedding and merging documents with precision."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Merge documents in various formats"
    exclude: "PPTX"
    description: "With .NET API, you can combine documents across more than 50 supported formats. Effortlessly embed files or sections into your final documents."
    items: 
          
        # format loop 1
        - name: "Embed a document in a PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Embed a document in a DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Embed a document in a PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Embed a document in an XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---