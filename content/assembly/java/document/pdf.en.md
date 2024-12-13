



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: en
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Insert one document into another in PDF using Java"
head_description: "Combine PDF files easily with Java. GroupDocs.Assembly simplifies the process of merging documents in just a few lines of code."

############################# Header ############################
title: "Embed content into PDF files effortlessly" 
description: "Use GroupDocs.Assembly for Java to seamlessly insert one PDF document into another. Get precise results with flexible and reliable tools."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get it for Free"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) is a versatile solution for handling documents. It enables you to integrate one document into another with ease, supporting over 50 formats such as PDFs and MS Office files. Tailor your output by merging, editing, and organizing content exactly how you want.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to insert a document into a PDF file"
    content: |
      [GroupDocs.Assembly](/assembly/java/) makes embedding one PDF document into another simple and customizable.
      
      1. Create a template with placeholders for the embedded content (PDF templates are not supported).
      2. Specify the file path for the template.
      3. Provide the file path for the document to embed.
      4. Save the final file with the merged content as a PDF.
   
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
        // Use this tag in your template to mark the spot for the embedded document
        // <<doc [doc_expression]>>

        // Set the file path for the main template
        // PDF templates are not supported at the moment.
        String template = "doc_template.docx";

        // Provide the path to the document you want to insert
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Save the final file with the embedded content
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Advanced tools to simplify document integration"
  description: "With GroupDocs.Assembly for Java, embedding documents is straightforward and customizable, no matter the file type. Achieve clean and consistent results across your projects."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Highlights of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Create reports using business data"
      content: "Fill documents with data from sources like JSON, XML, or CSV quickly and reliably, streamlining your workflows."

    # feature loop
    - title: "Enhance documents with visual content"
      content: "GroupDocs.Assembly lets you insert tables, charts, and lists alongside text, hyperlinks, images, and even dynamic barcodes."

    # feature loop
    - title: "Place data exactly where it belongs"
      content: "LINQ templates help position your data with precision, handle repeating elements like arrays, and apply custom styles effortlessly."

    # feature loop
    - title: "Compatible with diverse file formats"
      content: "Merge documents across various formats, including PDFs, HTML, MS Office files, and OpenOffice, ensuring flexibility for your projects."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to programmatically insert an image into a document"
      content: |
        This example shows how to embed an image into a PDF file using GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Add a placeholder tag in the template file
          // <<image [expression]>>

          // Define the path to the template
          // PDF templates are not supported at the moment.
          String template = "template.docx";

          // Specify the path to the image
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Initialize the DocumentAssembler instance
          DocumentAssembler asm = new DocumentAssembler();

          // Save the file with the embedded image
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "Key capabilities at a glance"
    exclude: "document"
    description: "Discover the extensive features GroupDocs.Assembly offers to make embedding and combining documents efficient and hassle-free."
    items: 
          
        # operation loop 1
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "Dynamically create and add barcodes to documents"

        # operation loop 2
        - name: "Visualize data with diagrams"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "Fill various diagram types with data"

        # operation loop 3
        - name: "Merge documents"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "Combine the content of one document into another"

        # operation loop 4
        - name: "Show data with lists"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "Generate lists in documents using specific data"

        # operation loop 5
        - name: "Organize data in tables"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "Retrieve data from any source and populate tables"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Merge across different document types"
    exclude: "PDF"
    description: "With Java, you can embed and combine content across more than 50 file formats. Add files seamlessly to create professional results."
    items: 
          
        # format loop 1
        - name: "Embed a document in a PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Embed a document in a DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Embed a document in a PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Embed a document in an XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---