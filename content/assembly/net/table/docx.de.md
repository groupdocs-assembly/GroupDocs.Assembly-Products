



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: de
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tabellen in DOCX-Dokumenten mit C# erstellen"
head_description: "Die GroupDocs.Assembly for .NET API ermöglicht es Entwicklern, Tabellen in Dokumenten und E-Mails mühelos mit Daten aus dynamischen Quellen hinzuzufügen und auszufüllen."

############################# Header ############################
title: "Daten Tabellen in DOCX-Dokumenten mit unserer .NET API generieren" 
description: "GroupDocs.Assembly for .NET ermöglicht das dynamische Befüllen von Tabellen in DOCX-Dokumenten mit Daten aus verschiedenen Quellen."
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
    title: "GroupDocs.Assembly for .NET Übersicht"
    link: "/assembly/net/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) wurde entwickelt, um Dokumente und Berichte durch das Befüllen von Vorlagen mit Daten aus mehreren Quellen zu erstellen. Fügen Sie mühelos strukturierte Daten in Tabellen, Listen und Diagramme ein oder betten Sie Bilder dynamisch ein. Eine ausgeklügelte Syntax gewährleistet eine präzise Datenplatzierung. Unterstützt über 50 Formate, darunter PDFs, MS Office-Dokumente und E-Mail-Dateien.

############################# Steps ############################
steps:
    enable: true
    title: "So befüllen Sie eine Tabelle in einem DOCX-Dokument"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ermöglicht es Ihnen, Tabellen in Vorlagen für Formate wie DOCX dynamisch zu befüllen. Fügen Sie Daten aus verschiedenen Quellen in Ihre Tabellen ein.
      
      1. Erstellen Sie eine DOCX-Vorlage mit Platzhaltern für die Tabelle.
      2. Daten aus einer beliebigen unterstützten Quelle abrufen.
      3. Filtern Sie die Daten, um nur die erforderlichen Informationen einzuschließen.
      4. Speichern Sie das Dokument mit der befüllten Tabelle.
   
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
        // Fügen Sie diese Tags in eine Tabellenzeile der Vorlage ein
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Legen Sie den Dateipfad für die Vorlage fest
        string template = "table_template.docx";

        // Daten aus einer unterstützten Quelle abrufen
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Speichern Sie das Dokument mit der mit Daten gefüllten Tabelle
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Dokumente mit dynamischen Tabellen generieren"
  description: "GroupDocs.Assembly for .NET vereinfacht die Dokumentenerstellung, indem die Tabellenbefüllung automatisiert und zusätzliche Elemente wie Diagramme, Listen und Bilder über Vorlagen und erweiterte Markup unterstützt werden."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte aus strukturierten Daten erstellen"
      content: "Die API verarbeitet Daten aus Quellen wie JSON, XML und CSV, um Tabellen in Office-Dokumenten effizient und genau zu befüllen."

    # feature loop
    - title: "Daten visuell darstellen"
      content: "GroupDocs.Assembly ermöglicht die Erstellung von Tabellen, Listen und Diagrammen sowie das Einbetten von Text, Links und Bildern für ein professionelles Dokumentendesign."

    # feature loop
    - title: "Tabellendaten präzise positionieren"
      content: "Verwenden Sie eine LINQ-basierte Syntax, um dynamisch Tabellenzeilen und -spalten hinzuzufügen. Passen Sie Stile, einschließlich Farben und Formatierung, programmatisch an."

    # feature loop
    - title: "Unterstützt eine breite Palette von Formaten"
      content: "Bearbeiten Sie mühelos gängige Dateiformate wie MS Office, OpenOffice, PDF und HTML. Fügen Sie befüllte Tabellen nahtlos in unterstützte Dokumenttypen ein."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So befüllen Sie eine Datentabelle dynamisch"
      content: |
        Dieses Beispiel zeigt, wie Sie eine Tabelle in einem DOCX-Dokument mit dynamischen Daten füllen.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Bereiten Sie eine Vorlage mit einem Platzhalter für die Tabelle vor
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Geben Sie den Dateipfad zur Vorlage an
          string template = "table_template.docx";

          // Rufen Sie Daten aus Ihrer gewählten Quelle ab
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Erstellen Sie ein Datenquelle-Objekt mit den erforderlichen Daten
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Initialisieren Sie DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie das fertige Dokument mit der befüllten Tabelle
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    title: "Entdecken Sie die Hauptmerkmale"
    exclude: "table"
    description: "Unsere Lösung vereinfacht die Erstellung professioneller Dokumente mit dynamisch befüllten Tabellen und zusätzlichen Elementen."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Berichte mit detaillierten Tabellen erstellen"
    exclude: "DOCX"
    description: ".NET ermöglicht die Erstellung umfassender Berichte, indem Vorlagen mit Tabellen und anderen Datenelementen in über 50 unterstützten Formaten gefüllt werden."
    items: 
          
        # format loop 1
        - name: "Fügen Sie eine Tabelle zu einem PDF hinzu"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Fügen Sie eine Tabelle zu einem DOCX hinzu"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Fügen Sie eine Tabelle zu einem PPTX hinzu"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Fügen Sie eine Tabelle zu einem XLSX hinzu"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---