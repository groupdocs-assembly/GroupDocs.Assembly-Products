---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: de
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET-API für Dokumentautomatisierung, -zusammenstellung und -berichterstellung"
head_description: "C# .NET API für Dokumentautomatisierung, -zusammenstellung und -berichterstellung. Erstellen Sie PDF, Word, Excel, PPTX, HTML- und E-Mail-Dokumente aus benutzerdefinierten Vorlagen."

############################# Header ############################
title: ".NET-Dokumentautomatisierungs- und Berichterstellungs-API"
description: "Generieren Sie Berichte in .NET-Anwendungen, indem Sie Vorlagen definieren und Daten zusammenführen."
words:
  for: "für"

actions:
  main: "Testversion über Nuget herunterladen"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an."

release:
  title: "Version {0} veröffentlicht"
  notes: "Sehen Sie, was neu ist"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Diagramm in DOCX mit C# ausfüllen"
  more: "Weitere Beispiele"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Pfad zur Hauptvorlage
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly Übersicht"
  description: ".NET-Lösung zur Automatisierung der Dokumentenerstellung mit fortschrittlicher Datenintegration."
  features:
    # feature loop
    - title: "Fügen Sie Geschäftsdaten mit C# zu Dokumentvorlagen hinzu"
      content: "Berichterstellung leicht gemacht: Mit GroupDocs.Assembly for .NET können Sie mühelos Daten aus Quellen wie JSON oder XML in vordefinierte Vorlagen einfügen."

    # feature loop
    - title: "Verarbeiten Sie native Datenobjekte"
      content: "Unterstützte Dokumenttypen umfassen eingebettete Objekte wie Diagramme, Tabellen, Tabellen und Listen, die automatisch mit Daten gefüllt werden können."

    # feature loop
    - title: "Zusätzliche Funktionen"
      content: "GroupDocs.Assembly for .NET bietet umfangreiche Anpassungsoptionen. Gestalten Sie Datenobjekte programmatisch, generieren Sie Barcodes, nutzen Sie Online-Datenquellen über URLs und speichern Sie Ausgaben in verschiedenen Formaten."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Assembly for .NET ist mit den folgenden Betriebssystemen, Frameworks und Paketmanagern kompatibel."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Assembly for .NET kann die folgenden [Dateiformate](https://docs.groupdocs.com/assembly/net/supported-document-formats/)verarbeiten.
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
  title: "GroupDocs.Assembly Funktionen"
  description: "Erstellen Sie Dokumente und Berichte mit erweiterten Datenmodellen."

  items:
    # feature loop
    - icon: "preview"
      title: "Erweiterte Datenrepräsentation"
      content: "Unterstützt eine breite Palette von Datenobjekten wie Diagramme, Listen, Tabellen, Bilder und mehr."

    # feature loop
    - icon: "manipulate"
      title: "Datenmanipulation"
      content: "Wenden Sie Formeln und sequenzielle Operationen an, um Daten effektiv zu formatieren und darzustellen."

    # feature loop
    - icon: "two_pages"
      title: "Breite der unterstützten Formate"
      content: "Arbeiten Sie nahtlos mit allen gängigen Dokumentformaten für Vorlagen oder Ausgabedateien."

    # feature loop
    - icon: "document_settings"
      title: "Reiches Vorlagen-Markup"
      content: "Nutzen Sie ordinale, kardinale und alphabetische numerische Formatierung in Vorlagen."

    # feature loop
    - icon: "text"
      title: "Barcodes einfügen"
      content: "Erzeugen Sie Barcode-Bilder dynamisch und fügen Sie diese in Ihre Dokumente ein."

    # feature loop
    - icon: "add"
      title: "Datenformatierung"
      content: "Formatieren Sie Strings in Vorlagen als Großbuchstaben, Kleinbuchstaben, kapitalisierte oder mit dem ersten Buchstaben als Großbuchstaben."

    # feature loop
    - icon: "manipulate"
      title: "Inhalt von Dokumenten manipulieren"
      content: "Fügen Sie dynamisch Inhalte von externen Dokumenten in Ihre Berichte ein."

    # feature loop
    - icon: "convert"
      title: "In mehreren Formaten speichern"
      content: "Geben Sie das Ausgabeformat der Datei anhand von Dateidownloads oder detaillierten Konfigurationen an."

    # feature loop
    - icon: "update"
      title: "Flexibles Datenverarbeiten"
      content: "Fügen Sie Bilder und Dokumente dynamisch mit Base64-codierten Bytes ein."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Codebeispiele für typische GroupDocs.Assembly-Operationen."
  items:
    # code sample loop
    - title: "Aufzählungsliste in einem Microsoft Word-Dokument"
      content: |
        [Aufzählungslisten](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) sind eine gängige Möglichkeit, Geschäftsdaten darzustellen. Hier ist ein Beispiel, wie man mit GroupDocs.Assembly eine Liste in ein Word-Dokument hinzufügt.
        {{< landing/code title="Wie man eine Liste in Dokumenten füllt">}}
        ```csharp {style=abap}
        // Fügen Sie diese Vorlage auf einer Dokumentseite ein:
        // Leistungsindikatoren der Manager
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Geben Sie den Vorlagenpfad an
        string template = "Bulleted List Template.docx";

        // Legen Sie den Ausgabedateipfad fest
        string result = "Result Report.docx"

        // Rufen Sie die Daten der Manager aus einer JSON-Quelle ab
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Generieren Sie den Bericht mit den ausgefüllten Daten
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tortendiagramme in PPTX-Präsentationen"
      content: |
        Sie können [Tortendiagramme](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) mithilfe von Vorlagen und XML-Daten erstellen. Verbessern Sie Ihre Berichte mit ansprechend dargestellten Daten.
        {{< landing/code title="Wie man Daten in einem Tortendiagramm darstellt">}}
        ```csharp {style=abap}
        // Fügen Sie das Titel-Template für das Diagramm zur Präsentation hinzu:
        // Umsatz der Kunden <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Fügen Sie auch das Daten-Template für das Diagramm hinzu:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Geben Sie den Pfad zur Diagrammvorlage an
        string template = "Pie Chart Template.pptx";

        // Legen Sie den Ausgabedateipfad fest
        string result = "Result Report.pptx"

        // Rufen Sie die Kundendaten aus einer XML-Quelle ab
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Generieren Sie das Diagramm und speichern Sie das Ergebnis
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---