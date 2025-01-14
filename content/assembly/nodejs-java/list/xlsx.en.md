



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:16
draft: false
lang: en
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Create Dynamic Lists in XLSX with JavaScript"
head_description: "Easily design and insert lists into XLSX templates using the GroupDocs.Assembly for Node.js via Java API."

############################# Header ############################
title: "Embed Data-Driven Lists in XLSX Files with Node.js" 
description: "GroupDocs.Assembly for Node.js via Java offers powerful tools to add flexible, data-powered lists to XLSX documents."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get Started for Free"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) simplifies document creation by pulling data from various sources and embedding it into templates. Use it to build lists, tables, charts, and other elements, with precise placement and formatting options. Supporting over 50 formats, including PDF, MS Office, and emails, it helps automate your document generation process.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to Insert a List into a XLSX File"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) makes it easy to add detailed, data-driven lists to your XLSX templates.
      
      1. Create a XLSX template and define placeholders for the list.
      2. Provide the template's file path.
      3. Load data from supported sources like JSON or XML.
      4. Save the document with the generated list.
   
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
        // Place this tag in your template to mark where the list will go
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Set the file path for your template
        const template = "list_template.xlsx";

        // Fetch data from the source you want to use
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Save the file with the embedded list
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Easily Generate Documents with Integrated Data"
  description: "With GroupDocs.Assembly for Node.js via Java, you can embed lists, tables, charts, and other elements into templates, saving time and effort."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Highlights of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Generate Reports from Multiple Data Sources"
      content: "Import data from JSON, XML, CSV, or other formats to populate lists and other components efficiently."

    # feature loop
    - title: "Add Lists and Other Visual Elements"
      content: "GroupDocs.Assembly allows you to seamlessly embed lists, tables, charts, and more alongside text, images, and links for polished results."

    # feature loop
    - title: "Precisely Place and Style Data"
      content: "LINQ-based templates let you control exactly where lists and other data appear, use loops for repeated items, and customize styles to fit your needs."

    # feature loop
    - title: "Works Across Multiple Formats"
      content: "Create documents in formats like MS Office, PDF, OpenOffice, HTML, and emails. Merge content from various sources into a single file."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Programmatically Create a List in a Document"
      content: |
        This example demonstrates how to dynamically add a list to a XLSX document using GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Add a placeholder in your template for the list
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Specify the file path of the template
          const template = "numlist_template.xlsx";

          // Load data to populate the list
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Prepare the data source with required details
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Initialize the DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Save the final document with the list included
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "Explore the Features of GroupDocs.Assembly"
    exclude: "list"
    description: "Design and generate data-rich documents effortlessly using powerful integration tools."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Create Documents in Multiple Formats"
    exclude: "XLSX"
    description: "Node.js via Java supports over 50 file formats, making it easy to merge templates and data into professional results."
    items: 
          
        # format loop 1
        - name: "Create a list in a PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Create a list in a DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Create a list in a PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Create a list in an XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---