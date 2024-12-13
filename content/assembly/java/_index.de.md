---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: de
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "Java-Bibliothek zur Dokumentenerstellung, Automatisierung und Berichterstellung"
head_description: "Java-Bibliothek zur Automatisierung der Dokumentenerstellung und Generierung von Berichten. Erstellen Sie PDF-, Word-, Excel-, PPTX-, HTML- und E-Mail-Dokumente mit benutzerdefinierten Vorlagen."

############################# Header ############################
title: "Java-API zur Automatisierung von Berichten und Dokumenten"
description: "Vereinfachen Sie die Berichterstellung in Java, indem Sie Daten mit Vorlagen zusammenführen."
words:
  for: "für"

actions:
  main: "Testversion über NuGet erhalten"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an."

release:
  title: "Version {0} veröffentlicht"
  notes: "Sehen Sie, was neu ist"
  downloads: "Downloads"

code:
  title: "Erzeugen eines Diagramms in DOCX mit Java"
  more: "Weitere Beispiele"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Pfad zur Hauptvorlage
    String template = "chart_template.docx";

    // Produktivitätsdaten der Manager aus der Quelle abrufen
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Erstellen Sie eine Instanz von DataSourceInfo mit den Daten
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Die Diagrammfaben mit einem anderen DataSourceInfo festlegen
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Die Vorlage mit Daten füllen und in die Ausgabe speichern
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly Übersicht"
  description: "Eine Java-Bibliothek, die für die automatisierte Dokumentenerstellung und nahtlose Datenintegration entwickelt wurde."
  features:
    # feature loop
    - title: "Fügen Sie Geschäftsdaten mit Java in Vorlagen ein"
      content: "Erstellen Sie mühelos professionelle Berichte, indem Sie Daten aus JSON, XML oder anderen Quellen in vordefinierte Vorlagen mithilfe von GroupDocs.Assembly for Java einfügen."

    # feature loop
    - title: "Arbeiten Sie mit eingebetteten Objekten"
      content: "Füllen Sie automatisch Elemente wie Tabellen, Diagramme und Diagramme in Dokumenten mit Daten aus externen Quellen aus."

    # feature loop
    - title: "Erweiterte Anpassung"
      content: "GroupDocs.Assembly for Java bietet flexible Funktionen wie die Erzeugung von Barcodes, das Abrufen von Online-Daten über URLs und das Exportieren von Ausgaben in verschiedenen Formaten."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Assembly for Java funktioniert nahtlos mit gängigen Betriebssystemen, Entwicklungsframeworks und Paketmanagern."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Assembly for Java unterstützt eine Vielzahl von [Dokumentformaten](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office Formate
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Bilder & Andere Formate
        * **Portabel:** PDF
        * **Bilder:** SVG, TIFF
        * **Andere Office-Formate:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Andere Formate
        * **Web:** HTML, MHTML
        * **E-Mails:** EML, MSG, EMLX
        * **Andere:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Hauptfähigkeiten von GroupDocs.Assembly"
  description: "Erstellen Sie professionelle Dokumente und Berichte mit fortschrittlicher Datenverarbeitung."

  items:
    # feature loop
    - icon: "preview"
      title: "Visuelle Datenobjekte"
      content: "Fügen Sie Elemente wie Diagramme, Tabellen, Bilder und Listen direkt in Ihre Dokumente ein und formatieren Sie diese."

    # feature loop
    - icon: "manipulate"
      title: "Datenumwandlung"
      content: "Verwenden Sie Formeln, Sortierung und andere Werkzeuge, um Ihre Daten effektiv zu organisieren und darzustellen."

    # feature loop
    - icon: "two_pages"
      title: "Unterstützung für mehrere Formate"
      content: "Arbeiten Sie mühelos mit gängigen Dateitypen für Vorlagen und Ausgabedateien."

    # feature loop
    - icon: "document_settings"
      title: "Erweiterte Formatierung von Vorlagen"
      content: "Passen Sie Vorlagen mit numerischen, alphabetischen und anderen erweiterten Formatierungsoptionen an."

    # feature loop
    - icon: "text"
      title: "Dynamische Barcode-Generierung"
      content: "Erstellen und fügen Sie schnell Barcode-Bilder nach Bedarf in Dokumente ein."

    # feature loop
    - icon: "add"
      title: "Flexible Textformatierung"
      content: "Wenden Sie Texttransformationen wie Großbuchstaben, Kleinbuchstaben, Titelcase oder andere Stile in Vorlagen an."

    # feature loop
    - icon: "manipulate"
      title: "Importieren Sie externe Inhalte"
      content: "Binden Sie Inhalte aus externen Dateien dynamisch in die Erstellung von Dokumenten ein."

    # feature loop
    - icon: "convert"
      title: "Exportieren in mehreren Formaten"
      content: "Speichern Sie endgültige Dokumente in verschiedenen Dateiformaten mit angegebenen Erweiterungen oder Konfigurationen."

    # feature loop
    - icon: "update"
      title: "Dynamisches Medien-Embedding"
      content: "Fügen Sie Bilder oder andere Inhalte mit Base64-codierten Daten während der Erstellung von Dokumenten ein."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Entdecken Sie Beispielcodes für häufige Aufgaben mit GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Erstellen Sie eine Aufzählungsliste in Word"
      content: |
        Erfahren Sie, wie Sie [Aufzählungslisten](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) zu Word-Dokumenten für eine organisierte Datenpräsentation hinzufügen. Dieses Beispiel zeigt, wie Sie mit GroupDocs.Assembly eine Liste in Word generieren.
        {{< landing/code title="Erstellen Sie eine Aufzählungsliste in Word">}}
        ```java {style=abap}
        // Fügen Sie diese Vorlage auf einer Dokumentseite ein:
        // Leistungsindikatoren der Manager
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Geben Sie den Vorlagenpfad an
        String template = "Bulleted List Template.docx";

        // Legen Sie den Ausgabedateipfad fest
        String result = "Result Report.docx"

        // Rufen Sie die Daten der Manager aus einer JSON-Quelle ab
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Generieren Sie den Bericht mit den ausgefüllten Daten
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Erstellen Sie Tortendiagramme in PPTX"
      content: |
        Verwenden Sie Vorlagen und XML, um [Tortendiagramme](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) in Ihre Präsentationen einzufügen. Machen Sie Ihre Berichte ansprechender, indem Sie Tortendiagramme zur Visualisierung von Daten einfügen.
        {{< landing/code title="Erstellen Sie Tortendiagramme in PPTX">}}
        ```java {style=abap}   
        // Fügen Sie das Titel-Template für das Diagramm zur Präsentation hinzu:
        // Umsatz der Kunden <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Fügen Sie auch das Daten-Template für das Diagramm hinzu:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Geben Sie den Pfad zur Diagrammvorlage an
        String template = "Pie Chart Template.pptx";

        // Legen Sie den Ausgabedateipfad fest
        String result = "Result Report.pptx"

        // Rufen Sie die Kundendaten aus einer XML-Quelle ab
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Generieren Sie das Diagramm und speichern Sie das Ergebnis
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---