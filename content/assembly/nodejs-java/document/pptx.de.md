



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: de
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Dokumente im PPTX mit JavaScript zusammenführen"
head_description: "JavaScript ermöglicht das Kombinieren von PPTX-Dateien. GroupDocs.Assembly vereinfacht das Zusammenführen von Dokumenten in nur wenigen Schritten."

############################# Header ############################
title: "Inhalte in PPTX-Dateien mühelos kombinieren" 
description: "Mit GroupDocs.Assembly for Node.js via Java ist das Integrieren einer PPTX-Datei in eine andere schnell und präzise. Profitieren Sie von flexiblen, zuverlässigen Werkzeugen für nahtloses Merging."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt kostenlos testen"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Überblick über GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) bietet eine leistungsstarke Möglichkeit zur Verwaltung von Dokumenten. Fügen Sie mit Leichtigkeit eine Datei in eine andere ein und unterstützen Sie über 50 Formate, darunter PDF und MS Office. Passen Sie Layouts an, bearbeiten Sie Inhalte und organisieren Sie Dokumente ganz nach Ihren Bedürfnissen.

############################# Steps ############################
steps:
    enable: true
    title: "Wie man ein Dokument in eine PPTX-Datei zusammenführt"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ermöglicht es Ihnen, eine PPTX-Datei in eine andere mit anpassbaren Optionen einzufügen.
      
      1. Entwerfen Sie eine PPTX-Vorlage mit Platzhaltern für den Inhalt.
      2. Setzen Sie den Dateipfad für die Vorlage.
      3. Geben Sie den Dateipfad für das zusammenzufügende Dokument an.
      4. Exportieren Sie die endgültige Datei mit dem kombinierten Inhalt.
   
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
        // Fügen Sie dieses Tag in Ihre Vorlage ein, um zu definieren, wo das Dokument eingebettet wird.
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Setzen Sie den Dateipfad für die Hauptvorlage.
        const template = "doc_template.pptx";

        // Geben Sie den Pfad für das Dokument an, das Sie zusammenführen möchten.
        const data 
            = new assemblyLib.DataSourceInfo("insert.pptx", "doc_expression");

        // Speichern Sie die endgültige Ausgabe mit dem eingebetteten Dokument.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Leistungsstarke Werkzeuge für die Dokumentenintegration"
  description: "GroupDocs.Assembly for Node.js via Java ermöglicht das Einbetten von Dateien in verschiedenen Formaten auf einfache und vollständig anpassbare Weise. Liefern Sie jedes Mal konsistente, professionelle Ergebnisse."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte mit Geschäftsdaten generieren"
      content: "Ziehen Sie Daten aus JSON-, XML- oder CSV-Quellen, um umfassende Berichte und Dokumente schnell und präzise zu erstellen."

    # feature loop
    - title: "Reiche visuelle Elemente hinzufügen"
      content: "GroupDocs.Assembly ermöglicht es Ihnen, Tabellen, Diagramme, Listen, Bilder und Strichcodes neben Text und Hyperlinks einzufügen."

    # feature loop
    - title: "Präzise Datenplatzierung"
      content: "Verwenden Sie LINQ-Vorlagen, um Daten genau dort zu platzieren, wo sie hingehören, wiederkehrende Elemente wie Arrays zu handhaben und Stile mühelos anzupassen."

    # feature loop
    - title: "Kompatibel mit verschiedenen Formaten"
      content: "Fügen Sie Inhalte nahtlos über Formate wie PDFs, MS Office-Dateien, HTML und OpenOffice zusammen und bieten Sie Flexibilität für alle Projekte."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ein Bild programmgesteuert in ein Dokument einfügen"
      content: |
        Dieses Beispiel zeigt, wie man ein Bild in eine PPTX-Datei mit GroupDocs.Assembly einfügt.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Fügen Sie einen Platzhalter in die Vorlage für das Bild ein.
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Geben Sie den Pfad zur Vorlage an.
          const template = "template.pptx";

          // Setzen Sie den Pfad zum Bild, das Sie einbetten möchten.
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Initialisieren Sie das DocumentAssembler-Objekt.
          const asm = new assemblyLib.DocumentAssembler();

          // Speichern Sie das Dokument mit dem enthaltenen Bild.
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    exclude: "document"
    description: "Erkunden Sie die umfassenden Werkzeuge, die GroupDocs.Assembly für effizientes und nahtloses Dokumenten-Merging bietet."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Dokumente in vielen Formaten kombinieren"
    exclude: "PPTX"
    description: "Verwenden Sie Node.js via Java, um Inhalte über 50 Datei-Formate hinweg zusammenzuführen und professionelle und makellose Ergebnisse zu garantieren."
    items: 
          
        # format loop 1
        - name: "Binden Sie ein Dokument in ein PDF ein"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Binden Sie ein Dokument in ein DOCX ein"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Binden Sie ein Dokument in ein PPTX ein"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Binden Sie ein Dokument in ein XLSX ein"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---