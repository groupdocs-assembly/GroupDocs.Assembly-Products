---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API for Document Automation, Assembly & Reports Generation"
head_description: "C# .NET Document automation, assembly & reports generation API. Create PDF Word Excel PPTX HTML & email documents from custom templates."

############################# Header ############################
title: ".NET Document Automation & Reporting API"
description: "‎Generate Reports in .NET Applications by Defining Templates, and Megring the Data."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
        product: "GroupDocs.Assembly"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for .NET API helps you build powerful document automation and report generation applications with capabilities to generate reports from customized templates in C#, ASP.NET and other .NET related applications. With just a few lines of code, the .NET reporting library intelligently assembles the given data from the defined document template and generates beautiful reports in the preferred output format by fetching data from various data sources (databases, XML, JSON, ODATA, CSV, Custom .NET objects).  

      It supports LINQ-based template syntax, and users can easily generate output documents in all commonly used business file formats such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations and slides. Formatting properties for template elements are also configurable by manipulating text, HTML & conditional blocks, images, charts, barcodes, hyperlinks, pivot tables etc.  

      GroupDocs.Assembly for .NET can be used to develop applications in any development environment that targets .NET platform. It is compatible with all .NET based languages and supports popular operating systems (Windows, Linux, MacOS) where Mono or .NET frameworks (including .NET Core) can be installed.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Assembly for .NET:
      
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
          Supported [document file formats](https://docs.groupdocs.com/assembly/net/supported-document-formats/) for .NET document generation API are listed below.

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
          GroupDocs.Assembly for .NET supports following Operating Systems, Frameworks & Package Managers:‎
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Package Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Development Environments"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Assembly for .NET Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Works with Multiple Data Formats"

      # feature loop
      - icon: "fas fa-eye"
        content: "Capable to Manipulate Data using Formulae & Sequential Data Operations"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Format Strings in Template Syntax to be Upper, Lower, Capital, FirstCap"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Perform Ordinal, Cardinal, Alphabetic Numeric Formatting in Template Syntax"

      # feature loop
      - icon: "fas fa-code"
        content: "Define Variables in Template Documents & Support Text Comments within Template Syntax Tags"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Dynamically Insert Contents of Outer Documents to your Reports"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Dynamically Generate Barcode Image in Reports & Set Background Color for HTML Documents"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Dynamically Assign Attributes to Email Message Body & Insert Hyperlinks in Reports‎"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Dynamically Build Email Message Attachments"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Support for Analogue of Microsoft Word NEXT Field"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Update Fields while Assembling Word Processing Documents"

      # feature loop
      - icon: "fas fa-columns"
        content: "Calculate Formula while Assembling Spreadsheet Documents"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Format Numeric, Text, Image, Chart, Date-Time Elements of Template"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Loading & Saving Assembled POT & OTP Presentation Document Formats"

      # feature loop
      - icon: "fas fa-print"
        content: "Use LINQ-Based Syntax for Template & Perform Conditional Text Formatting of Template Elements"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Change File Format of the Assembled Document using File Extension or Explicit Specs"

      # feature loop
      - icon: "fas fa-lock"
        content: "Ordered List Supported for Markdown - Save Newly Assembled Emails & Word Documents to Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Supports Reports of Numerous Types, e.g., Charts, Lists, Tables, Images and more"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Inline Template Syntax Errors in Generated Documents instead of Exception Throwing"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Load Template Documents from HTML with Resources and Save Assembled Word, Excel, PowerPoint & Emails to HTML with Resources"

      # feature loop
      - icon: "fas fa-heading"
        content: "Dynamically Add Restart List Numbering in Word Document Formats and Email with HTML & RTF Bodies"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Dynamically Insert images & documents from Base64-encoded bytes and adjust checkbox value settings of Word documents"

      # feature loop
      - icon: "fas fa-cube"
        content: "Stretch Image in Textbox of Word, Excel, Presentations & Emails while Preserving the Image Ratio"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Dynamically Add Links and Bookmarks to Document Formats and Name the Cell Ranges of Excel Spreadsheets"

    more_feature:
      # more_feature_loop
      - title: "Support for Template Elements"
        content: |
          GroupDocs.Assembly for .NET API gives you control to work with numerous template elements. You can work with formatted text blocks, HTML blocks, Images, Charts, Hyperlinks and Bar Codes (through Barcode Fonts). Repeated blocks & Conditional blocks are also supported including list items and table rows. You can also dynamically merge table cells containing the same text based on template expressions for spreadsheets, presentations, documents, and emails with HTML and RTF bodies.‎

      # more_feature_loop
      - title: "Working with List Reports"
        content: |
          Using GroupDocs.Assembly for .NET API, you can work with List Reports of following three types:  

          * Bulleted List
          * Numbered List
          * Colored Numbered List

      # more_feature_loop
      - title: "Working with Chart Reports"
        content: |
          GroupDocs.Assembly for .NET supports following type of Chart Reports:  

          * Bubble Chart, that displays three dimensions of data
          * Column Chart
          * Pie Chart
          * Scatter Chart
          * Series Chart (Colored)

      # more_feature_loop
      - title: "Working with Table Reports"
        content: |
          GroupDocs.Assembly for .NET supports following types of Table Reports:  

          * Master-Detail Table
          * Table with Highlighted Rows
          * Table with Alternate Content
          * Table with Filtering, Grouping, and Ordering  
          
          You can also use Data Bands in table rows.

      # more_feature_loop
      - title: "Easy Integration"
        content: |
          You can easily integrate GroupDocs.Assembly for .NET API with your .NET application using just a few lines of code. Following is an example code for generating report in open document format:

          ```cs
          //Instantiate DocumentAssembler class
          DocumentAssembler assembler = new DocumentAssembler();
          //Call AssembleDocument to generate report
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
          //(See DataLayer.GetCustomerData() method details at https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET)
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
        - img_alt: "GroupDocs.Assembly for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
