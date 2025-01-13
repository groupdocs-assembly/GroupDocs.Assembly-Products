



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:16
draft: false
lang: en
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: ""
head_description: ""

############################# Header ############################
title: "" 
description: ""
subtitle: "" 

header_actions:
  enable: true
  items:
    #  loop
    - title: ""
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: ""
    link: "/assembly/nodejs-java/"
    link_title: "Learn more"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {steps.content.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {steps.content.step_4}
   
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
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```java {style=abap}
        // {examples.comment_1}
        // <<barcode [barcode_expression] -barcode_type>>

        // {examples.comment_2}
        String template = "barcode_template.xlsx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "{more_features.image_description}"
  features:
    # feature loop
    - title: "{more_features.feature_1.title}"
      content: "{more_features.feature_1.content}"

    # feature loop
    - title: "{more_features.feature_2.title}"
      content: "{more_features.feature_2.content}"

    # feature loop
    - title: "{more_features.feature_3.title}"
      content: "{more_features.feature_3.content}"

    # feature loop
    - title: "{more_features.feature_4.title}"
      content: "{more_features.feature_4.content}"
      
  code_samples_ext:
    # code sample ext loop
    - title: "{code_1.title}"
      content: |
        {code_1.content}
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // {code_1.comment_1}
          // <<barcode [barcode_expression] -barcode_type>>

          // {code_1.comment_2}
          String template = "barcode_template.xlsx";

          // {code_1.comment_3}
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // {code_1.comment_5}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_6}
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // {code_1.comment_7}
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: ""
    exclude: "barcode"
    description: ""
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
    title: ""
    exclude: "XLSX"
    description: ""
    items: 
          
        # format loop 1
        - name: "Add a barcode to a PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add a barcode to a DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add a barcode to a PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Add a barcode to an XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---