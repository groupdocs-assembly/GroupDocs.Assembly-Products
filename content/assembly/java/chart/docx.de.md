



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: de
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Diagramme in DOCX-Dokumenten mit Java generieren"
head_description: "Die GroupDocs.Assembly for Java API ermöglicht Entwicklern die nahtlose Erstellung und Einfügung dynamischer Diagramme oder Grafiken in Dokumente, unterstützt durch Live-Daten."

############################# Header ############################
title: "Diagramme zu DOCX-Dokumenten mit Java API hinzufügen" 
description: "GroupDocs.Assembly for Java vereinfacht den Prozess der Einbettung von Diagrammen in DOCX-Dokumenten, indem es Echtzeitdaten nutzt."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt kostenlos starten"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Einführung in GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) ist eine vielseitige Lösung zur Automatisierung der Erstellung von Dokumenten und Berichten. Es ermöglicht die direkte Einfügung von Diagrammen, Tabellen, Listen, Barcodes und Bildern in Ihre Dateien, mit erweiterten Tools für präzise Formatierung und Datenintegration. Die Plattform unterstützt über 50 Formate, darunter PDF, Microsoft Office-Dateien und E-Mails.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zur Einbettung eines Diagramms in ein DOCX-Dokument"
    content: |
      [GroupDocs.Assembly](/assembly/java/) vereinfacht den Prozess der Einfügung von Diagrammen in DOCX-Vorlagen. Wählen Sie aus verschiedenen Diagrammtypen, einschließlich Balken-, Kreis- und Liniendiagrammen.
      
      1. Erstellen Sie eine DOCX-Vorlage mit Platzhaltern für das Diagramm.
      2. Laden Sie Ihre Daten aus einer kompatiblen Quelle.
      3. Legen Sie die Diagrammoptionen wie Typ, Labels und Farben fest.
      4. Speichern Sie das Dokument mit dem eingebetteten Diagramm.
   
    code:
      platform: "java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Beispieldokument"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "Klicken Sie zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Fügen Sie dieses Tag Ihrer Vorlage hinzu, um ein Diagramm einzufügen
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Geben Sie den Dateipfad zu Ihrer Vorlage an
        String template = "chart_template.docx";

        // Extrahieren Sie die erforderlichen Daten aus Ihrer Quelle
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Speichern Sie das endgültige Dokument mit dem eingebetteten Diagramm
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Dynamische Diagramme mühelos in Ihre Dokumente einbetten"
  description: "GroupDocs.Assembly for Java bietet eine unkomplizierte Möglichkeit, datenreiche Dokumente in gängigen Formaten zu erstellen. Verwenden Sie Vorlagen, um Diagramme, Tabellen, Barcodes, Listen, Links und Bilder mit dynamischen Updates aus Ihren Daten einzufügen."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Daten in Diagramme umwandeln"
      content: "Nutzen Sie die API, um Daten aus JSON, XML, CSV oder anderen Quellen in saubere, professionelle Diagramme für Ihre Dokumente zu verwandeln."

    # feature loop
    - title: "Visuell ansprechende Inhalte erstellen"
      content: "GroupDocs.Assembly unterstützt verschiedene visuelle Formate, darunter Säulendiagramme, Kreisdiagramme und Liniendiagramme, die mit Tabellen, Barcodes, Bildern und mehr für verbessere Berichte kombiniert werden können."

    # feature loop
    - title: "Anpassbare Diagrammplatzierung und -gestaltung"
      content: "Mit der LINQ-basierten Syntax können Sie Diagramme dynamisch im Dokument erstellen und positionieren und gleichzeitig Stil, Farben und Layouts problemlos an Ihre Designvorgaben anpassen."

    # feature loop
    - title: "Unterstützt mehrere Dokumentformate"
      content: "Generieren Sie Dokumente in Formaten wie MS Office, PDF, OpenOffice und HTML. Die Diagramme fügen sich nahtlos in jedes unterstützte Format ein und sorgen für professionelle Ergebnisse."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Diagramme programmgesteuert generieren und einfügen"
      content: |
        Dieses Beispiel zeigt, wie Sie ein Diagramm programmatisch in ein DOCX-Dokument erstellen und einfügen.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Bereiten Sie eine Vorlage mit einem Platzhalter für das Diagramm vor
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Geben Sie den Dateipfad zur Vorlage an
          String template = "table_template.docx";

          // Laden Sie Daten aus Ihrer gewählten Quelle
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Erstellen Sie ein Datenobjekt mit den relevanten Informationen
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Konfigurieren Sie den Diagrammtyp und das Aussehen
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Initialisieren Sie DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie das fertige Dokument mit dem eingebetteten Diagramm
          asm.assembleDocument(template, "result.docx", data, design);
          ```
        platform: "java"
        copy_title: "Kopieren"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "Klicken Sie zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Laden Sie das Ergebnis herunter"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.docx"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Bereit anzufangen?"
  description: "Erforschen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Herunterladen von Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Erfahren Sie mehr über Lizenzen"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Entdecken Sie leistungsstarke Funktionen"
    exclude: "chart"
    description: "Diese Plattform vereinfacht den Entwurfsprozess für datenorientierte, visuell ansprechende Dokumente, die auf Ihre Bedürfnisse zugeschnitten sind."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Umfassende Berichte in verschiedenen Formaten generieren"
    exclude: "DOCX"
    description: "Java ermöglicht Ihnen die Erstellung von Dokumenten mit integrierten Diagrammen in über 50 Dateiformaten, wodurch eine nahtlose Zusammenführung von Vorlagen und Daten gewährleistet wird."
    items: 
          
        # format loop 1
        - name: "Diagramme in PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Diagramme in DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Diagramme in PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Diagramme in XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---