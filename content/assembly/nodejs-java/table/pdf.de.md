



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: de
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tabellen in PDF-Dokumente mit JavaScript einfügen"
head_description: "Verwenden Sie GroupDocs.Assembly for Node.js via Java, um Tabellen schnell in Dokumente oder E-Mails einzufügen und Daten aus verschiedenen Quellen zu beziehen."

############################# Header ############################
title: "Tabellen mühelos zu PDF-Dateien mit Node.js hinzufügen" 
description: "Mit GroupDocs.Assembly for Node.js via Java ist das Befüllen von Tabellen in PDF-Dokumenten unkompliziert, indem Daten aus mehreren Quellen verwendet werden."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Testversion starten"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Einführung in GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ist ein leistungsstarkes Tool zur Automatisierung der Dokumentenerstellung. Es ermöglicht das einfache Einfügen von Tabellen, Diagrammen, Listen und Bildern in Vorlagen mit präziser Inhaltsplatzierung. Mit Unterstützung für über 50 Dateiformate, einschließlich PDF, Word und E-Mail, optimiert es die Erstellung von Berichten und anderen Aufgaben.

############################# Steps ############################
steps:
    enable: true
    title: "Wie man Daten in eine Tabelle in PDF einfügt"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ermöglicht es Ihnen, dynamische Datenquellen schnell für Tabellenvorlagen in PDF-Dateien zu nutzen.
      
      1. Erstellen Sie eine Vorlage mit Platzhaltern für die Tabelle (PDF-Vorlagen werden derzeit nicht unterstützt).
      2. Laden Sie Daten aus einer unterstützten Quelle wie JSON oder CSV.
      3. Organisieren und formatieren Sie die Daten nach Bedarf.
      4. Exportieren Sie das Dokument mit der gefüllten Tabelle als PDF-Datei.
   
    code:
      platform: "java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Beispieldokument"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "Klicken Sie zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Fügen Sie diese Tags in die Platzhalter für Tabellenzeilen Ihrer Vorlage ein
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Geben Sie den Pfad zur Vorlagendatei an
        // PDF-Vorlagen werden zurzeit nicht unterstützt.
        const template = "table_template.docx";

        // Laden Sie Ihre Daten aus einer ausgewählten Quelle
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Speichern Sie das endgültige Dokument mit der ausgefüllten Tabelle
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Datengetriebene Tabellen einfach in Dokumente einfügen"
  description: "GroupDocs.Assembly for Node.js via Java ermöglicht es Benutzern, Tabellen automatisch zu erstellen und gleichzeitig Diagramme, Bilder und Listen mit vorlagenbasierten Workflows einzufügen."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Top-Funktionen von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Tabellen aus strukturierten Daten generieren"
      content: "Daten aus JSON, XML, CSV und anderen Formaten abrufen, um Dokumenttabellen automatisch auszufüllen."

    # feature loop
    - title: "Professionelle visuelle Inhalte erstellen"
      content: "Verwenden Sie GroupDocs.Assembly, um professionelle Tabellen, Diagramme und Listen zu gestalten und Links, Bilder sowie Text für ein verfeinertes Dokumentenlayout hinzuzufügen."

    # feature loop
    - title: "Dynamische Inhaltsplatzierung in Tabellen"
      content: "Reihen und Spalten programmgesteuert mit LINQ-basierten Vorlagen hinzufügen und Stile wie Schriftarten, Farben und Ausrichtung anpassen."

    # feature loop
    - title: "Funktioniert nahtlos über Formate hinweg"
      content: "Tabellen in MS Office, OpenOffice, PDF, HTML und anderen Formaten einfach erstellen oder bearbeiten und nach Bedarf in Dateien zusammenführen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So fügen Sie programmgesteuert eine Tabelle ein"
      content: |
        Dieses Beispiel zeigt, wie man eine Tabelle in einem PDF-Dokument mit Daten aus einer externen Quelle füllt.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Gestalten Sie eine Vorlage mit Platzhaltern für die Tabelle
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Geben Sie den Dateipfad zur Vorlage an
          // PDF-Vorlagen werden zurzeit nicht unterstützt.
          const template = "table_template.docx";

          // Laden Sie die erforderlichen Daten aus Ihrer Quelle
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Organisieren Sie die Daten in die notwendige Struktur
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Initialisieren Sie DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Speichern Sie das Ausgabedokument mit der ausgefüllten Tabelle
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "Kopieren"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "Klicken Sie zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Laden Sie das Ergebnis herunter"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.pdf"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Bereit anzufangen?"
  description: "Erforschen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Herunterladen von NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Erfahren Sie mehr über Lizenzen"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Kernfunktionen auf einen Blick"
    exclude: "table"
    description: "Unsere API automatisiert die Tabellenerstellung und verbessert die Dokumentengenerierung mit vielseitigen Tools und Vorlagen."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tabellen in einer Vielzahl von Formaten generieren"
    exclude: "PDF"
    description: "Mit Node.js via Java Vorlagen ausfüllen und umfassende Tabellen über mehr als 50 unterstützte Dateitypen erstellen."
    items: 
          
        # format loop 1
        - name: "Fügen Sie eine Tabelle zu einem PDF hinzu"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Fügen Sie eine Tabelle zu einem DOCX hinzu"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Fügen Sie eine Tabelle zu einem PPTX hinzu"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Fügen Sie eine Tabelle zu einem XLSX hinzu"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---