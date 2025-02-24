



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: it
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Inserisci tabelle nei documenti PPTX con JavaScript"
head_description: "Utilizza GroupDocs.Assembly for Node.js via Java per inserire rapidamente tabelle in documenti o e-mail, estraendo dati da diverse fonti."

############################# Header ############################
title: "Aggiungi tabelle ai file PPTX con Node.js" 
description: "Con GroupDocs.Assembly for Node.js via Java, riempire tabelle nei documenti PPTX è semplice, utilizzando dati da più fonti."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inizia la tua prova gratuita"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduzione a GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) è uno strumento potente per automatizzare la creazione di documenti. Ti consente di inserire tabelle, grafici, elenchi e immagini nei modelli, con posizionamento preciso del contenuto. Supportando oltre 50 formati di file, inclusi PDF, Word e e-mail, semplifica la generazione di report e altre attività.

############################# Steps ############################
steps:
    enable: true
    title: "Come aggiungere dati a una tabella in PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) ti consente di popolare rapidamente i modelli di tabella per file PPTX utilizzando sorgenti di dati dinamiche.
      
      1. Crea un modello PPTX con segnaposto per righe e colonne della tabella.
      2. Carica dati da una fonte supportata come JSON o CSV.
      3. Organizza e formatta i dati secondo necessità.
      4. Genera il documento con la tabella completata.
   
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
        // Includi questi tag nei segnaposto delle righe della tabella del tuo modello
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specifica il percorso del file modello
        const template = "table_template.pptx";

        // Carica i tuoi dati da una fonte scelta
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Salva il documento finale con la tabella completata
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Aggiungi tabelle basate su dati ai documenti"
  description: "GroupDocs.Assembly for Node.js via Java consente agli utenti di generare tabelle automaticamente, integrando anche grafici, immagini ed elenchi utilizzando flussi di lavoro basati su modelli."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera tabelle da dati strutturati"
      content: "Estrai dati da JSON, XML, CSV e altri formati per popolare automaticamente le tabelle nei documenti."

    # feature loop
    - title: "Crea contenuti visivi curati"
      content: "Utilizza GroupDocs.Assembly per progettare tabelle, grafici ed elenchi professionali, e aggiungere link, immagini e testo per un aspetto raffinato del documento."

    # feature loop
    - title: "Posizionamento dinamico del contenuto delle tabelle"
      content: "Aggiungi righe e colonne programmaticamente utilizzando modelli basati su LINQ, e personalizza stili come font, colori e allineamento."

    # feature loop
    - title: "Funziona senza problemi tra i formati"
      content: "Crea o modifica facilmente tabelle in MS Office, OpenOffice, PDF, HTML e altri formati, unendoli nei file secondo necessità."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come popolare programmaticamente una tabella"
      content: |
        Questo esempio dimostra come riempire una tabella in un documento PPTX con dati provenienti da una fonte esterna.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Progetta un modello con segnaposti per la tabella
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Specifica il percorso del file al modello
          const template = "table_template.pptx";

          // Carica i dati necessari dalla tua fonte
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Organizza i dati nella struttura necessaria
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Inizializza DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salva il documento di output con la tabella completata
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "Caratteristiche principali a colpo d'occhio"
    exclude: "table"
    description: "La nostra API automatizza la creazione di tabelle e migliora la generazione di documenti con strumenti e modelli versatili."
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
    title: "Genera tabelle in una varietà di formati"
    exclude: "PPTX"
    description: "Con Node.js via Java, popola modelli e crea tabelle complete su oltre 50 tipi di file supportati."
    items: 
          
        # format loop 1
        - name: "Aggiungi una tabella a un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Aggiungi una tabella a un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Aggiungi una tabella a un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Aggiungi una tabella a un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---