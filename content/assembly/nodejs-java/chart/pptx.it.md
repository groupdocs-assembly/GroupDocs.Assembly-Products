



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:00
draft: false
lang: it
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Inserisci grafici nei file PPTX con JavaScript"
head_description: "Con GroupDocs.Assembly for Node.js via Java, gli sviluppatori possono creare e incorporare rapidamente grafici dinamici nei documenti utilizzando fonti di dati live."

############################# Header ############################
title: "Aggiungi grafici ai file PPTX utilizzando Node.js" 
description: "GroupDocs.Assembly for Node.js via Java semplifica il processo di integrazione dei grafici nei documenti PPTX con input di dati in tempo reale."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inizia gratis oggi"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica di GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) è una soluzione robusta per la creazione di documenti e report automatizzati. Aggiungi grafici, tabelle, immagini, codici a barre e liste ai file con precisione e senza difficoltà. Questa piattaforma versatile supporta oltre 50 formati, inclusi PDF, documenti Office e email.

############################# Steps ############################
steps:
    enable: true
    title: "Passi per aggiungere un grafico a un documento PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) rende aggiungere grafici ai file PPTX semplice. Scegli tra tipi di grafici come grafici a barre, a linee o a torta.
      
      1. Progetta un modello PPTX con segnaposto per i grafici.
      2. Carica dati da una fonte supportata.
      3. Configura le opzioni del grafico, inclusi tipo, colori e etichette.
      4. Esporta il documento con il grafico incorporato.
   
    code:
      platform: "java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento di esempio"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Includi questo tag nel tuo modello per generare un grafico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specifica il percorso del file modello
        const template = "chart_template.pptx";

        // Estrai dati dal tuo sistema sorgente
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Salva il documento finale con il grafico incorporato
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Incorpora grafici senza sforzo nei tuoi documenti"
  description: "GroupDocs.Assembly for Node.js via Java rende semplice generare documenti ricchi di funzionalità nei formati di file più diffusi. Usa modelli per aggiungere grafici, tabelle, codici a barre, liste, immagini e altro con aggiornamenti dei dati in tempo reale."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Trasforma i dati in grafici professionali"
      content: "Converti dati provenienti da sorgenti come JSON, XML o CSV in grafici di alta qualità che possono essere incorporati direttamente nei documenti."

    # feature loop
    - title: "Crea visualizzazioni straordinarie"
      content: "Genera grafici a barre, grafici a torta e grafici a linee che funzionano perfettamente con altri elementi del documento come immagini, tabelle e codici a barre."

    # feature loop
    - title: "Stilizzazione e posizionamento flessibili dei grafici"
      content: "Utilizza modelli LINQ per controllare il posizionamento e la stilizzazione dei grafici, inclusi colori, layout e etichette, per una presentazione curata."

    # feature loop
    - title: "Supporta molti formati di file"
      content: "Genera documenti in formati come MS Office, PDF, OpenOffice e HTML, con grafici perfettamente integrati per un risultato professionale."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Genera e inserisci grafici dinamicamente"
      content: |
        Questo esempio illustra come creare e incorporare grafici nei file PPTX programmaticamente.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Imposta un modello con un segnaposto per il grafico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Definisci il percorso del file modello
          const template = "table_template.pptx";

          // Recupera dati da una sorgente scelta
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Prepara un oggetto dati contenente le informazioni sul grafico
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Scegli il tipo di grafico e personalizza il suo aspetto
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Inizializza DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salva il documento aggiornato con il grafico incorporato
          asm.assembleDocument(template, "result.pptx", data, design);
          ```
        platform: "java"
        copy_title: "Copia"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica il risultato"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.pptx"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Esplora le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Scarica da NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Scopri di più sulle licenze"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Scopri funzionalità avanzate"
    exclude: "chart"
    description: "Questa piattaforma semplifica la creazione di documenti con strumenti progettati per la visualizzazione dei dati e integrazione fluida."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Genera report in più formati di file"
    exclude: "PPTX"
    description: "Node.js via Java supporta oltre 50 formati, facilitando la combinazione di modelli con dati per produrre documenti rifiniti."
    items: 
          
        # format loop 1
        - name: "Grafici in PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Grafici in DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Grafici in PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Grafici in XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---