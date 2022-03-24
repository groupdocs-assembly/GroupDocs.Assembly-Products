---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET-API für Dokumentenautomatisierung, Zusammenstellung und Berichterstellung"
head_description: "C# .NET API für Dokumentenautomatisierung, Assemblierung und Generierung von Berichten. Erstellen Sie PDF-, Word-, Excel-, PPTX-, HTML- und E-Mail-Dokumente aus benutzerdefinierten Vorlagen."

############################# Header ############################
title: ".NET-Dokumentautomatisierungs- und Berichterstellungs-API"
description: "Generieren Sie Berichte in .NET-Anwendungen, indem Sie Vorlagen definieren und die Daten zusammenführen."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "/border/groupdocs-assembly-net.svg"
        product: "GroupDocs.Assembly"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Überblick ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly für die .NET-API unterstützt Sie beim Erstellen leistungsstarker Dokumentenautomatisierungs- und Berichterstellungsanwendungen mit Funktionen zum Generieren von Berichten aus benutzerdefinierten Vorlagen in C#, ASP.NET und anderen .NET-bezogenen Anwendungen. Mit nur wenigen Codezeilen stellt die .NET-Berichtsbibliothek die angegebenen Daten intelligent aus der definierten Dokumentvorlage zusammen und generiert ansprechende Berichte im bevorzugten Ausgabeformat, indem sie Daten aus verschiedenen Datenquellen (Datenbanken, XML, JSON, ODATA, CSV, Benutzerdefinierte .NET-Objekte).

      Es unterstützt die LINQ-basierte Vorlagensyntax, und Benutzer können problemlos Ausgabedokumente in allen gängigen Geschäftsdateiformaten wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblättern, PowerPoint-Präsentationen und Folien erstellen. Formatierungseigenschaften für Vorlagenelemente können auch durch Bearbeiten von Text, HTML- und Bedingungsblöcken, Bildern, Diagrammen, Barcodes, Hyperlinks, Pivot-Tabellen usw. konfiguriert werden.

      GroupDocs.Assembly für .NET kann verwendet werden, um Anwendungen in jeder Entwicklungsumgebung zu entwickeln, die auf die .NET-Plattform abzielt. Es ist mit allen .NET-basierten Sprachen kompatibel und unterstützt gängige Betriebssysteme (Windows, Linux, MacOS), auf denen Mono- oder .NET-Frameworks (einschließlich .NET Core) installiert werden können.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Nachfolgend finden Sie eine Übersicht über GroupDocs.Assembly für .NET:
      
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
          Unterstützte [Dokumentdateiformate](https://docs.groupdocs.com/assembly/net/supported-document-formats/) für die .NET-Dokumentgenerierungs-API sind unten aufgeführt.

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
          GroupDocs.Assembly for .NET unterstützt das Folgen Betriebssysteme, Frameworks & Paket-Managers:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * .NET Framework 2.0 oder höher
                * Mono Framework 1.2 oder höher

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Paket-Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entwicklungsumgebungen"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Merkmale ############################
features:
    enable: true
    title: "GroupDocs.Assembly für .NET-Funktionen"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Funktioniert mit mehreren Datenformaten"

      # feature loop
      - icon: "fas fa-eye"
        content: "Kann Daten mithilfe von Formeln und sequentiellen Datenoperationen manipulieren"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Formatieren Sie Zeichenfolgen in der Vorlagensyntax so, dass sie Upper, Lower, Capital, FirstCap sind"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Führen Sie die ordinale, kardinale und alphabetische numerische Formatierung in der Vorlagensyntax durch"

      # feature loop
      - icon: "fas fa-code"
        content: "Definieren Sie Variablen in Vorlagendokumenten und unterstützen Sie Textkommentare in Vorlagensyntax-Tags"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Inhalte äußerer Dokumente dynamisch in Ihre Berichte einfügen"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Barcode-Bild dynamisch in Berichten generieren und Hintergrundfarbe für HTML-Dokumente festlegen"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Weisen Sie dem E-Mail-Nachrichtentext dynamisch Attribute zu und fügen Sie Hyperlinks in Berichte ein"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "E-Mail-Nachrichtenanhänge dynamisch erstellen"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Unterstützung für analoges NEXT-Feld von Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Felder beim Zusammenstellen von Textverarbeitungsdokumenten aktualisieren"

      # feature loop
      - icon: "fas fa-columns"
        content: "Berechnen Sie die Formel beim Zusammenstellen von Tabellenkalkulationsdokumenten"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Format Numerisch, Text, Bild, Diagramm, Datum-Uhrzeit-Elemente der Vorlage"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Laden und Speichern von zusammengesetzten POT- und OTP-Präsentationsdokumentformaten"

      # feature loop
      - icon: "fas fa-print"
        content: "Verwenden Sie die LINQ-basierte Syntax für Vorlagen und führen Sie eine bedingte Textformatierung von Vorlagenelementen durch"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Ändern Sie das Dateiformat des zusammengestellten Dokuments mithilfe der Dateierweiterung oder der expliziten Spezifikationen"

      # feature loop
      - icon: "fas fa-lock"
        content: "Geordnete Liste unterstützt für Markdown – Speichern Sie neu zusammengestellte E-Mails und Word-Dokumente in Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Unterstützt Berichte zahlreicher Typen, z. B. Diagramme, Listen, Tabellen, Bilder und mehr"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Inline-Vorlagensyntaxfehler in generierten Dokumenten anstelle von Ausnahmeauslösungen"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Laden Sie Vorlagendokumente aus HTML mit Ressourcen und speichern Sie zusammengesetzte Word-, Excel-, PowerPoint- und E-Mail-Dateien in HTML mit Ressourcen"

      # feature loop
      - icon: "fas fa-heading"
        content: "Fügen Sie die Nummerierung der Neustartliste dynamisch in Word-Dokumentformaten und E-Mails mit HTML- und RTF-Texten hinzu"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Dynamisches Einfügen von Bildern und Dokumenten aus Base64-codierten Bytes and adjust checkbox value settings of Word documents"

      # feature loop
      - icon: "fas fa-cube"
        content: "Strecken Sie das Bild in Textfeldern von Word, Excel, Präsentationen und E-Mails, während Sie das Bildverhältnis beibehalten"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Fügen Sie dynamisch Links und Lesezeichen zu Dokumentformaten hinzu und benennen Sie die Zellbereiche von Excel-Tabellen"

    more_feature:
      # more_feature_loop
      - title: "Unterstützung für Vorlagenelemente"
        content: |
          GroupDocs.Assembly für die .NET-API gibt Ihnen die Kontrolle über die Arbeit mit zahlreichen Vorlagenelementen. Sie können mit formatierten Textblöcken, HTML-Blöcken, Bildern, Diagrammen, Hyperlinks und Barcodes (über Barcode-Schriftarten) arbeiten. Wiederholte Blöcke und bedingte Blöcke werden ebenfalls unterstützt, einschließlich Listenelementen und Tabellenzeilen. Sie können auch Tabellenzellen, die denselben Text enthalten, basierend auf Vorlagenausdrücken für Tabellenkalkulationen, Präsentationen, Dokumente und E-Mails mit HTML- und RTF-Textkörpern dynamisch zusammenführen.

      # more_feature_loop
      - title: "Arbeiten mit Listenberichten"
        content: |
          Mit GroupDocs.Assembly für die .NET-API können Sie mit Listenberichten der folgenden drei Typen arbeiten:

          * Liste mit Aufzählungszeichen
          * Nummerierte Liste
          * Colored Nummerierte Liste

      # more_feature_loop
      - title: "Arbeiten mit Diagrammberichten"
        content: |
          GroupDocs.Assembly für .NET unterstützt die folgenden Arten von Diagrammberichten:

          * Blasendiagramm, das drei Dimensionen von Daten anzeigt
          * Säulendiagramm
          * Kuchendiagramm
          * Streudiagramm
          * Seriendiagramm (farbig)

      # more_feature_loop
      - title: "Arbeiten mit Tabellenberichten"
        content: |
          GroupDocs.Assembly für .NET unterstützt die folgenden Arten von Tabellenberichten:

          * Master-Detail-Tabelle
          * Tabelle mit hervorgehobenen Zeilen
          * Tabelle mit alternativem Inhalt
          * Tabelle mit Filtern, Gruppieren und Ordnen
          
          Sie können Datenbänder auch in Tabellenzeilen verwenden.

      # more_feature_loop
      - title: "Einfache Integration"
        content: |
          Sie können GroupDocs.Assembly für die .NET-API mit nur wenigen Codezeilen problemlos in Ihre .NET-Anwendung integrieren. Es folgt ein Beispielcode zum Generieren eines Berichts in einem geöffneten Dokument format:

          ```cs
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
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
        - img_alt: "GroupDocs.Assembly for Java"
          image: "/border/groupdocs-assembly-java.svg"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
