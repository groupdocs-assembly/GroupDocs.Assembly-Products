---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Automation Assembly & Dynamic Reports Generator API"
head_description: "Java API for document automation, assembly & reporting. Create reports from custom templates. Assemble PDF Word Excel PPTX HTML from DB, JSON, OData & XML data sources."

############################# Header ############################
title: "Java API to Automate Documents & Reports"
description: "‎Build Document Automation Applications to Fetch Data; put it in Customizable Templates & Generate Dynamic Reports via Java API.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
        product: "GroupDocs.Assembly"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/assembly"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java API helps you rapidly develop document automation and reporting applications in Java to generate custom reports from templates without installing any external software. The report generation engine fetches data from the template document, assembles it and generates reports in the specified output format according to the defined syntax. It allows you to configure and insert formatting properties of template elements dynamically and supports various data sources (JSON, XML, OData, databases, CSV, spreadsheet as table of data, word processing table as table of data and databases) to retrieve data from.  

      The document assembly library recognizes multiple document formats and allows you to create templates in all supported file types such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations and text. It supports LINQ-based template syntax and users can also configure and insert formatting properties of template elements dynamically.  

      GroupDocs.Assembly for Java is easy to integrate with new or existing java applications. It is highly compatible with all Java versions and supports popular operating systems (Windows, Linux, MacOS) that are capable to run Java runtime.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Assembly for Java:

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Overview"
          content: |
            * Data Formulation
            * Data Formatting
            * Data Automation
            * Create Template
            * Template Element Formatting
            * Report Generation
      
      ## TAB TWO ##
      tab_two:
        description: |
          Supported [document file formats](https://docs.groupdocs.com/assembly/java/supported-document-formats/) for Java document generation API are listed below.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            # table loop
            - title: "Supported Data Sources"
              content: |
                * Database
                * XML
                * OData
                * JSON
                * CSV
                * Custom .NET Objects
                * Spreadsheet as Table of Data
                * Word Processing Table as Table of Data

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenOffice Document Formats**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **Markdown Documentation File**: MD
                * **Other**: TXT

            # table loop
            - title: "Inter-Format Assembly Support"
              content: |
                * Word Processing **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Spreadsheet **TO** Spreadsheet, HTML, PDF, XPS, TIFF, MHTML
                * Presentation **TO** Presentation, HTML, PDF, XPS, TIFF
                * Email **TO** Word Processing, Email, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML & TXT **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Assembly for Java supports following Operating Systems, Frameworks & Package ‎Managers:‎
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Assembly for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Adjust Image in Textbox of Word, Excel, Presentations & Emails while Preserving the Image Ratio"

      # feature loop
      - icon: "fas fa-eye"
        content: "Use Formulae & Perform Sequential Data Operations - Apply Formula during Spreadsheet Assembly"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Apply Upper, Lower, Capital, FirstCap Formatting to Strings in Template Syntax"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Template Syntax support Formatting of Ordinal, Cardinal, Alphabetic Numeric Nature"

      # feature loop
      - icon: "fas fa-code"
        content: "Support Template Documents with Custom Variables & Text Comments within Template Syntax Tags"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Dynamically Insert Out Document Content in Report"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Dynamically Configure Background Color of HTML Documents & Generate Barcode in Reports"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Dynamically Insert Hyperlinks in Reports & Apply Attributes to Email Message Body"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Dynamically Attach Email Attachments and Update Fields during Word Processing Document Assembly"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Support of NEXT Field Analogue of Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Dynamically Add Links and Bookmarks to Document Formats and Name the Cell Ranges of Excel Spreadsheets"

      # feature loop
      - icon: "fas fa-columns"
        content: "Loading & Saving Assembled POT & OTP Presentation Document Formats"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Template Formatting for Numeric, Text, Image, Date-Time, Chart Elements"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Dynamically Insert images & documents from Base64-encoded bytes"

      # feature loop
      - icon: "fas fa-print"
        content: "LINQ-Based Template Syntax"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Change Format of Assembled File using Explicit Specifications or File Extension"

      # feature loop
      - icon: "fas fa-lock"
        content: "Ordered List Supported for Markdown - Save Newly Assembled Emails & Word Documents to Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Generate Various Report Types, e.g., Charts, Image, Tables, Lists and more"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Inline Template Syntax Errors in Generated Documents instead of Exception Throwing"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Dynamically Restart A Numbered List in Word Documents as well as Emails with HTML & RTF Bodies"

      # feature loop
      - icon: "fas fa-heading"
        content: "Support of Tables, Autolinks, Inline Links and Images for Assembled Markdown Documents"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Dynamically Generate Barcodes (GS1-128 AI 8102 Coupon Extended and UPCA & GS1 Databar Coupon"

      # feature loop
      - icon: "fas fa-cube"
        content: "Load Template Documents from HTML with Resources and Save Assembled Word, Excel, PowerPoint & Emails to HTML with Resources"

    more_feature:
      # more_feature_loop
      - title: "Manipulate Template Elements"
        content: |
          Manipulate numerous template elements with GroupDocs.Assembly for Java API. The template elements that you can work with include, text blocks, Images, Hyperlinks, HTML blocks, Barcodes (via Barcode fonts), and Charts. You can also apply repeated blocks & conditional blocks for list items and table rows. Dynamic merging of table cells holding the same text, based on template expressions for documents, presentations, spreadsheets, and emails with HTML and RTF bodies.
      
      # more_feature_loop
      - title: "Manipulate List Reports"
        content: |
          Using GroupDocs.Assembly for Java API, supports following types of List Reports:  

          * Bulleted List
          * Numbered List
          * Colored Numbered List

      # more_feature_loop
      - title: "Manipulate Chart Reports"
        content: |
          GroupDocs.Assembly for Java supports following type of Chart Reports:

          * Bubble Chart, which displays three dimensions of data
          * Column Chart
          * Pie Chart
          * Scatter Chart
          * Series Chart (Colored)

      # more_feature_loop
      - title: "Manipulate Table Reports"
        content: |
          GroupDocs.Assembly for Java supports following types of Table Reports:  

          * Master-Detail Table
          * Table with Highlighted Rows
          * Table with Alternate Content
          * Table with Filtering, Grouping, and Ordering  

          You can also use Data Bands in table rows.

      # more_feature_loop
      - title: "Manipulate Chart Reports"
        content: |
          Integration of GroupDocs.Assembly for Java API with your Java application is like a breeze. What follows is an example block of code that generates report in OpenDocument format using Java:  

          ```java
          // Instantiate DocumentAssembler class
          DocumentAssembler assembler = new DocumentAssembler();
          //Call AssembleDocument to generate report
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          //(See new DataStorage() method details at https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java)
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Assembly offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---