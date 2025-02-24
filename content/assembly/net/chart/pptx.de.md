



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: de
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Diagramme in PPTX-Dateien mit C# erstellen"
head_description: "Die GroupDocs.Assembly for .NET API ermöglicht Entwicklern, Diagramme oder Grafiken dynamisch in Dokumente einzufügen, indem sie Echtzeitdaten nutzen."

############################# Header ############################
title: "Diagramme in PPTX-Dateien mit .NET API einbetten" 
description: "GroupDocs.Assembly for .NET bietet eine leistungsstarke Möglichkeit, PPTX-Dateien mit dynamischen Daten zu füllen und Diagramme mühelos zu integrieren."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos testen"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) ist ein Tool, das entwickelt wurde, um die Erstellung von Dokumenten und Berichten zu optimieren, indem Daten aus verschiedenen Quellen integriert werden. Generiere dynamisch Diagramme, Tabellen, Listen, Barcodes und Bilder. Fortschrittliche Formatierungsoptionen ermöglichen eine präzise Platzierung und Anpassung deiner Inhalte. Es unterstützt über 50 Dateiformate, einschließlich PDFs, MS Office-Dokumenten und E-Mails.

############################# Steps ############################
steps:
    enable: true
    title: "Wie man ein Diagramm in ein PPTX-Dokument einfügt"
    content: |
      [GroupDocs.Assembly](/assembly/net/) erleichtert das Erzeugen und Einbetten von Diagrammen in deine PPTX-Vorlagen. Unterstützt eine Vielzahl von Diagrammtypen, wie Balken-, Kreis- und Liniendiagramme.
      
      1. Entwirf eine PPTX-Vorlage mit Platzhaltern für die Diagramme.
      2. Rufe deine Daten aus einer kompatiblen Quelle ab.
      3. Definiere Diagrammoptionen wie Typ, Beschriftungen und Farbschema.
      4. Speichere die aktualisierte Datei mit dem eingebetteten Diagramm.
   
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
        // Füge dieses Tag in deine Vorlage ein, um ein Diagramm zu generieren
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Gib den Dateipfad für deine Vorlage an
        string template = "chart_template.pptx";

        // Lade Daten aus deiner bevorzugten Quelle
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Speichere das Dokument mit dem eingebetteten Diagramm
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Füge deiner Dokumentation mühelos dynamische Diagramme hinzu"
  description: "GroupDocs.Assembly for .NET vereinfacht die Erstellung von datengestützten Dokumenten in weit verbreiteten Formaten. Nutze Vorlagen, um Diagramme, Tabellen, Barcodes, Listen, Hyperlinks und Bilder mit fortschrittlicher, dynamischer Datenintegration einzufügen."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Daten in professionelle Diagramme umwandeln"
      content: "Wandle Daten aus JSON, XML, CSV und anderen Quellen in ansprechend gestaltete Diagramme mit nur wenigen Schritten mithilfe unserer API um."

    # feature loop
    - title: "Visuell ansprechende Inhalte erstellen"
      content: "GroupDocs.Assembly unterstützt mehrere Diagrammtypen wie Balkendiagramme, Kreisdiagramme und Liniendiagramme. Kombiniere diese mit Tabellen, Barcodes, Bildern und anderen Elementen, um professionelle Berichte zu erstellen."

    # feature loop
    - title: "Diagramme präzise positionieren und anpassen"
      content: "Mit LINQ-Syntax kannst du Diagramme dynamisch generieren und genau dort platzieren, wo sie benötigt werden. Stile, Farben und Layout lassen sich problemlos an deine Anforderungen anpassen."

    # feature loop
    - title: "Funktioniert mit verschiedenen Dateiformaten"
      content: "Erstelle Dokumente in beliebten Formaten wie MS Office, PDF, OpenOffice und HTML. Betten Sie Diagramme nahtlos in jedes unterstützte Format mit voller Kompatibilität ein."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ein Diagramm programmgesteuert erstellen"
      content: |
        Dieses Beispiel zeigt, wie man dynamisch ein Diagramm in ein PPTX-Dokument erstellt und einfügt.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Bereite eine Vorlage mit einem Platzhalter für das Diagramm vor
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Gib den Pfad zur Vorlagendatei an
          string template = "table_template.pptx";

          // Rufe die Daten aus deiner Quelle ab
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Erstelle ein Datenobjekt mit den erforderlichen Informationen
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Lege die Diagrammeigenschaften wie Typ und Erscheinungsbild fest
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Initialisiere DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Exportiere das Dokument mit dem enthaltenen Diagramm
          asm.AssembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "Entdecke die wichtigsten Funktionen"
    exclude: "chart"
    description: "Unsere Plattform hilft dir, überzeugende, datengestützte Dokumente zu erstellen, die auf deine Bedürfnisse zugeschnitten sind."
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
    title: "Erstelle visuell ansprechende Berichte in mehreren Formaten"
    exclude: "PPTX"
    description: ".NET ermöglicht es dir, Dokumente mit integrierten Diagrammen in über 50 unterstützten Formaten zu generieren und Vorlagen nahtlos mit deinen Daten zu kombinieren."
    items: 
          
        # format loop 1
        - name: "Diagramme in PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Diagramme in DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Diagramme in PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Diagramme in XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---