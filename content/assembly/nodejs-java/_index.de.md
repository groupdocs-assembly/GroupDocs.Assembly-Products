---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: de
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Toolkit zum Erstellen, Automatisieren und Anpassen von Dokumenten"
head_description: "Node.js-Bibliothek zur Automatisierung von Dokumenten-Workflows. Erstellen Sie PDF-, Word-, Excel-, PowerPoint-, HTML- und E-Mail-Dateien aus Ihren Vorlagen."

############################# Header ############################
title: "Node.js API für vereinfachte Dokumenten- und Berichtautomatisierung"
description: "Optimieren Sie die Erstellung von JavaScript-Berichten, indem Sie Ihre Daten mit vorgefertigten Vorlagen zusammenführen."
words:
  for: "für"

actions:
  main: "Beginnen Sie Ihre Testversion bei NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Assembly kostenlos oder fordern Sie eine Lizenz an."

release:
  title: "Version {0} veröffentlicht"
  notes: "Sehen Sie, was neu ist"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Erstellen Sie ein Diagramm in einem Word-Dokument mit Node.js"
  more: "Weitere Beispiele"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Pfad zur Hauptvorlage
    const template = "chart_template.docx";

    // Produktivitätsdaten der Manager aus der Quelle abrufen
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Erstellen Sie eine Instanz von DataSourceInfo mit den Daten
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Die Diagrammfaben mit einem anderen DataSourceInfo festlegen
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Die Vorlage mit Daten füllen und in die Ausgabe speichern
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly Übersicht"
  description: "Eine Node.js-Bibliothek, die entwickelt wurde, um Dokumente programmatisch mit integrierter Datenverarbeitung zu erstellen."
  features:
    # feature loop
    - title: "Geschäftsdaten in Vorlagen mit JavaScript integrieren"
      content: "Erstellen Sie ansprechende Berichte, indem Sie JSON, XML oder andere Daten in Vorlagen mit GroupDocs.Assembly for Node.js via Java einbetten."

    # feature loop
    - title: "Inhalt verwalten"
      content: "Füllen Sie automatisch Tabellen, Diagramme und andere visuelle Elemente in Ihren Dokumenten mit externen Daten aus."

    # feature loop
    - title: "Anpassbare Optionen"
      content: "GroupDocs.Assembly for Node.js via Java ermöglicht es Ihnen, Funktionen wie Barcodes hinzuzufügen, Daten von URLs abzurufen und Dateien in verschiedenen Formaten zu exportieren."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Assembly for Node.js via Java integriert sich nahtlos mit führenden Betriebssystemen, Frameworks und Paketmanagern."
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
    GroupDocs.Assembly for Node.js via Java unterstützt eine Vielzahl von [Dokumentenformaten](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "Kernfunktionen von GroupDocs.Assembly"
  description: "Erstellen Sie dynamische Dokumente und Berichte mit leistungsstarken Datenmanagement-Tools."

  items:
    # feature loop
    - icon: "preview"
      title: "Reiche Datenvisualisierungen"
      content: "Fügen Sie problemlos Diagramme, Tabellen, Bilder und Listen in Ihre Dokumente mit vollständiger Anpassung ein."

    # feature loop
    - icon: "manipulate"
      title: "Daten transformieren"
      content: "Nutzen Sie Tools wie Formeln und Sortierung, um Informationen effektiv zu strukturieren und darzustellen."

    # feature loop
    - icon: "two_pages"
      title: "Breite Formatkompatibilität"
      content: "Arbeiten Sie nahtlos mit gängigen Dateiformaten für Vorlagen und Ausgaben."

    # feature loop
    - icon: "document_settings"
      title: "Erweiterte Vorlagenanpassung"
      content: "Formatieren Sie Vorlagen mit numerischen, alphabetischen und anderen Stiloptionen."

    # feature loop
    - icon: "text"
      title: "Dynamisches Generieren von Barcodes"
      content: "Erstellen und betten Sie Barcode-Bilder direkt nach Bedarf in Ihre Dokumente ein."

    # feature loop
    - icon: "add"
      title: "Flexible Textgestaltung"
      content: "Wenden Sie einfach Textstile wie Großschreibung oder Titel-Schreibung in Ihren Vorlagen an."

    # feature loop
    - icon: "manipulate"
      title: "Dynamische Inhaltsintegration"
      content: "Fügen Sie während der Dokumentenerstellung dynamisch Inhalte aus externen Dateien ein."

    # feature loop
    - icon: "convert"
      title: "Exportieren in verschiedene Formate"
      content: "Speichern Sie Dokumente in mehreren Formaten mit Ihren spezifizierten Konfigurationen."

    # feature loop
    - icon: "update"
      title: "Dynamisches Einbetten von Medien"
      content: "Fügen Sie Bilder oder andere Elemente mit Base64-Daten beim Erstellen von Dokumenten ein."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Entdecken Sie praktische Beispiele, wie Sie GroupDocs.Assembly für gängige Aufgaben nutzen können."
  items:
    # code sample loop
    - title: "Fügen Sie eine Aufzählungsliste in Word-Dokumente ein"
      content: |
        Erfahren Sie, wie Sie [aufgezählte Listen](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) in Word-Dokumenten erstellen, um Daten effektiv zu organisieren. Dieses Beispiel zeigt, wie Sie eine Aufzählungsliste mit GroupDocs.Assembly erstellen.
        {{< landing/code title="Fügen Sie eine Aufzählungsliste in Word-Dokumente ein">}}
        ```javascript {style=abap}
        // Fügen Sie diese Vorlage auf einer Dokumentseite ein:
        // Leistungsindikatoren der Manager
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Geben Sie den Vorlagenpfad an
        const template = "Bulleted List Template.docx";

        // Legen Sie den Ausgabedateipfad fest
        const result = "Result Report.docx"

        // Rufen Sie die Daten der Manager aus einer JSON-Quelle ab
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Generieren Sie den Bericht mit den ausgefüllten Daten
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Kreisdiagramme in PowerPoint einfügen"
      content: |
        Erfahren Sie, wie Sie Vorlagen und XML verwenden, um [Kreisdiagramme](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) in Ihren Präsentationen hinzuzufügen. Verbessern Sie Ihre Berichte mit Kreisdiagrammen, um Daten visuell und klar darzustellen.
        {{< landing/code title="Kreisdiagramme in PowerPoint einfügen">}}
        ```javascript {style=abap} 
        // Fügen Sie das Titel-Template für das Diagramm zur Präsentation hinzu:
        // Umsatz der Kunden <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Fügen Sie auch das Daten-Template für das Diagramm hinzu:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Geben Sie den Pfad zur Diagrammvorlage an
        const template = "Pie Chart Template.pptx";

        // Legen Sie den Ausgabedateipfad fest
        const result = "Result Report.pptx"

        // Rufen Sie die Kundendaten aus einer XML-Quelle ab
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Generieren Sie das Diagramm und speichern Sie das Ergebnis
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---