---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: it
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
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Libreria Java per Creazione Documentale, Automazione e Reporting"
head_description: "Libreria Java per l'automazione della creazione di documenti e generazione di report. Crea documenti PDF, Word, Excel, PPTX, HTML e email utilizzando modelli personalizzati."

############################# Header ############################
title: "API Java per Automazione di Report e Documenti"
description: "Semplifica la generazione di report in Java unendo dati con modelli."
words:
  for: "per"

actions:
  main: "Richiedi Trial tramite Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Pronto per Cominciare?"
  description: "Prova le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza."

release:
  title: "Versione {0} rilasciata"
  notes: "Scopri le novità"
  downloads: "Download"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Genera un Grafico in DOCX con Java"
  more: "Ulteriori esempi"
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
    // Percorso del modello principale
    String template = "chart_template.docx";

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
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Assembly"
  description: "Una libreria Java progettata per la creazione automatica di documenti e l'integrazione dati semplificata."
  features:
    # feature loop
    - title: "Unisci Dati Aziendali ai Modelli con Java"
      content: "Crea facilmente report professionali incorporando dati da JSON, XML o altre fonti in modelli preprogettati utilizzando GroupDocs.Assembly for Java."

    # feature loop
    - title: "Lavora con Oggetti Incorporati"
      content: "Popola automaticamente elementi come tabelle, grafici e diagrammi nei documenti utilizzando dati provenienti da fonti esterne."

    # feature loop
    - title: "Personalizzazione Avanzata"
      content: "GroupDocs.Assembly for Java offre funzionalità flessibili come la generazione di codici a barre, l'acquisizione di dati online tramite URL e l'esportazione di output in diversi formati."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Assembly for Java funziona senza soluzione di continuità con sistemi operativi, framework di sviluppo e gestori di pacchetti popolari."
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
    GroupDocs.Assembly for Java supporta un'ampia gamma di [formati documentali](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Capacità Chiave di GroupDocs.Assembly"
  description: "Crea documenti e report professionali con gestione dati avanzata."

  items:
    # feature loop
    - icon: "preview"
      title: "Elementi Dati Visivi"
      content: "Aggiungi e formatta elementi come grafici, tabelle, immagini ed elenchi direttamente nei tuoi documenti."

    # feature loop
    - icon: "manipulate"
      title: "Trasformazione dei Dati"
      content: "Utilizza formule, ordinamenti e altri strumenti per organizzare e presentare i tuoi dati in modo efficace."

    # feature loop
    - icon: "two_pages"
      title: "Supporto per Formati Multipli"
      content: "Lavora facilmente con tipi di file comuni per modelli e file di output."

    # feature loop
    - icon: "document_settings"
      title: "Formattazione Avanzata del Modello"
      content: "Personalizza i modelli con opzioni di formattazione numerica, alfabetica e altre avanzate."

    # feature loop
    - icon: "text"
      title: "Generazione Dinamica di Codici a Barre"
      content: "Crea rapidamente e inserisci immagini di codici a barre nei documenti secondo necessità."

    # feature loop
    - icon: "add"
      title: "Formattazione Flessibile del Testo"
      content: "Applica trasformazioni di testo come maiuscolo, minuscolo, maiuscolo per la prima lettera o altri stili nei modelli."

    # feature loop
    - icon: "manipulate"
      title: "Importa Contenuti Esterni"
      content: "Incorpora dinamicamente contenuti da file esterni mentre generi i documenti."

    # feature loop
    - icon: "convert"
      title: "Esporta in Formati Multipli"
      content: "Salva i documenti finali in vari formati di file utilizzando estensioni o configurazioni specifiche."

    # feature loop
    - icon: "update"
      title: "Incorporamento Dinamico dei Media"
      content: "Inserisci immagini o altri contenuti utilizzando dati codificati in Base64 durante la creazione del documento."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Esplora il codice di esempio per compiti comuni con GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Crea un Elenco Puntato in Word"
      content: |
        Scopri come aggiungere [elenchi puntati](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) ai documenti Word per una rappresentazione organizzata dei dati. Questo esempio mostra come generare un elenco in Word utilizzando GroupDocs.Assembly.
        {{< landing/code title="Crea un Elenco Puntato in Word">}}
        ```java {style=abap}
        // Inserisci questo modello in una pagina del documento:
        // Indicatori di prestazione dei manager
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Specifica il percorso del modello
        String template = "Bulleted List Template.docx";

        // Imposta il percorso del file di output
        String result = "Result Report.docx"

        // Recupera i dati dei manager da una fonte JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Genera il report con i dati completati
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Crea Grafici a Torta in PPTX"
      content: |
        Utilizza modelli e XML per aggiungere [grafici a torta](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) alle tue presentazioni. Rendi i tuoi report più coinvolgenti includendo grafici a torta per visualizzare i dati.
        {{< landing/code title="Crea Grafici a Torta in PPTX">}}
        ```java {style=abap}   
        // Aggiungi il modello del titolo del grafico alla presentazione:
        // Fatturato dei clienti <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Includi anche il modello del dato del grafico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Specifica il percorso del modello del grafico
        String template = "Pie Chart Template.pptx";

        // Imposta il percorso del file di output
        String result = "Result Report.pptx"

        // Recupera i dati dei clienti da una fonte XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Genera il grafico e salva il risultato
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---