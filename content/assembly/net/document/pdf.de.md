



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: de
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Ein Dokument in ein anderes im PDF mit C# API einbetten"
head_description: "Fügen Sie mühelos PDF-Dokumente mit C# zusammen. Mit GroupDocs.Assembly kombinieren Sie Dateien nahtlos in nur wenigen Schritten."

############################# Header ############################
title: "Dokumente im PDF-Format kombinieren" 
description: "Mit GroupDocs.Assembly for .NET können Sie schnell ein PDF-Dokument in ein anderes einbetten. Diese API bietet leistungsstarke Werkzeuge für präzises Dokumenten-Merging."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ist ein leistungsstarkes Tool zur Dokumentenzusammenstellung und -manipulation. Es ermöglicht Benutzern, ein Dokument in ein anderes einzubetten, um nahtlos Inhalte zusammenzuführen. Mit Unterstützung für über 50 Formate—darunter PDFs, MS Office-Dateien und mehr—können Sie das endgültige Ergebnis organisieren, bearbeiten und anpassen, um Ihren Anforderungen gerecht zu werden.

############################# Steps ############################
steps:
    enable: true
    title: "Wie man ein Dokument in eine PDF-Datei einfügt"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ermöglicht es, ein Dokument mühelos in eine andere PDF-Datei einzubetten. Inhalte zusammenführen und anpassen.
      
      1. Gestalten Sie eine Vorlage mit spezifischen Platzhaltern für den einzubettenden Inhalt (PDF-Vorlagen werden nicht unterstützt).
      2. Definieren Sie den Dateipfad für die Vorlage.
      3. Geben Sie den Dateipfad des einzubettenden Dokuments an.
      4. Exportieren Sie die fertige Datei mit dem integrierten Inhalt als PDF-Dokument.
   
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
        // Fügen Sie dieses Tag zu Ihrem Template hinzu, um den Einfügepunkt zu markieren
        // <<doc [doc_expression]>>

        // Geben Sie den Dateipfad für das Template an
        // Zurzeit können keine PDF-Vorlagen verwendet werden.
        string template = "doc_template.docx";

        // Geben Sie den Pfad des einzubettenden Dokuments an
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Speichern Sie das zusammengeführte Dokument
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimieren Sie das Dokumenten-Merging mit fortschrittlichen Werkzeugen"
  description: "Die GroupDocs.Assembly for .NET-Bibliothek vereinfacht das Einbetten eines Dokuments in ein anderes, unterstützt verschiedene Dateiformate und bietet Anpassungen für eine nahtlose Integration."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte aus Ihren Geschäftsdaten generieren"
      content: "Automatisches Befüllen von Dokumenten mit Daten aus JSON, XML, CSV oder anderen Quellen, um genaue und effiziente Arbeitsabläufe sicherzustellen."

    # feature loop
    - title: "Dokumente mit visuellen Elementen anreichern"
      content: "GroupDocs.Assembly ermöglicht es Ihnen, Tabellen, Diagramme und Listen sowie Text, Links, Bilder und dynamisch generierte Barcodes einzufügen."

    # feature loop
    - title: "Daten präzise platzieren und formatieren"
      content: "LINQ-basierte Templates geben Ihnen die Kontrolle über die Platzierung der Daten, ermöglichen die Handhabung von Schleifen für Arrays und erlauben Stile wie Farbänderungen."

    # feature loop
    - title: "Funktioniert mit mehreren Dateiformaten"
      content: "Nahtloses Einbetten von Dokumenten in andere Formate wie MS Office, PDFs, HTML, OpenOffice und mehr."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Wie man ein Bild programmgesteuert in ein Dokument einfügt"
      content: |
        Dieses Beispiel zeigt, wie man ein Bild in ein PDF-Dokument mit GroupDocs.Assembly einfügt.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Fügen Sie ein Platzhalter-Tag in Ihr Template ein
          // <<image [expression]>>

          // Geben Sie den Dateipfad für das Template an
          // Zurzeit können keine PDF-Vorlagen verwendet werden.
          string template = "template.docx";

          // Setzen Sie den Pfad zur Bilddatei
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Initialisieren Sie eine Instanz von DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie das Dokument mit dem eingebetteten Bild
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "Entdecken Sie unsere leistungsstarken Werkzeuge"
    exclude: "document"
    description: "Erforschen Sie die Funktionen, die GroupDocs.Assembly für das Einbetten und Zusammenführen von Dokumenten mit Präzision bietet."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Dokumente in verschiedenen Formaten zusammenführen"
    exclude: "PDF"
    description: "Mit der .NET API können Sie Dokumente in über 50 unterstützten Formaten kombinieren. Mühelos Dateien oder Abschnitte in Ihre Enddokumente einbetten."
    items: 
          
        # format loop 1
        - name: "Binden Sie ein Dokument in ein PDF ein"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Binden Sie ein Dokument in ein DOCX ein"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Binden Sie ein Dokument in ein PPTX ein"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Binden Sie ein Dokument in ein XLSX ein"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---