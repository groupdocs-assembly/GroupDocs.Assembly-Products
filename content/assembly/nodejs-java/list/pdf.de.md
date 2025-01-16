



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: de
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Erstellen Sie dynamische Listen in PDF mit JavaScript"
head_description: "Gestalten und fügen Sie Listen in PDF-Vorlagen über die GroupDocs.Assembly for Node.js via Java-API ein."

############################# Header ############################
title: "Datengetriebene Listen in PDF-Dateien mit Node.js einbetten" 
description: "GroupDocs.Assembly for Node.js via Java bietet leistungsstarke Werkzeuge, um flexible, datenbasierte Listen in PDF-Dokumente einzufügen."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos starten"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) vereinfacht die Dokumentenerstellung, indem Daten aus verschiedenen Quellen gezogen und in Vorlagen eingebettet werden. Nutzen Sie es, um Listen, Tabellen, Diagramme und andere Elemente zu erstellen, mit präziser Platzierung und Formatierungsoptionen. Mit Unterstützung für über 50 Formate, einschließlich PDF, MS Office und E-Mails, hilft es, Ihren Dokumentenerstellungsprozess zu automatisieren.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Einfügen einer Liste in eine PDF-Datei"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) vereinfacht das Hinzufügen detaillierter, datengetriebener Listen zu Ihren PDF-Vorlagen.
      
      1. Gestalten Sie eine Vorlage mit Platzhaltern für die Liste (PDF-Vorlagen werden derzeit nicht unterstützt).
      2. Geben Sie den Dateipfad der Vorlage an.
      3. Laden Sie Daten aus unterstützten Quellen wie JSON oder XML.
      4. Exportieren Sie das fertiggestellte Dokument mit der Liste als PDF-Datei.
   
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
        // Platzieren Sie dieses Tag in Ihrer Vorlage, um zu markieren, wo die Liste erscheinen soll
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Setzen Sie den Dateipfad für Ihre Vorlage
        // PDF-Vorlagen werden derzeit nicht unterstützt.
        const template = "list_template.docx";

        // Holen Sie die Daten aus der gewünschten Quelle
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Speichern Sie die Datei mit der eingefügten Liste
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Dokumente mit integrierten Daten auf einfache Weise erstellen"
  description: "Mit GroupDocs.Assembly for Node.js via Java können Sie Listen, Tabellen, Diagramme und andere Elemente in Vorlagen einbetten und so Zeit und Aufwand sparen."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Highlights von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte aus mehreren Datenquellen generieren"
      content: "Importieren Sie Daten aus JSON, XML, CSV oder anderen Formaten, um Listen und andere Komponenten effizient zu befüllen."

    # feature loop
    - title: "Listen und andere visuelle Elemente hinzufügen"
      content: "GroupDocs.Assembly ermöglicht es Ihnen, Listen, Tabellen, Diagramme und mehr nahtlos neben Text, Bildern und Links für ein professionelles Ergebnis einzufügen."

    # feature loop
    - title: "Daten präzise platzieren und gestalten"
      content: "LINQ-basierte Vorlagen ermöglichen es Ihnen, genau zu steuern, wo Listen und andere Daten erscheinen, Schleifen für wiederkehrende Elemente zu verwenden und Stile anzupassen, um Ihren Anforderungen gerecht zu werden."

    # feature loop
    - title: "Funktioniert über mehrere Formate hinweg"
      content: "Erstellen Sie Dokumente in Formaten wie MS Office, PDF, OpenOffice, HTML und E-Mails. Fügen Sie Inhalte aus verschiedenen Quellen in eine einzige Datei zusammen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Programmatisch eine Liste in ein Dokument erstellen"
      content: |
        Dieses Beispiel zeigt, wie Sie dynamisch eine Liste zu einem PDF-Dokument mit GroupDocs.Assembly hinzufügen.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Fügen Sie in Ihrer Vorlage einen Platzhalter für die Liste hinzu
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Geben Sie den Dateipfad der Vorlage an
          // PDF-Vorlagen werden derzeit nicht unterstützt.
          const template = "numlist_template.docx";

          // Laden Sie Daten, um die Liste zu befüllen
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Bereiten Sie die Datenquelle mit den erforderlichen Details vor
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Initialisieren Sie den DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Speichern Sie das endgültige Dokument mit der enthaltenen Liste
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "Entdecken Sie die Funktionen von GroupDocs.Assembly"
    exclude: "list"
    description: "Gestalten und generieren Sie datenreiche Dokumente mühelos mithilfe leistungsstarker Integrationswerkzeuge."
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
    title: "Dokumente in mehreren Formaten erstellen"
    exclude: "PDF"
    description: "Node.js via Java unterstützt über 50 Dateiformate, wodurch es leicht ist, Vorlagen und Daten in professionelle Ergebnisse zu integrieren."
    items: 
          
        # format loop 1
        - name: "Erstellen Sie eine Liste in einem PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Erstellen Sie eine Liste in einem DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Erstellen Sie eine Liste in einem PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Erstellen Sie eine Liste in einem XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---