



---
############################# Static ############################
layout: "format"
date:  2024-12-05T13:21:29
draft: false
lang: en
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Generate charts in PDF documents using Java"
head_description: "The GroupDocs.Assembly for Java API allows developers to create and insert dynamic charts or graphs into documents seamlessly, powered by live data."

############################# Header ############################
title: "Add charts to PDF documents with Java API" 
description: "GroupDocs.Assembly for Java simplifies the process of embedding charts into PDF documents by utilizing real-time data."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get Started for Free"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction to GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) is a versatile solution for automating the creation of documents and reports. It enables you to add charts, tables, lists, barcodes, and images directly into your files, with advanced tools for precise formatting and data integration. The platform supports over 50 formats, including PDF, Microsoft Office files, and emails.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to embed a chart into a PDF document"
    content: |
      [GroupDocs.Assembly](/assembly/java/) simplifies the process of inserting charts into PDF templates. Choose from a variety of chart styles, including bar, pie, and line charts.
      
      1. Create a PDF template with placeholders for the chart.
      2. Load your data from a compatible source.
      3. Set the chart options, such as type, labels, and colors.
      4. Save the document with the chart included.
   
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
        // Add this tag to your template to include a chart
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Provide the file path to your template
        String template = "chart_template.pdf";

        // Extract the necessary data from your source
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Save the final document with the embedded chart
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Effortlessly embed dynamic charts in your documents"
  description: "GroupDocs.Assembly for Java provides an easy way to build data-rich documents in popular formats. Use templates to insert charts, tables, barcodes, lists, links, and images with dynamic updates from your data."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Easily turn data into charts"
      content: "Use the API to transform data from JSON, XML, CSV, or other sources into clean, professional charts for your documents."

    # feature loop
    - title: "Create visually impactful content"
      content: "GroupDocs.Assembly supports various visual formats, including bar graphs, pie charts, and line graphs, which can be combined with tables, barcodes, images, and more for enhanced reports."

    # feature loop
    - title: "Customizable chart placement and styling"
      content: "With LINQ-based syntax, you can dynamically generate and position charts in the document, while easily adjusting styles, colors, and layouts to meet your design needs."

    # feature loop
    - title: "Supports multiple document formats"
      content: "Generate documents in formats like MS Office, PDF, OpenOffice, and HTML. The charts integrate smoothly into any supported format for professional results."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Programmatically generate and embed charts"
      content: |
        This example demonstrates how to create and embed a chart into a PDF document programmatically.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Prepare a template with a placeholder for the chart
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Specify the file path to the template
          String template = "table_template.pdf";

          // Load data from your chosen source
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Create a data object with the relevant information
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configure the chart's type and appearance
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Initialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Save the completed document with the chart embedded
          asm.AssembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "Explore powerful capabilities"
    exclude: "chart"
    description: "This platform simplifies the process of designing data-focused, visually appealing documents tailored to your needs."
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
    title: "Generate comprehensive reports in diverse formats"
    exclude: "PDF"
    description: "Java lets you create documents with integrated charts across over 50 file formats, ensuring seamless merging of templates and data."
    items: 
          
        # format loop 1
        - name: "Charts in PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Charts in DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Charts in PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Charts in XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---