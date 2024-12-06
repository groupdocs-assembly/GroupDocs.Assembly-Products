



---
############################# Static ############################
layout: "format"
date:  2024-12-06T10:45:23
draft: false
lang: en
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Create lists in XLSX documents using Java"
head_description: "Easily design and embed dynamic lists into your XLSX templates with GroupDocs.Assembly for Java API."

############################# Header ############################
title: "Add dynamic lists to XLSX files with our Java API" 
description: "GroupDocs.Assembly for Java provides flexible tools to generate and insert data-rich lists directly into XLSX documents."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try it for Free"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) makes it easy to design professional documents by pulling data from multiple sources. Use it to create lists, tables, charts, or text, and place these elements exactly where needed using advanced template features. With support for over 50 formats, including PDFs, MS Office files, and email documents, it helps automate and streamline your workflow.

############################# Steps ############################
steps:
    enable: true
    title: "How to add a data-driven list to a XLSX document"
    content: |
      [GroupDocs.Assembly](/assembly/java/) lets you quickly insert data-rich lists into XLSX templates. Customize and organize content effortlessly.
      
      1. Create a XLSX template and mark placeholder spots for the list.
      2. Set the file path to the template.
      3. Fetch data from supported formats like JSON or XML.
      4. Save the final document with the list added.
   
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
        // Include this tag in your template where the list should appear
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Define the file path of the template
        String template = "list_template.xlsx";

        // Pull data from your chosen source
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Save the document with the embedded list
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Generate documents from templates with data integration"
  description: "GroupDocs.Assembly for Java simplifies adding dynamic lists, tables, charts, and other components into document templates."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Build reports with data from various sources"
      content: "Use data from formats like JSON, XML, and CSV to populate lists and other components efficiently."

    # feature loop
    - title: "Add lists and other data elements seamlessly"
      content: "GroupDocs.Assembly enables embedding of lists, charts, tables, and more, alongside text, images, and links to create polished documents."

    # feature loop
    - title: "Precisely control where data appears"
      content: "LINQ-based templates allow you to define exact locations for your lists and data. Use loops to create detailed lists automatically and apply custom formatting."

    # feature loop
    - title: "Supports various document formats"
      content: "Create or edit files in formats such as MS Office, PDF, OpenOffice, HTML, and email. Merge content from multiple documents as needed."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to create a list programmatically"
      content: |
        This example shows how to add a list dynamically into a XLSX file using GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Add a placeholder tag in your template for the list
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Provide the file path to your template
          String template = "numlist_template.xlsx";

          // Pull the required data to populate the list
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Prepare the data source with the necessary details
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Initialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Save the output document with the completed list
          asm.AssembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "Discover what GroupDocs.Assembly can do"
    exclude: "list"
    description: "Easily design and generate content-rich documents with advanced data integration tools."
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
    title: "Produce documents in various formats"
    exclude: "XLSX"
    description: "Java supports over 50 formats, allowing you to create structured documents by combining data and templates."
    items: 
          
        # format loop 1
        - name: "Create a list in a PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Create a list in a DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Create a list in a PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Create a list in an XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---