---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Automation Assembly & Dynamic Reports Generator-API"
head_description: "Java-API für Dokumentenautomatisierung, Zusammenstellung und Berichterstellung. Erstellen Sie Berichte aus benutzerdefinierten Vorlagen. Stellen Sie PDF Word Excel PPTX HTML aus DB-, JSON-, OData- und XML-Datenquellen zusammen."

############################# Header ############################
title: "Java-API zur Automatisierung von Dokumenten und Berichten"
description: "Erstellen Sie Dokumentenautomatisierungsanwendungen zum Abrufen von Daten; Fügen Sie es in anpassbare Vorlagen ein und generieren Sie dynamische Berichte über die Java-API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "/border/groupdocs-assembly-java.svg"
        product: "GroupDocs.Assembly"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Überblick"

            # button loop
            - link: "#features"
              text: "Merkmale"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/assembly"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Überblick ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java API unterstützt Sie bei der schnellen Entwicklung von Dokumentenautomatisierungs- und Berichterstellungsanwendungen in Java, um benutzerdefinierte Berichte aus Vorlagen zu generieren, ohne externe Software installieren zu müssen. Die Berichterstellungs-Engine ruft Daten aus dem Vorlagendokument ab, stellt sie zusammen und generiert Berichte im angegebenen Ausgabeformat gemäß der definierten Syntax. Es ermöglicht Ihnen, Formatierungseigenschaften von Vorlagenelementen dynamisch zu konfigurieren und einzufügen und unterstützt verschiedene Datenquellen (JSON, XML, OData, Datenbanken, CSV, Tabellenkalkulation als Datentabelle, Textverarbeitungstabelle als Datentabelle und Datenbanken), um Daten abzurufen.

      Die Dokumentzusammenstellungsbibliothek erkennt mehrere Dokumentformate und ermöglicht Ihnen das Erstellen von Vorlagen in allen unterstützten Dateitypen wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblättern, PowerPoint-Präsentationen und Text. Es unterstützt LINQ-basierte Vorlagensyntax und Benutzer können auch Formatierungseigenschaften von Vorlagenelementen dynamisch konfigurieren und einfügen.

      GroupDocs.Assembly für Java lässt sich einfach in neue oder bestehende Java-Anwendungen integrieren. Es ist hochkompatibel mit allen Java-Versionen und unterstützt gängige Betriebssysteme (Windows, Linux, MacOS), die Java-Runtime ausführen können.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Nachfolgend finden Sie eine Übersicht über GroupDocs.Assembly für Java:

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Überblick"
          content: |
            * Datenformulierung
            * Datenformatierung
            * Datenautomatisierung
            * Vorlage erstellen
            * Formatierung von Vorlagenelementen
            * Berichterstellung
      
      ## TAB TWO ##
      tab_two:
        description: |
          Unterstützte [Dokumentdateiformate](https://docs.groupdocs.com/assembly/java/supported-document-formats/) für die Java-Dokumentgenerierungs-API sind unten aufgeführt.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office-Formate"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            # table loop
            - title: "Unterstützte Datenquellen"
              content: |
                * Datenbank
                * XML
                * OData
                * JSON
                * CSV
                * Benutzerdefinierte .NET-Objekte
                * Tabellenkalkulation als Datentabelle
                * Textverarbeitungstabelle als Datentabelle

        right:
          enable: true
          table:
            # table loop
            - title: "Andere Formate"
              content: |
                * **OpenOffice Document Formats**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **Markdown Dokumentation File**: MD
                * **Other**: TXT

            # table loop
            - title: "Unterstützung für Formatübergreifende Assemblierungen"
              content: |
                * Word Processing **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Spreadsheet **TO** Spreadsheet, HTML, PDF, XPS, TIFF, MHTML
                * Presentation **TO** Presentation, HTML, PDF, XPS, TIFF
                * Email **TO** Word Processing, Email, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML & TXT **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Assembly for Java unterstützt das Folgen Betriebssysteme, Frameworks & Paket-Managers:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * Java 7 (1.7) und höher

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entwicklungsumgebungen"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build-Automatisierungstool"
              content: |
                * Maven

############################# Merkmale ############################
features:
    enable: true
    title: "GroupDocs.Assembly für Java-Funktionen"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Passen Sie das Bild im Textfeld von Word, Excel, Präsentationen und E-Mails an, während Sie das Bildverhältnis beibehalten"

      # feature loop
      - icon: "fas fa-eye"
        content: "Verwenden Sie Formeln und führen Sie sequentielle Datenoperationen durch - Wenden Sie die Formel während der Tabellenkalkulation an"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Wenden Sie die Formatierung Upper, Lower, Capital, FirstCap auf Zeichenfolgen in der Vorlagensyntax an"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Vorlagensyntax unterstützt die Formatierung von Ordinal-, Kardinal- und alphabetischer Numerik"

      # feature loop
      - icon: "fas fa-code"
        content: "Unterstützen Sie Vorlagendokumente mit benutzerdefinierten Variablen und Textkommentaren innerhalb von Vorlagensyntax-Tags"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Fügen Sie Dokumentinhalte dynamisch in den Bericht ein"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Konfigurieren Sie dynamisch die Hintergrundfarbe von HTML-Dokumenten und generieren Sie Barcodes in Berichten"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Fügen Sie dynamisch Hyperlinks in Berichte ein und wenden Sie Attribute auf den E-Mail-Nachrichtentext an"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Hängen Sie E-Mail-Anhänge dynamisch an und aktualisieren Sie Felder während der Zusammenstellung von Textverarbeitungsdokumenten"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Unterstützung von NEXT Field Analogue von Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Fügen Sie dynamisch Links und Lesezeichen zu Dokumentformaten hinzu und benennen Sie die Zellbereiche von Excel-Tabellen"

      # feature loop
      - icon: "fas fa-columns"
        content: "Laden und Speichern von zusammengesetzten POT- und OTP-Präsentationsdokumentformaten"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Vorlagenformatierung für numerische, Text-, Bild-, Datum-Uhrzeit-, Diagrammelemente"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Dynamisches Einfügen von Bildern und Dokumenten aus Base64-codierten Bytes"

      # feature loop
      - icon: "fas fa-print"
        content: "LINQ-basierte Vorlagensyntax"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Ändern Sie das Format der zusammengesetzten Datei mit expliziten Spezifikationen oder der Dateierweiterung"

      # feature loop
      - icon: "fas fa-lock"
        content: "Geordnete Liste unterstützt für Markdown – Speichern Sie neu zusammengestellte E-Mails und Word-Dokumente in Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Generieren Sie verschiedene Berichtstypen, z. B. Diagramme, Bilder, Tabellen, Listen und mehr"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Inline-Vorlagensyntaxfehler in generierten Dokumenten anstelle von Ausnahmeauslösungen"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Starten Sie dynamisch eine nummerierte Liste in Word-Dokumenten sowie E-Mails mit HTML- und RTF-Texten neu"

      # feature loop
      - icon: "fas fa-heading"
        content: "Unterstützung von Tabellen, Autolinks, Inline-Links und Bildern für zusammengesetzte Markdown-Dokumente"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Barcodes dynamisch generieren (GS1-128 AI 8102 Coupon Extended und UPCA & GS1 Databar Coupon"

      # feature loop
      - icon: "fas fa-cube"
        content: "Laden Sie Vorlagendokumente aus HTML mit Ressourcen und speichern Sie zusammengesetzte Word-, Excel-, PowerPoint- und E-Mail-Dateien in HTML mit Ressourcen"

    more_feature:
      # more_feature_loop
      - title: "Vorlagenelemente manipulieren"
        content: |
          Bearbeiten Sie zahlreiche Vorlagenelemente mit GroupDocs.Assembly für die Java-API. Zu den Vorlagenelementen, mit denen Sie arbeiten können, gehören Textblöcke, Bilder, Hyperlinks, HTML-Blöcke, Barcodes (über Barcode-Schriftarten) und Diagramme. Sie können auch wiederholte Blöcke und bedingte Blöcke für Listenelemente und Tabellenzeilen anwenden. Dynamisches Zusammenführen von Tabellenzellen mit demselben Text basierend auf Vorlagenausdrücken für Dokumente, Präsentationen, Tabellenkalkulationen und E-Mails mit HTML- und RTF-Bodys.
      
      # more_feature_loop
      - title: "Listenberichte manipulieren"
        content: |
          Die Verwendung von GroupDocs.Assembly für die Java-API unterstützt die folgenden Arten von Listenberichten:

          * Liste mit Aufzählungszeichen
          * Nummerierte Liste
          * Colored Nummerierte Liste

      # more_feature_loop
      - title: "Diagrammberichte manipulieren"
        content: |
          GroupDocs.Assembly für Java unterstützt die folgenden Arten von Diagrammberichten:

          * Blasendiagramm, das drei Dimensionen von Daten anzeigt
          * Säulendiagramm
          * Kuchendiagramm
          * Streudiagramm
          * Seriendiagramm (farbig)

      # more_feature_loop
      - title: "Tabellenberichte manipulieren"
        content: |
          GroupDocs.Assembly für Java unterstützt die folgenden Arten von Tabellenberichten:

          * Master-Detail-Tabelle
          * Tabelle mit hervorgehobenen Zeilen
          * Tabelle mit alternativem Inhalt
          * Tabelle mit Filtern, Gruppieren und Ordnen

          Sie können Datenbänder auch in Tabellenzeilen verwenden.

      # more_feature_loop
      - title: "Diagrammberichte manipulieren"
        content: |
          Die Integration von GroupDocs.Assembly for Java API in Ihre Java-Anwendung ist wie ein Kinderspiel. Es folgt ein Beispielcodeblock, der einen Bericht im OpenDocument-Format mit Java generiert: 

          ```java
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Assembly bietet APIs zum Anzeigen von Dokumenten für andere beliebte Entwicklungsumgebungen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "/border/groupdocs-assembly-net.svg"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---