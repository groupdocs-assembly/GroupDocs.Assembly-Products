---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "assembly/java/hyperlink/xlsx"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Add Hyperlinks to Office XLSX Documents & Reports via Java API"
head_description: "GroupDocs.Assembl for Java supports dynamic insertion of hyperlinks to office & emails documents such as PDF DOCX, RTF, XLSX, PPTX, EML, MSG & more inside Java apps."

############################# Header ############################
title: "Add Hyperlinks to Office Documents & Emails via Java API"
description: "GroupDocs.Assembly Java API allows software professionals to programmatically  add hyperlinks to email messages & Office Documents like PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, MSG & more."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Use Java API to Add Hyperlinks to Office & Emails Documents?"
    content: |
       A hyperlink is a word, phrase, or image that you can click on to jump to a new document or a new section within the current document. Hyperlinks are the backbone worldwide web and are used for many necessary functions on the World Wide Web. GroupDocs.Assembly for Java is a document automation and reports generation API that helps software developers to dynamically insert hyperlinks inside their documents or reports ease. The API is very stable and fully supports several advanced features related to hyperlinks management, such as add hyperlinks to a document page, links addition to a presentation slide, adding hyperlinks to spreadsheet cells, modifying hyperlinks content, dynamically inserting links from bookmarks, delete unwanted links,  show text instead of hyperlink, and many more. Some of very common documents types like PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations etc. are fully supported. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Insert Hyperlinks to Word Processing Documents via Java"
      content_left: |
       GroupDocs.Assembly Java API fully supports the insertion and editing of hyperlinks inside various commonly used documents formats. The below Java code example shows how to insert hyperlinks inside a Microsoft Word document.

      title_right: "Insert Hyperlinks in XLSX Document via Java"
      content_right: |
        * Setting up source and destination documents
        * Set Uri Expression as well as  display text Expression
        * Create an instance of [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) class 
        * Call [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) method to assemble document. It supports
          * Stream to read a template document.
          * Stream to write the resultant document.
          * Additional options for document loading and saving.
          * Information on data source objects.

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "Add Hyperlinks in Spreadsheets via Java"
      content_left: |
       GroupDocs.Assembly Java API allows computer programmers to insert and modify hyperlinks inside their Spreadsheet documents with ease. They can easily access, edit its location or replace it with a new one. The following Java code demonstrates how easily programmers can add hyperlinks inside their Spreadsheets.

      title_right: "How to Insert Hyperlinks to XLSX File"
      content_right: |
        * Setting up source and destination Spreadsheet files
        * Set Uri Expression as well as  display text Expression
        * Create an instance of [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) class 
        * Call [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) method to assemble document. It supports
          * Stream to read a template document.
          * Stream to write the resultant document.
          * Additional options for document loading and saving.
          * Information on data source objects. 

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "Insert Hyperlinks to PowerPoint Presentation via Java"
      content_left: |
       GroupDocs.Assembly Java API makes it easy for programmers to handle their documents management related tasks. Here is a Java code example that shows how easily software programmers can access their PowerPoint Presentation documents and add hyperlinks inside it.

      title_right: "How to Insert Hyperlinks in Presentations"
      content_right: |
        * Setting up source and destination presentation files
        * Set Uri and  display text Expressions
        * Create an instance of [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) class 
        * Call [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) method to assemble document. It supports
          * Stream to read a template document.
          * Stream to write the resultant document.
          * Additional options for document loading and saving.
          * Information on data source objects.

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "Use Java API to Add Hyperlinks in Emails"
      content_left: |
       GroupDocs.Assembly for Java makes it easy for software developers to add hyperlinks to their email messages with just a couple of lines of Java code. The following example demonstrates how easily can developers insert hyperlinks inside their email documents and send to other users inside their own Java apps. 

      title_right: "how to Add Hyperlinks to Emails"
      content_right: |
        * Setting up source and destination Spreadsheet files
        * Set Uri and  display text Expressions
        * Create an instance of [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) class 
        * Call [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) method to assemble document. It supports
          * Stream to read a template document.
          * Stream to write the resultant document.
          * Additional options for document loading and saving.
          * Information on data source objects. 

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

    - title_left: "System Requirements"
      content_left: |
        GroupDocs.Assembly Java APIs are supported on all major platforms and operating systems. It can generate documents in Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice & 50+ other formats. For complete system requirements guide, please visit [system requirements](https://docs.groupdocs.com/assembly/java/system-requirements/) Before executing the code below, please make sure that you have the following prerequisites installled on your system:
        * Operating Systems: Microsoft Windows, Linux, MacOS
        * Java Versions Support: J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above
        * Get the latest version of GroupDocs.Assembly Java APIs from [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/)
        
      title_right: "Why Use GroupDocs.Assembly"
      content_right: |
        * Create custom documents from templates.
        * Dynamically attach email attachments.
        * No additional software is required to create and automate documents.
        * Generates an output document based on the data source.
        * Dynamically insert out document content in report
        * Apply formula during spreadsheet assembly.
        * Provides support for Multiple data formats
        * Sequential data operations support. 

demos:
    enable: true
        

about_formats:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---