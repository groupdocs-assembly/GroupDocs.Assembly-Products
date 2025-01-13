---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: it
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
head_title: "API .NET per Automazione Documentale, Assemblaggio e Generazione Report"
head_description: "API C# .NET per automazione documentale, assemblaggio e generazione di report. Crea documenti PDF, Word, Excel, PPTX, HTML e email da modelli personalizzati."

############################# Header ############################
title: "API di Automazione Documentale e Reporting per .NET"
description: "Genera report nelle applicazioni .NET definendo modelli e unendo dati."
words:
  for: "per"

actions:
  main: "Scarica il Trial tramite Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Pronto per Cominciare?"
  description: "Prova le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza."

release:
  title: "Versione {0} rilasciata"
  notes: "Scopri le novità"
  downloads: "Download"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Compila un Grafico in DOCX Utilizzando C#"
  more: "Ulteriori esempi"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Percorso del modello principale
    string template = "chart_template.docx";

    // Recupera i dati di produttività dei manager dalla fonte
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Crea un'istanza di DataSourceInfo con i dati
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Imposta i colori dei grafici utilizzando un altro DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Compila il modello con i dati e salvalo nell'output
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Assembly"
  description: "Soluzione .NET per automatizzare la creazione di documenti con integrazione dati avanzata."
  features:
    # feature loop
    - title: "Aggiungi Dati Aziendali ai Modelli di Documento con C#"
      content: "Generazione di report semplificata: con GroupDocs.Assembly for .NET, puoi facilmente inserire dati da fonti come JSON o XML in modelli predefiniti."

    # feature loop
    - title: "Elaborazione di Oggetti Dati Nativi"
      content: "I tipi di documenti supportati includono oggetti incorporati come diagrammi, grafici, tabelle e elenchi che possono essere popolati automaticamente con i dati."

    # feature loop
    - title: "Funzionalità Aggiuntive"
      content: "GroupDocs.Assembly for .NET fornisce ampie opzioni di personalizzazione. Progetta oggetti dati programmaticamente, genera codici a barre, utilizza fonti di dati online tramite URL e salva output in vari formati."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Assembly for .NET è compatibile con i seguenti sistemi operativi, framework e gestori di pacchetti."
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
  title: "Formati di file supportati"
  description: |
    GroupDocs.Assembly for .NET può elaborare i seguenti [formati di file](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formati Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Immagini e Altri Formati
        * **Portabile:** PDF
        * **Immagini:** SVG, TIFF
        * **Altri formati di ufficio:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Altri formati
        * **Web:** HTML, MHTML
        * **Email:** EML, MSG, EMLX
        * **Altro:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Caratteristiche di GroupDocs.Assembly"
  description: "Crea documenti e report utilizzando modelli di dati avanzati."

  items:
    # feature loop
    - icon: "preview"
      title: "Rappresentazione Avanzata dei Dati"
      content: "Supporta un'ampia gamma di oggetti dati come grafici, elenchi, tabelle, immagini e altro."

    # feature loop
    - icon: "manipulate"
      title: "Manipolazione dei Dati"
      content: "Applica formule e operazioni sequenziali per formattare e visualizzare i dati in modo efficace."

    # feature loop
    - icon: "two_pages"
      title: "Ampia Gamma di Formati Supportati"
      content: "Lavora senza soluzione di continuità con tutti i formati di documento comuni per modelli o file di output."

    # feature loop
    - icon: "document_settings"
      title: "Markup Ricco del Modello"
      content: "Sfrutta la formattazione numerica ordinale, cardinale e alfabetica nei modelli."

    # feature loop
    - icon: "text"
      title: "Incorpora Codici a Barre"
      content: "Genera immagini di codici a barre dinamicamente e inseriscile nei tuoi documenti."

    # feature loop
    - icon: "add"
      title: "Formattazione dei Dati"
      content: "Formatta le stringhe nei modelli in maiuscolo, minuscolo, maiuscolo iniziale o stili con prima lettera maiuscola."

    # feature loop
    - icon: "manipulate"
      title: "Manipolazione dei Contenuti Documentali"
      content: "Inserisci dinamicamente contenuti da documenti esterni nei tuoi report."

    # feature loop
    - icon: "convert"
      title: "Salva in Formati Multipli"
      content: "Specifica il formato del file di output utilizzando estensioni di file o configurazioni dettagliate."

    # feature loop
    - icon: "update"
      title: "Elaborazione Dati Flessibile"
      content: "Inserisci immagini e documenti dinamicamente utilizzando byte codificati in Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Esempi di codice per operazioni tipiche di GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Elenco Puntato in un Documento Microsoft Word"
      content: |
        [Elenchi puntati](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) sono un modo comune per presentare i dati aziendali. Ecco un esempio di come aggiungere un elenco a un documento Word utilizzando GroupDocs.Assembly.
        {{< landing/code title="Come Popolare un Elenco nei Documenti">}}
        ```csharp {style=abap}
        // Inserisci questo modello in una pagina del documento:
        // Indicatori di prestazione dei manager
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Specifica il percorso del modello
        string template = "Bulleted List Template.docx";

        // Imposta il percorso del file di output
        string result = "Result Report.docx"

        // Recupera i dati dei manager da una fonte JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Genera il report con i dati completati
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Grafici a Torta in Presentazioni PPTX"
      content: |
        Puoi creare [Grafici a Torta](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) utilizzando modelli e dati XML. Migliora i tuoi report con rappresentazioni grafiche dei dati visivamente accattivanti.
        {{< landing/code title="Come Rappresentare Dati in un Grafico a Torta">}}
        ```csharp {style=abap}
        // Aggiungi il modello del titolo del grafico alla presentazione:
        // Fatturato dei clienti <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Includi anche il modello del dato del grafico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Specifica il percorso del modello del grafico
        string template = "Pie Chart Template.pptx";

        // Imposta il percorso del file di output
        string result = "Result Report.pptx"

        // Recupera i dati dei clienti da una fonte XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Genera il grafico e salva il risultato
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---