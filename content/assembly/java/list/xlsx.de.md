



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:09
draft: false
lang: de
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Listen in XLSX-Dokumenten mit Java erstellen"
head_description: "GroupDocs.Assembly for Java-API ermöglicht das Entwerfen und Einfügen dynamischer Listen in Ihre XLSX-Vorlagen."

############################# Header ############################
title: "Dynamische Listen zu XLSX-Dateien mit unserer Java-API hinzufügen" 
description: "GroupDocs.Assembly for Java bietet flexible Werkzeuge zur Erstellung und zum Einfügen von datenreichen Listen direkt in XLSX-Dokumente."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos testen"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Mehr erfahren"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) erleichtert das Entwerfen professioneller Dokumente durch das Abrufen von Daten aus mehreren Quellen. Verwenden Sie es zur Erstellung von Listen, Tabellen, Diagrammen oder Texten und platzieren Sie diese Elemente mithilfe fortschrittlicher Vorlagenfunktionen genau dort, wo sie benötigt werden. Mit Unterstützung für über 50 Formate, einschließlich PDF, MS Office-Dateien und E-Mail-Dokumenten, hilft es, Ihren Workflow zu automatisieren und zu optimieren.

############################# Steps ############################
steps:
    enable: true
    title: "So fügen Sie eine datengestützte Liste in ein XLSX-Dokument ein"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ermöglicht es Ihnen, schnell datenreiche Listen in XLSX-Vorlagen einzufügen. Passen Sie den Inhalt mühelos an und organisieren Sie ihn.
      
      1. Erstellen Sie eine XLSX-Vorlage und markieren Sie Platzhalter für die Liste.
      2. Legen Sie den Dateipfad zur Vorlage fest.
      3. Rufen Sie Daten aus unterstützten Formaten wie JSON oder XML ab.
      4. Speichern Sie das finale Dokument mit der hinzugefügten Liste.
   
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
        // Fügen Sie dieses Tag in Ihrer Vorlage ein, wo die Liste erscheinen soll
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Definieren Sie den Dateipfad der Vorlage
        String template = "list_template.xlsx";

        // Daten aus Ihrer gewählten Quelle abrufen
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Das Dokument mit der eingebetteten Liste speichern
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Dokumente aus Vorlagen mit Datenintegration generieren"
  description: "GroupDocs.Assembly for Java vereinfacht das Hinzufügen dynamischer Listen, Tabellen, Diagramme und anderer Komponenten in Dokumentvorlagen."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Berichte mit Daten aus verschiedenen Quellen erstellen"
      content: "Verwenden Sie Daten aus Formaten wie JSON, XML und CSV, um Listen und andere Komponenten effizient zu befüllen."

    # feature loop
    - title: "Listen und andere Daten Elemente nahtlos hinzufügen"
      content: "GroupDocs.Assembly ermöglicht das Einbetten von Listen, Diagrammen, Tabellen und mehr, neben Texten, Bildern und Links, um ansprechende Dokumente zu erstellen."

    # feature loop
    - title: "Präzise steuern, wo Daten erscheinen"
      content: "LINQ-basierte Vorlagen ermöglichen es Ihnen, genaue Positionen für Ihre Listen und Daten zu definieren. Verwenden Sie Schleifen, um automatisch detaillierte Listen zu erstellen und benutzerdefinierte Formatierungen anzuwenden."

    # feature loop
    - title: "Unterstützt verschiedene Dokumentenformate"
      content: "Erstellen oder bearbeiten Sie Dateien in Formaten wie MS Office, PDF, OpenOffice, HTML und E-Mail. Fügen Sie Inhalte aus mehreren Dokumenten nach Bedarf zusammen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So erstellen Sie eine Liste programmgesteuert"
      content: |
        Dieses Beispiel zeigt, wie eine Liste dynamisch in eine XLSX-Datei mit GroupDocs.Assembly hinzugefügt wird.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Fügen Sie in Ihrer Vorlage ein Platzhaltersymbol für die Liste hinzu
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Geben Sie den Dateipfad zu Ihrer Vorlage an
          String template = "numlist_template.xlsx";

          // Holen Sie die erforderlichen Daten, um die Liste zu befüllen
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Bereiten Sie die Datenquelle mit den notwendigen Details vor
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Initialisieren Sie DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Speichern Sie das Ausgabedokument mit der fertiggestellten Liste
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "Entdecken Sie, was GroupDocs.Assembly leisten kann"
    exclude: "list"
    description: "Gestalten und generieren Sie Inhaltsreiche Dokumente mit fortschrittlichen Datenintegrationswerkzeugen."
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
    title: "Produzieren Sie Dokumente in verschiedenen Formaten"
    exclude: "XLSX"
    description: "Java unterstützt über 50 Formate, mit denen Sie strukturierte Dokumente durch Kombinieren von Daten und Vorlagen erstellen können."
    items: 
          
        # format loop 1
        - name: "Erstellen Sie eine Liste in einem PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Erstellen Sie eine Liste in einem DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Erstellen Sie eine Liste in einem PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Erstellen Sie eine Liste in einem XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Microsoft Excel Open XML-Tabellenblatt"


          

---