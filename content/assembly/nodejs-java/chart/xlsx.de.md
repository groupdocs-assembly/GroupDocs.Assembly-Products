



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: de
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Diagramme in XLSX-Dateien mit JavaScript einfügen"
head_description: "Mit GroupDocs.Assembly for Node.js via Java können Entwickler schnell dynamische Diagramme in Dokumente einfügen, die auf Live-Datenquellen basieren."

############################# Header ############################
title: "Fügen Sie Diagramme mit Node.js zu XLSX-Dateien hinzu" 
description: "GroupDocs.Assembly for Node.js via Java vereinfacht den Prozess der Integration von Diagrammen in XLSX-Dokumente mit Echtzeitdaten."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt kostenlos starten"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Überblick über GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ist eine leistungsstarke Lösung zum Erstellen von automatisierten Dokumenten und Berichten. Fügen Sie Diagramme, Tabellen, Bilder, Barcodes und Listen präzise hinzu. Diese vielseitige Plattform unterstützt über 50 Formate, einschließlich PDFs, Office-Dokumenten und E-Mails.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Hinzufügen eines Diagramms zu einem XLSX-Dokument"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) erleichtert das Hinzufügen von Diagrammen zu XLSX-Dateien. Wählen Sie aus Diagrammtypen wie Balken-, Linien- oder Kreisdiagrammen.
      
      1. Entwerfen Sie eine XLSX-Vorlage mit Platzhaltern für Diagramme.
      2. Laden Sie Daten aus einer unterstützten Quelle.
      3. Konfigurieren Sie die Diagrammoptionen, einschließlich Typ, Farben und Beschriftungen.
      4. Exportieren Sie das Dokument mit dem eingebetteten Diagramm.
   
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
        // Fügen Sie dieses Tag in Ihre Vorlage ein, um ein Diagramm zu generieren
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Geben Sie den Pfad zur Vorlagendatei an
        const template = "chart_template.xlsx";

        // Extrahieren Sie Daten aus Ihrem Quellsystem
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Speichern Sie das endgültige Dokument mit dem eingebetteten Diagramm
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Diagramme mühelos in Ihren Dokumenten einfügen"
  description: "GroupDocs.Assembly for Node.js via Java ermöglicht es, funktionsreiche Dokumente in gängigen Dateiformaten zu erstellen. Verwenden Sie Vorlagen, um Diagramme, Tabellen, Barcodes, Listen, Bilder und mehr mit Echtzeitdatenaktualisierungen hinzuzufügen."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Daten in professionelle Diagramme umwandeln"
      content: "Konvertieren Sie Daten aus Quellen wie JSON, XML oder CSV in hochwertige Diagramme, die direkt in Dokumente eingebettet werden können."

    # feature loop
    - title: "Erstellen Sie beeindruckende Grafiken"
      content: "Generieren Sie Balkendiagramme, Kreisdiagramme und Liniendiagramme, die nahtlos mit anderen Dokumentenelementen wie Bildern, Tabellen und Barcodes funktionieren."

    # feature loop
    - title: "Flexible Diagrammgestaltung und -platzierung"
      content: "Nutzen Sie LINQ-Vorlagen, um die Positionierung und Gestaltung von Diagrammen zu steuern, einschließlich Farben, Layouts und Beschriftungen, für eine ansprechende Präsentation."

    # feature loop
    - title: "Unterstützt viele Dateiformate"
      content: "Erstellen Sie Dokumente in Formaten wie MS Office, PDF, OpenOffice und HTML, mit perfekt integrierten Diagrammen für ein professionelles Finish."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Diagramme dynamisch generieren und einfügen"
      content: |
        Dieses Beispiel veranschaulicht, wie man programmatisch Diagramme in XLSX-Dateien erstellt und einfügt.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Richten Sie eine Vorlage mit einem Platzhalter für das Diagramm ein
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Definieren Sie den Pfad zur Vorlagendatei
          const template = "table_template.xlsx";

          // Rufen Sie Daten aus einer gewählten Quelle ab
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Bereiten Sie ein Datenobjekt mit den Diagramminformationen vor
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Wählen Sie den Diagrammtyp und passen Sie dessen Aussehen an
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Initialisieren Sie DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Speichern Sie das aktualisierte Dokument mit dem eingebetteten Diagramm
          asm.assembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Entdecken Sie erweiterte Funktionen"
    exclude: "chart"
    description: "Diese Plattform vereinfacht die Dokumentenerstellung mit Tools, die für Datenvisualisierung und nahtlose Integration entwickelt wurden."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Berichte in mehreren Dateiformaten erstellen"
    exclude: "XLSX"
    description: "Node.js via Java unterstützt über 50 Formate, was es einfach macht, Vorlagen mit Daten zu kombinieren, um aufpolierte Dokumente zu produzieren."
    items: 
          
        # format loop 1
        - name: "Diagramme in PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Diagramme in DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Diagramme in PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Diagramme in XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---