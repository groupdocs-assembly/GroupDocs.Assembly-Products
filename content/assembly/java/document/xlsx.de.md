



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:07
draft: false
lang: de
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "XLSX-Dokumente mit Java in einander einfügen"
head_description: "Kombinieren Sie XLSX-Dateien mit Java. GroupDocs.Assembly vereinfacht den Prozess des Zusammenführens von Dokumenten in nur wenigen Codezeilen."

############################# Header ############################
title: "XLSX-Dokumente nahtlos einbetten" 
description: "GroupDocs.Assembly for Java ermöglicht es Ihnen, ein XLSX-Dokument in ein anderes einzufügen. Erhalten Sie präzise Ergebnisse mit flexiblen und zuverlässigen Tools."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt kostenlos erhalten"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) ist eine vielseitige Lösung für die Dokumentenverarbeitung. Es ermöglicht Ihnen, ein Dokument in ein anderes zu integrieren und unterstützt über 50 Formate wie PDF- und MS Office-Dateien. Gestalten Sie Ihre Ausgabe, indem Sie Inhalte nach Ihren Wünschen zusammenführen, bearbeiten und organisieren.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Einfügen eines Dokuments in eine XLSX-Datei"
    content: |
      [GroupDocs.Assembly](/assembly/java/) macht das Einbetten eines XLSX-Dokuments in ein anderes einfach und anpassbar.
      
      1. Bereiten Sie eine XLSX-Vorlage mit Platzhaltern für den eingebetteten Inhalt vor.
      2. Geben Sie den Dateipfad der Vorlage an.
      3. Geben Sie den Dateipfad für das einzufügende Dokument an.
      4. Speichern Sie die Ausgabedatei mit dem zusammengeführten Inhalt.
   
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
        // Verwenden Sie dieses Tag in Ihrer Vorlage, um die Stelle für das eingebettete Dokument zu markieren
        // <<doc [doc_expression]>>

        // Legen Sie den Dateipfad für die Hauptvorlage fest
        String template = "doc_template.xlsx";

        // Geben Sie den Pfad zu dem Dokument an, das Sie einfügen möchten
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // Speichern Sie die finale Datei mit dem eingebetteten Inhalt
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Fortgeschrittene Werkzeuge zur Vereinfachung der Dokumentenintegration"
  description: "Mit GroupDocs.Assembly for Java ist das Einbetten von Dokumenten unkompliziert und anpassbar, unabhängig vom Dateityp. Erreichen Sie klare und konsistente Ergebnisse in Ihren Projekten."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Höhepunkte von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte mit Geschäftsdaten erstellen"
      content: "Füllen Sie Dokumente schnell und zuverlässig mit Daten aus Quellen wie JSON, XML oder CSV und optimieren Sie Ihre Arbeitsabläufe."

    # feature loop
    - title: "Dokumente mit visuellem Inhalt verbessern"
      content: "GroupDocs.Assembly ermöglicht die Einfügung von Tabellen, Diagrammen und Listen zusammen mit Text, Hyperlinks, Bildern und sogar dynamischen Barcodes."

    # feature loop
    - title: "Daten genau dort platzieren, wo sie hingehören"
      content: "LINQ-Vorlagen helfen, Ihre Daten präzise zu positionieren, wiederholende Elemente wie Arrays zu handhaben und benutzerdefinierte Stile mühelos anzuwenden."

    # feature loop
    - title: "Kompatibel mit verschiedenen Dateiformaten"
      content: "Fügen Sie Dokumente über verschiedene Formate hinweg zusammen, einschließlich PDFs, HTML, MS Office-Dateien und OpenOffice, um Flexibilität für Ihre Projekte zu gewährleisten."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Wie man programmatisch ein Bild in ein Dokument einfügt"
      content: |
        Dieses Beispiel zeigt, wie man ein Bild in eine XLSX-Datei mit GroupDocs.Assembly einbettet.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Fügen Sie ein Platzhalter-Tag in die Vorlagendatei ein
          // <<image [expression]>>

          // Definieren Sie den Pfad zur Vorlage
          String template = "template.xlsx";

          // Geben Sie den Pfad zum Bild an
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Initialisieren Sie die DocumentAssembler-Instanz
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie die Datei mit dem eingebetteten Bild
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "Wesentliche Funktionen auf einen Blick"
    exclude: "document"
    description: "Entdecken Sie die umfangreichen Funktionen, die GroupDocs.Assembly bietet, um das Einbetten und Kombinieren von Dokumenten effizient und problemlos zu gestalten."
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
    title: "Über verschiedene Dokumenttypen hinweg zusammenführen"
    exclude: "XLSX"
    description: "Mit Java können Sie Inhalte über mehr als 50 Dateiformate einbetten und kombinieren. Fügen Sie Dateien nahtlos hinzu, um professionelle Ergebnisse zu erzielen."
    items: 
          
        # format loop 1
        - name: "Binden Sie ein Dokument in ein PDF ein"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Binden Sie ein Dokument in ein DOCX ein"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Binden Sie ein Dokument in ein PPTX ein"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Binden Sie ein Dokument in ein XLSX ein"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---