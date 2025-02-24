---
############################# Static ############################
layout: "family"
date:  2025-02-24T17:52:12
draft: false

product: "Assembly"
product_tag: "assembly"

lang: en

############################# Head ############################
head_title: ".NET, Java, Node.js APIs & Online Document Assembly Apps by GroupDocs"
head_description: "Get all-in-one Document Automation & Reporting Solution for .NET, Java and Node.js applications. Generate all common documents from custom templates and data."

############################# Header ############################
title: "Document Automation and Reporting Solution"
description:  |
  Easily create detailed reports using templates and data sources with our cross-platform apps and APIs.

  Generate reports in formats like Word, Excel, Presentations, and many more using templates with flexible markup.

  Populate charts, barcodes, tables, and other elements with data from sources like JSON, XML, CSV, etc.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choose your platform"
  title: "Platform independence"
  description: "GroupDocs.Assembly is compatible with the following operating systems and frameworks:"
  details_link_title: "Learn more"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Any other text editor
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Assembly key features"
  description: "This solution helps you create reports in popular document formats, automatically filled with your business data. Easily automate your document generation tasks."

  items:
    # items loop
    - icon: "additional"
      title: "Populate templates with data"
      content: "Fill reports using data from supported sources."

    # items loop
    - icon: "manipulate"
      title: "Flexible markup"
      content: "Add data to documents in a customizable way."

    # items loop
    - icon: "structure"
      title: "Native document features"
      content: "Display data using tables, charts, and barcodes."

    # items loop
    - icon: "merge"
      title: "All popular formats"
      content: "Supports all commonly used document formats."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Generate well-customized reports"
  description: "GroupDocs.Assembly code examples"
  items:
    # code sample loop
    - title: "Using Generated Barcodes"
      content: |
       GroupDocs.Assembly allows barcode markup in report templates. When creating a report, a barcode is generated based on the markup and provided data. Specify the path to the template containing the text, data objects, and markup. Also, specify the data source to fill the barcode with content.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Create an instance of the DocumentAssembler class
            DocumentAssembler assembler = new DocumentAssembler();

            //Specify the path to the template
            var tmp_path = "barcode_template.docx";

            //Specify the path for the result document
            var res_path = "result.docx";

            //Create an instance of the datasource
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Call AssembleDocument to generate the report
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Create an instance of the DocumentAssembler class
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Specify the path to the template
            String tmp_path = "barcode_template.docx";

            //Specify the path for the result document
            String res_path = "result.docx";

            //Create an instance of the datasource
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Call AssembleDocument to generate the report
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // Create an instance of the DocumentAssembler class
            const assembler = new assemblyLib.DocumentAssembler();
            
            //Specify the path to the template
            const tmp_path = "barcode_template.docx";

            //Specify the path for the result document
            const res_path = "result.docx";

            //Create an instance of the datasource
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // Call AssembleDocument to generate the report
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Supports 50+ file formats"
  description: "GroupDocs.Assembly works with nearly all popular file formats"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Our product statistics"
  description: "Explore product metrics to gain insights into our progress, impact, and growth."

  items:
    # items loop
    - number: "50+"
      title: "Supported Formats"
      content: "We support over 50 of the most widely used document formats."

    # items loop
    - number: "650k"
      title: "NuGet Downloads"
      content: "GroupDocs.Assembly for .NET is a popular library with more than 650,000 downloads on NuGet."

    # items loop
    - number: "18k"
      title: "Maven Downloads"
      content: "Java developers have downloaded GroupDocs.Assembly on Maven over 18,000 times."

    # items loop
    - number: "150+"
      title: "Happy Customers"
      content: "Our products are trusted by individual developers and leading companies worldwide to create innovative solutions."


############################# Customers ###############################
customers:
  enable: true
  title: "Our Happy Customers"
  description: "GroupDocs libraries are used by some of the most renowned and respected brands across the globe."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Ready to Get Started?"
  description: "Test GroupDocs.Assembly features for free on your platform."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Frequently Asked Questions"
  description: "Browse our Frequently Asked Questions."

  items:
    # items loop
    - question: "Does GroupDocs.Assembly require any external libraries for document composing?"
      answer: "No, GroupDocs.Assembly works independently and does not require third-party libraries like Adobe Acrobat or Microsoft Office."

    # items loop
    - question: "Can I test GroupDocs.Assembly features before purchasing?"
      answer: "Yes, you can! GroupDocs.Assembly offers a free trial. Install it and explore its features. The trial version adds 'trial badges' to your documents and only processes the first 3 pages. For the full experience, get a free 30-day temporary license to access all features. More details are available under [temporary license](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "What types of licenses are available?"
      answer: "Looking for a GroupDocs.Assembly license? We offer a variety of options to suit your needs. Choose based on your team size, deployment location (single office or remote), and whether you need to share the SDK/API with clients for distribution. Alternatively, choose a monthly usage license with metered plans—pay only for what you use. Find the best option for you under [pricing](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Assembly Low-Code APIs"
  description: "Generate documents using your application through our cloud-based REST API."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Use the cURL RESTful API to add data to Word, Excel, PowerPoint, and many other templates."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Enhance your .NET applications by generating reports through the Cloud SDK. Display business data in your custom format."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK offers different options for Java applications to generate various types of documents."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Assembly Web Apps"
  description: "GroupDocs.Assembly offers a free web application for generating documents. You can process more than 50 popular file formats directly in your browser, FOR FREE."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Generate reports in Excel, Word, PowerPoint, and many other file types directly from your web browser."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Create Microsoft Word documents from templates and data sources."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Upload a template and a data source to generate Excel reports for free."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---