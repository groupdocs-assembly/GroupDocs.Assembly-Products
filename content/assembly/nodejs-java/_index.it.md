---
############################# Static ############################
layout: "landing"
date: 2025-01-16T13:04:06
draft: false

lang: it
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
head_title: "Toolkit Node.js per Creare, Automatizzare e Personalizzare Documenti"
head_description: "Libreria Node.js per l'automazione dei flussi documentali. Genera file PDF, Word, Excel, PowerPoint, HTML e email dai tuoi modelli."

############################# Header ############################
title: "API Node.js per l'Automazione Semplificata di Documenti e Report"
description: "Ottimizza la generazione di report JavaScript unendo i tuoi dati con modelli predefiniti."
words:
  for: "per"

actions:
  main: "Inizia la tua Prova su NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Pronto per Cominciare?"
  description: "Prova le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza."

release:
  title: "Versione {0} rilasciata"
  notes: "Scopri le novità"
  downloads: "Download"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Crea un Grafico in un Documento Word Utilizzando Node.js"
  more: "Ulteriori esempi"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Percorso del modello principale
    const template = "chart_template.docx";

    // Recupera i dati di produttività dei manager dalla fonte
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Crea un'istanza di DataSourceInfo con i dati
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Imposta i colori dei grafici utilizzando un altro DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Compila il modello con i dati e salvalo nell'output
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Assembly"
  description: "Una libreria Node.js progettata per creare documenti in modo programmatico con gestione dei dati integrata."
  features:
    # feature loop
    - title: "Integra Dati Aziendali nei Modelli con JavaScript"
      content: "Genera report professionali incorporando JSON, XML o altri dati nei modelli utilizzando GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Gestisci Contenuti Integrati"
      content: "Compila automaticamente tabelle, grafici e altre visualizzazioni nei tuoi documenti utilizzando dati esterni."

    # feature loop
    - title: "Opzioni Personalizzabili"
      content: "GroupDocs.Assembly for Node.js via Java ti consente di aggiungere funzionalità come codici a barre, recupero dati da URL e esportazione di file in vari formati."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Assembly for Node.js via Java si integra perfettamente con i principali sistemi operativi, framework e gestori di pacchetti."
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
  title: "Formati di file supportati"
  description: |
    GroupDocs.Assembly for Node.js via Java supporta un'ampia gamma di [formati documentali](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "Caratteristiche Principali di GroupDocs.Assembly"
  description: "Crea documenti e report dinamici con potenti strumenti di gestione dei dati."

  items:
    # feature loop
    - icon: "preview"
      title: "Visualizzazioni Dati Ricche"
      content: "Inserisci grafici, tabelle, immagini e elenchi nei tuoi documenti con piena personalizzazione."

    # feature loop
    - icon: "manipulate"
      title: "Trasforma i Tuoi Dati"
      content: "Sfrutta strumenti come formule e ordinamenti per strutturare e visualizzare le informazioni in modo efficace."

    # feature loop
    - icon: "two_pages"
      title: "Ampia Compatibilità con i Formati"
      content: "Lavora senza soluzione di continuità con i formati di file più diffusi per modelli e output."

    # feature loop
    - icon: "document_settings"
      title: "Personalizzazione Avanzata dei Modelli"
      content: "Formatta i modelli con opzioni di stile numeriche, alfabetiche e altre."

    # feature loop
    - icon: "text"
      title: "Generazione Dinamica di Codici a Barre"
      content: "Crea e incorpora immagini di codici a barre direttamente nei tuoi documenti su richiesta."

    # feature loop
    - icon: "add"
      title: "Stile del Testo Flessibile"
      content: "Applica facilmente stili di testo come maiuscole o maiuscole iniziali nei tuoi modelli."

    # feature loop
    - icon: "manipulate"
      title: "Inserimento Dinamico di Contenuti"
      content: "Include contenuti da file esterni dinamicamente durante la generazione di documenti."

    # feature loop
    - icon: "convert"
      title: "Esporta in Vari Formati"
      content: "Salva documenti in più formati con le configurazioni specificate."

    # feature loop
    - icon: "update"
      title: "Incorpora Media Dinamicamente"
      content: "Inserisci immagini o altri elementi utilizzando dati Base64 durante la creazione dei documenti."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Scopri esempi pratici su come utilizzare GroupDocs.Assembly per compiti comuni."
  items:
    # code sample loop
    - title: "Aggiungi un Elenco Puntato nei Documenti Word"
      content: |
        Vedi come creare [elenchi puntati](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) nei documenti Word per organizzare i dati in modo efficace. Questo esempio dimostra come generare un elenco puntato utilizzando GroupDocs.Assembly.
        {{< landing/code title="Aggiungi un Elenco Puntato nei Documenti Word">}}
        ```javascript {style=abap}
        // Inserisci questo modello in una pagina del documento:
        // Indicatori di prestazione dei manager
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specifica il percorso del modello
        const template = "Bulleted List Template.docx";

        // Imposta il percorso del file di output
        const result = "Result Report.docx"

        // Recupera i dati dei manager da una fonte JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Genera il report con i dati completati
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Inserisci Grafici a Torta in PowerPoint"
      content: |
        Scopri come utilizzare modelli e XML per aggiungere [grafici a torta](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) nelle tue presentazioni. Migliora i tuoi report con grafici a torta per presentare visivamente e chiaramente i dati.
        {{< landing/code title="Inserisci Grafici a Torta in PowerPoint">}}
        ```javascript {style=abap} 
        // Aggiungi il modello del titolo del grafico alla presentazione:
        // Fatturato dei clienti <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Includi anche il modello del dato del grafico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specifica il percorso del modello del grafico
        const template = "Pie Chart Template.pptx";

        // Imposta il percorso del file di output
        const result = "Result Report.pptx"

        // Recupera i dati dei clienti da una fonte XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Genera il grafico e salva il risultato
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---