



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: en
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Add tables to XLSX documents using Java"
head_description: "With GroupDocs.Assembly for Java, developers can quickly integrate tables into documents and emails, pulling data from dynamic sources."

############################# Header ############################
title: "Easily populate tables in XLSX files with our Java API" 
description: "GroupDocs.Assembly for Java simplifies the process of filling tables in XLSX documents with data from various inputs."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get Your Free Trial"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) is a tool for generating documents and reports by automatically inserting data into pre-designed templates. You can effortlessly add tables, lists, charts, and images. Its advanced features allow you to precisely place content within your documents. Compatible with over 50 file types, including PDF, MS Office, and email formats.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to insert data into a XLSX table"
    content: |
      [GroupDocs.Assembly](/assembly/java/) helps you populate table templates for XLSX and other formats. Use dynamic data from your sources to create tables with ease.
      
      1. Set up a XLSX template with placeholders for table rows and columns.
      2. Pull data from any supported input source.
      3. Filter or preprocess the data to match your needs.
      4. Generate the final document with the completed table.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Example document"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Use these tags in a table row placeholder within your template
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Define the path to the template file
        String template = "table_template.xlsx";

        // Load data from your chosen source
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Save the output file with the table populated
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Create documents with data-filled tables"
  description: "GroupDocs.Assembly for Java makes it simple to automate table creation in your documents. It also supports adding elements like charts, lists, and images using templates."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Main Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Generate reports from multiple data formats"
      content: "The API works seamlessly with JSON, XML, CSV, and other formats to fill tables in your documents with organized data."

    # feature loop
    - title: "Present information visually"
      content: "GroupDocs.Assembly helps you build professional tables, lists, and charts, as well as insert links, text, and images, for a polished look."

    # feature loop
    - title: "Place table content with precision"
      content: "Use flexible LINQ-based syntax to add rows and columns dynamically. Customize appearance, such as font styles and colors, programmatically."

    # feature loop
    - title: "Compatible with multiple formats"
      content: "Work with MS Office, OpenOffice, PDF, HTML, and more. Merge tables into any supported file format effortlessly."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dynamically create a data-filled table"
      content: |
        This example shows how to populate a table in a XLSX document using dynamic input data.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Design a template with a placeholder for the table
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Set the template file location
          String template = "table_template.xlsx";

          // Load data from your preferred source
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Prepare a data object containing the necessary fields
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Create an instance of DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Save the document with the table populated
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Copy"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download the result"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.xlsx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Ready to begin?"
  description: "Explore GroupDocs.Assembly features for free or request a license"
  items:
    #  loop
    - title: "Download from Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Learn about licensing"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Key features at a glance"
    exclude: "table"
    description: "Our API simplifies creating professional documents by automating table population alongside other powerful components."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produce detailed tables in various formats"
    exclude: "XLSX"
    description: "With Java, you can populate templates with data and generate detailed reports in over 50 file types."
    items: 
          
        # format loop 1
        - name: "Add a table to a PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add a table to a DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add a table to a PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Add a table to an XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---