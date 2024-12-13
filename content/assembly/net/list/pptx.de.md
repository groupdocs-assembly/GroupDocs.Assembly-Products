



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: de
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Erstellen Sie Listen in PPTX-Dokumenten mit C#"
head_description: "GroupDocs.Assembly for .NET API ermöglicht es Entwicklern, Daten gefüllte Listen dynamisch in Dokumente und Vorlagen einzufügen."

############################# Header ############################
title: "Fügen Sie datengestützte Listen zu PPTX-Dokumenten mit unserer .NET API hinzu" 
description: "GroupDocs.Assembly for .NET bietet leistungsstarke Werkzeuge, um Listen dynamisch in PPTX-Dokumenten zu erstellen und einzufügen."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlose Testversion herunterladen"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Überblick über GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ist darauf ausgelegt, die Erstellung von Dokumenten und Berichten zu optimieren, indem Daten nahtlos aus verschiedenen Quellen integriert werden. Füllen Sie Vorlagen mit Listen, Diagrammen, Tabellen, Barcodes oder Text und platzieren Sie Inhalte präzise mit fortgeschrittener Markup-Syntax. Mit Unterstützung für über 50 Formate - einschließlich PDFs, MS Office-Dateien und E-Mails - ist es ideal zur Automatisierung von Dokumenten-Workflows.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Hinzufügen einer datengestützten Liste zu einem PPTX-Dokument"
    content: |
      [GroupDocs.Assembly](/assembly/net/) erleichtert das Einfügen von datengestützten Listen in PPTX-Vorlagen. Erstellen und passen Sie Listen einfach an.
      
      1. Bereiten Sie eine PPTX-Vorlage mit Platzhaltern für die Liste vor.
      2. Setzen Sie den Pfad zur Vorlage.
      3. Holen Sie Daten aus unterstützten Quellen wie JSON oder XML ab.
      4. Speichern Sie das endgültige Dokument mit der eingebetteten Liste.
   
    code:
      platform: "net"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Beispieldokument"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "Klicken Sie zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Fügen Sie dieses Tag zu Ihrer Vorlage hinzu, um zu markieren, wo die Liste erscheinen wird.
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Geben Sie den Pfad zur Vorlagendatei an.
        string template = "list_template.pptx";

        // Rufen Sie die Daten aus Ihrer gewählten Quelle ab.
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Speichern Sie das Dokument mit der generierten Liste.
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erstellen Sie Dokumente, indem Sie Vorlagen mit strukturierten Daten füllen"
  description: "GroupDocs.Assembly for .NET vereinfacht den Aufbau von datengestützten Dokumenten. Fügen Sie Listen, Tabellen, Barcodes, Diagramme, Bilder und andere Elemente dynamisch mit fortschrittlichen Vorlagen hinzu."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly Funktionen"
  features:
    # feature loop
    - title: "Berichte aus Geschäftsdaten generieren"
      content: "Die API füllt Dokumente in gängigen Formaten mit Daten aus Quellen wie JSON, XML, CSV usw. mit Genauigkeit und Effizienz."

    # feature loop
    - title: "Verwenden Sie Listen und andere Elemente zur Datenpräsentation"
      content: "GroupDocs.Assembly ermöglicht es Ihnen, Listen, Tabellen und Diagramme zusammen mit Text, Barcodes, Hyperlinks und Bildern einzufügen, um gut strukturierte Dokumente zu erstellen."

    # feature loop
    - title: "Daten präzise einfügen, wo sie gebraucht werden"
      content: "Nutzen Sie die auf LINQ basierende Syntax, um Listen und andere Datenelemente genau zu positionieren. Verwenden Sie Schleifen, um Listen dynamisch zu füllen und benutzerdefinierte Formatierungen programmatisch anzuwenden."

    # feature loop
    - title: "Unterstützt mehrere Dokumentenformate"
      content: "Generieren und verwalten Sie Dokumente in verschiedenen Formaten wie MS Office, OpenOffice, PDF, HTML und E-Mail-Dateien. Integrieren Sie problemlos mehrere Dokumente in eines."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So generieren Sie eine Liste dynamisch"
      content: |
        Dieses Beispiel zeigt, wie Sie eine dynamisch generierte Liste in ein PPTX-Dokument einfügen.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Fügen Sie ein Platzhalter-Tag zu Ihrer Vorlage für die Liste hinzu.
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Geben Sie den Pfad zur Vorlagendatei an.
          string template = "numlist_template.pptx";

          // Rufen Sie die Daten ab, um die Liste zu füllen.
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Erstellen Sie ein Datenquellenobjekt mit den notwendigen Informationen.
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Initialisieren Sie DocumentAssembler.
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie das endgültige Dokument mit der generierten Liste.
          asm.AssembleDocument(template, "result.pptx", data);
          ```
        platform: "net"
        copy_title: "Kopieren"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "Klicken Sie zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Laden Sie das Ergebnis herunter"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.pptx"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit anzufangen?"
  description: "Erforschen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Herunterladen von Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Erfahren Sie mehr über Lizenzen"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Entdecken Sie wichtige Funktionen"
    exclude: "list"
    description: "Unsere Plattform wurde entwickelt, um die Erstellung und Integration von datengestütztem Dokumenteninhalt zu vereinfachen."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Erstellen Sie strukturierte Dokumente in gängigen Formaten"
    exclude: "PPTX"
    description: ".NET unterstützt über 50 Formate und ermöglicht es Ihnen, Daten und Vorlagen nahtlos zu kombinieren, um hochwertige, strukturierte Ergebnisse zu erzielen."
    items: 
          
        # format loop 1
        - name: "Erstellen Sie eine Liste in einem PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Erstellen Sie eine Liste in einem DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Erstellen Sie eine Liste in einem PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Erstellen Sie eine Liste in einem XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---