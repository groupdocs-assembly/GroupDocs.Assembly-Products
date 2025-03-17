---
############################# Static ############################
layout: "family"
date:  2025-03-17T13:11:11
draft: false

product: "Assembly"
product_tag: "assembly"

lang: de

############################# Head ############################
head_title: ".NET, Java, Node.js APIs & Online-Dokumentenerstellungsanwendungen von GroupDocs"
head_description: "Erhalten Sie eine umfassende Dokumentenautomatisierungs- und Reporting-Lösung für .NET-, Java- und Node.js-Anwendungen. Generieren Sie alle gängigen Dokumente aus benutzerdefinierten Vorlagen und Daten."

############################# Header ############################
title: "Dokumentautomatisierung und Berichterstattungslösung"
description:  |
  Erstellen Sie detaillierte Berichte mit Vorlagen und Datenquellen mit unseren plattformübergreifenden Apps und APIs.

  Generieren Sie Berichte in Formaten wie Word, Excel, Präsentationen und vielen weiteren mithilfe von Vorlagen mit flexibel einstellbarem Markup.

  Füllen Sie Diagramme, Barcodes, Tabellen und andere Elemente mit Daten aus Quellen wie JSON, XML, CSV usw. aus.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Wählen Sie Ihre Plattform"
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Assembly ist mit den folgenden Betriebssystemen und Frameworks kompatibel:"
  details_link_title: "Erfahren Sie mehr"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Assembly Hauptmerkmale"
  description: "Diese Lösung hilft Ihnen, Berichte in gängigen Dokumentformaten zu erstellen, die automatisch mit Ihren Geschäftsdaten gefüllt werden. Automatisieren Sie Ihre Dokumentgenerierungsaufgaben."

  items:
    # items loop
    - icon: "additional"
      title: "Vorlagen mit Daten füllen"
      content: "Füllen Sie Berichte mit Daten aus unterstützten Quellen."

    # items loop
    - icon: "manipulate"
      title: "Flexibles Markup"
      content: "Fügen Sie Daten auf anpassbare Weise zu Dokumenten hinzu."

    # items loop
    - icon: "structure"
      title: "Native Dokumentfunktionen"
      content: "Stellen Sie Daten mit Tabellen, Diagrammen und Barcodes dar."

    # items loop
    - icon: "merge"
      title: "Alle gängigen Formate"
      content: "Unterstützt alle gängig verwendeten Dokumentformate."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Erstellen Sie gut angepasste Berichte"
  description: "GroupDocs.Assembly Codebeispiele"
  items:
    # code sample loop
    - title: "Verwendung von generierten Barcodes"
      content: |
       GroupDocs.Assembly ermöglicht Barcode-Markup in Berichtsvorlagen. Bei der Erstellung eines Berichts wird ein Barcode basierend auf dem Markup und den bereitgestellten Daten generiert. Geben Sie den Pfad zur Vorlage mit dem Text, den Datenobjekten und dem Markup an. Geben Sie auch die Datenquelle an, um den Barcode mit Inhalten zu füllen.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Erstellen Sie eine Instanz der DocumentAssembler-Klasse
            DocumentAssembler assembler = new DocumentAssembler();

            //Geben Sie den Pfad zur Vorlage an
            var tmp_path = "barcode_template.docx";

            //Geben Sie den Pfad zum Ergebnissdokument an
            var res_path = "result.docx";

            //Erstellen Sie eine Instanz der Datenquelle
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Rufen Sie AssembleDocument auf, um den Bericht zu erstellen
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Erstellen Sie eine Instanz der DocumentAssembler-Klasse
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Geben Sie den Pfad zur Vorlage an
            String tmp_path = "barcode_template.docx";

            //Geben Sie den Pfad zum Ergebnissdokument an
            String res_path = "result.docx";

            //Erstellen Sie eine Instanz der Datenquelle
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Rufen Sie AssembleDocument auf, um den Bericht zu erstellen
            assembler.assembleDocument(tmp_path, res_path, data);

            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Unterstützt über 50 Dateiformate"
  description: "GroupDocs.Assembly arbeitet mit nahezu allen gängigen Dateiformaten."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Unsere Produktstatistiken"
  description: "Entdecken Sie Produktmetriken, um Einblicke in unseren Fortschritt, Einfluss und Wachstum zu gewinnen."

  items:
    # items loop
    - number: "50+"
      title: "Unterstützte Formate"
      content: "Wir unterstützen über 50 der am weitesten verbreiteten Dokumentformate."

    # items loop
    - number: "650k"
      title: "NuGet-Downloads"
      content: "GroupDocs.Assembly für .NET ist eine beliebte Bibliothek mit über 650.000 Downloads auf NuGet."

    # items loop
    - number: "18k"
      title: "Maven-Downloads"
      content: "Java-Entwickler haben GroupDocs.Assembly auf Maven über 18.000 Mal heruntergeladen."

    # items loop
    - number: "150+"
      title: "Zufriedene Kunden"
      content: "Unsere Produkte werden von einzelnen Entwicklern und führenden Unternehmen weltweit verwendet, um innovative Lösungen zu erstellen."


############################# Customers ###############################
customers:
  enable: true
  title: "Unsere zufriedenen Kunden"
  description: "Die GroupDocs-Bibliotheken werden von einigen der renommiertesten und angesehensten Marken weltweit verwendet."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Assembly kostenlos auf Ihrer Plattform."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Häufig gestellte Fragen"
  description: "Durchsuchen Sie unsere häufig gestellten Fragen."

  items:
    # items loop
    - question: "Benötigt GroupDocs.Assembly externe Bibliotheken für die Dokumentenerstellung?"
      answer: "Nein, GroupDocs.Assembly arbeitet unabhängig und benötigt keine Drittanbieter-Bibliotheken wie Adobe Acrobat oder Microsoft Office."

    # items loop
    - question: "Kann ich die Funktionen von GroupDocs.Assembly vor dem Kauf testen?"
      answer: "Ja, können Sie! GroupDocs.Assembly bietet eine kostenlose Testversion. Installieren Sie es und erkunden Sie seine Funktionen. Die Testversion fügt 'Testabzeichen' zu Ihren Dokumenten hinzu und verarbeitet nur die ersten 3 Seiten. Um die vollständige Erfahrung zu machen, erhalten Sie eine kostenlose 30-tägige Testlizenz, um alle Funktionen zu nutzen. Weitere Informationen finden Sie unter [temporäre Lizenz](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Welche Arten von Lizenzen sind verfügbar?"
      answer: "Suchen Sie eine GroupDocs.Assembly-Lizenz? Wir bieten eine Vielzahl von Optionen, die Ihren Bedürfnissen entsprechen. Wählen Sie basierend auf der Teamgröße, dem Bereitstellungsort (einzelnes Büro oder remote) und ob Sie das SDK/API mit Kunden zur Verteilung teilen müssen. Alternativ können Sie eine monatliche Nutzungslizenz mit verbrauchsabhängigen Plänen wählen – zahlen Sie nur für das, was Sie verwenden. Finden Sie die beste Option für Sie unter [Preise](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Assembly Low-Code APIs"
  description: "Generieren Sie Dokumente über unsere cloudbasierten REST-API aus Ihrer Anwendung."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Verwenden Sie die cURL RESTful API, um Daten zu Word, Excel, PowerPoint und vielen anderen Vorlagen hinzuzufügen."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Verbessern Sie Ihre .NET-Anwendungen, indem Sie Berichte über das Cloud SDK generieren. Stellen Sie Geschäftsdaten in Ihrem benutzerdefinierten Format dar."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK bietet verschiedene Optionen für Java-Anwendungen zur Erstellung verschiedener Dokumenttypen."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Assembly Web Apps"
  description: "GroupDocs.Assembly bietet eine kostenlose Webanwendung zum Generieren von Dokumenten. Sie können über 50 gängige Dateiformate direkt in Ihrem Browser kostenlos verarbeiten."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Generieren Sie Berichte in Excel, Word, PowerPoint und vielen anderen Dateitypen direkt aus Ihrem Webbrowser."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Erstellen Sie Microsoft Word-Dokumente aus Vorlagen und Datenquellen."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Laden Sie eine Vorlage und eine Datenquelle hoch, um Excel-Berichte kostenlos zu generieren."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---