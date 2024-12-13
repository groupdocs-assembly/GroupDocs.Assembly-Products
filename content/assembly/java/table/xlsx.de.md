



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: de
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Fügen Sie Tabellen zu XLSX-Dokumenten mit Java hinzu"
head_description: "Mit GroupDocs.Assembly for Java können Entwickler schnell Tabellen in Dokumente und E-Mails integrieren, indem sie Daten aus dynamischen Quellen abrufen."

############################# Header ############################
title: "Füllen Sie Tabellen in XLSX-Dateien mit unserer Java API aus" 
description: "GroupDocs.Assembly for Java vereinfacht den Prozess des Befüllens von Tabellen in XLSX-Dokumenten mit Daten aus verschiedenen Eingaben."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlose Testversion holen"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) ist ein Werkzeug zur Erstellung von Dokumenten und Berichten durch automatisches Einfügen von Daten in vorab gestaltete Vorlagen. Sie können mühelos Tabellen, Listen, Diagramme und Bilder hinzufügen. Seine fortschrittlichen Funktionen ermöglichen es Ihnen, Inhalte präzise in Ihren Dokumenten zu platzieren. Kompatibel mit über 50 Dateiformaten, einschließlich PDF, MS Office und E-Mail-Formaten.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Einfüllen von Daten in eine XLSX-Tabelle"
    content: |
      [GroupDocs.Assembly](/assembly/java/) hilft Ihnen, Tabellenvorlagen für XLSX und andere Formate auszufüllen. Nutzen Sie dynamische Daten aus Ihren Quellen, um Tabellen zu erstellen.
      
      1. Richten Sie eine XLSX-Vorlage mit Platzhaltern für Tabellenzeilen und -spalten ein.
      2. Ziehen Sie Daten aus einer unterstützten Eingangsquelle.
      3. Filtern oder verarbeiten Sie die Daten, um Ihren Anforderungen zu entsprechen.
      4. Generieren Sie das finale Dokument mit der ausgefüllten Tabelle.
   
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
        // Verwenden Sie diese Tags in einem Platzhalter für eine Tabellenzeile innerhalb Ihrer Vorlage
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Definieren Sie den Pfad zur Vorlage
        String template = "table_template.xlsx";

        // Laden Sie Daten aus Ihrer gewählten Quelle
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Speichern Sie die Ausgabedatei mit der ausgefüllten Tabelle
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Erstellen Sie Dokumente mit datengestützten Tabellen"
  description: "GroupDocs.Assembly for Java macht die Automatisierung der Tabellenerstellung in Ihren Dokumenten unkompliziert. Es unterstützt auch das Hinzufügen von Elementen wie Diagrammen, Listen und Bildern mithilfe von Vorlagen."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte aus mehreren Datenformaten generieren"
      content: "Die API funktioniert nahtlos mit JSON, XML, CSV und anderen Formaten, um Tabellen in Ihren Dokumenten mit organisierten Daten zu füllen."

    # feature loop
    - title: "Informationen visuell präsentieren"
      content: "GroupDocs.Assembly hilft Ihnen, professionelle Tabellen, Listen und Diagramme zu erstellen sowie Links, Texte und Bilder für ein hochwertiges Erscheinungsbild einzufügen."

    # feature loop
    - title: "Tabelleninhalte präzise platzieren"
      content: "Verwenden Sie eine flexible, LINQ-basierte Syntax, um Zeilen und Spalten dynamisch hinzuzufügen. Passen Sie das Erscheinungsbild, einschließlich Schriftarten und Farben, programmgesteuert an."

    # feature loop
    - title: "Kompatibel mit mehreren Formaten"
      content: "Arbeiten Sie mit MS Office, OpenOffice, PDF, HTML und mehr. Fügen Sie Tabellen mühelos in jedes unterstützte Dateiformat ein."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dynamisch eine datengestützte Tabelle erstellen"
      content: |
        Dieses Beispiel zeigt, wie man eine Tabelle in einem XLSX-Dokument mit dynamischen Eingabedaten befüllt.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Gestalten Sie eine Vorlage mit einem Platzhalter für die Tabelle
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Legen Sie den Standort der Vorlagendatei fest
          String template = "table_template.xlsx";

          // Laden Sie Daten aus Ihrer bevorzugten Quelle
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Bereiten Sie ein Datenobjekt vor, das die erforderlichen Felder enthält
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Erstellen Sie eine Instanz von DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie das Dokument mit der ausgefüllten Tabelle
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_table.xlsx"
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
    title: "Wichtige Funktionen auf einen Blick"
    exclude: "table"
    description: "Unsere API vereinfacht die Erstellung professioneller Dokumente, indem sie die Tabellenbefüllung zusammen mit anderen leistungsstarken Komponenten automatisiert."
    items: 
          
        # operation loop 1
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "Erstellen und fügen Sie dynamisch Barcodes in Dokumente ein"

        # operation loop 2
        - name: "Daten mit Diagrammen visualisieren"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "Füllen Sie verschiedene Diagrammtypen mit Daten"

        # operation loop 3
        - name: "Dokumente zusammenführen"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "Kombinieren Sie den Inhalt eines Dokuments mit einem anderen"

        # operation loop 4
        - name: "Daten mit Listen anzeigen"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "Erstellen Sie Listen in Dokumenten mit spezifischen Daten"

        # operation loop 5
        - name: "Daten in Tabellen organisieren"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "Daten aus jeder Quelle abrufen und Tabellen befüllen"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Erstellen Sie detaillierte Tabellen in verschiedenen Formaten"
    exclude: "XLSX"
    description: "Mit Java können Sie Vorlagen mit Daten befüllen und detaillierte Berichte in über 50 Dateiformaten erstellen."
    items: 
          
        # format loop 1
        - name: "Fügen Sie eine Tabelle zu einem PDF hinzu"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Fügen Sie eine Tabelle zu einem DOCX hinzu"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Fügen Sie eine Tabelle zu einem PPTX hinzu"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Fügen Sie eine Tabelle zu einem XLSX hinzu"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---