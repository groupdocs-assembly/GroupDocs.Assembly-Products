



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: it
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Aggiungi Codici a Barre a File XLSX Utilizzando JavaScript"
head_description: "Genera e incorpora codici a barre nei tuoi documenti e nelle tue email con l'API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Crea Codici a Barre per File XLSX Utilizzando Node.js" 
description: "Con GroupDocs.Assembly for Node.js via Java, puoi generare dinamicamente, personalizzare e incorporare codici a barre nei documenti XLSX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inizia"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduzione a GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) consente di creare documenti professionali combinando dati provenienti da più fonti. Aggiungi grafici, tabelle, elenchi, immagini e codici a barre ai tuoi file. Utilizza modelli per organizzare i contenuti esattamente dove devono essere. Funziona con oltre 50 formati, inclusi PDF, documenti Office ed email.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per Aggiungere un Codice a Barre in File XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) semplifica l'incorporamento di codici a barre nei documenti XLSX. Supporta oltre 60 tipi di codici a barre, inclusi formati 1D e 2D.
      
      1. Crea un modello XLSX con segnaposto per i codici a barre.
      2. Recupera i dati da una fonte compatibile.
      3. Imposta le opzioni del codice a barre come dimensione e risoluzione.
      4. Salva il documento finale con il codice a barre incorporato.
   
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
        // Usa questo tag nel modello per includere un codice a barre nel documento di output
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Specifica il percorso del file modello
        const template = "barcode_template.xlsx";

        // Carica i dati necessari dalla tua fonte
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Salva il documento con il codice a barre applicato
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Genera Documenti con Modelli Basati su Dati"
  description: "Con GroupDocs.Assembly for Node.js via Java, puoi creare file professionali in formati popolari incorporando senza problemi grafici, tabelle, elenchi, collegamenti, immagini e codici a barre."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Funzionalità Principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crea Report con Dati Aziendali"
      content: "Utilizza l'API per popolare i modelli con dati provenienti da formati come JSON, XML e CSV in modo rapido e accurato."

    # feature loop
    - title: "Aggiungi Elementi Visivi"
      content: "GroupDocs.Assembly supporta l'inserimento di elementi come grafici, tabelle, elenchi, testo, collegamenti, immagini e codici a barre in tempo reale."

    # feature loop
    - title: "Controllo della Posizione dei Dati"
      content: "Con i modelli basati su LINQ, puoi posizionare con precisione i dati, eseguire cicli attraverso gli array e applicare formattazioni personalizzate tramite codice."

    # feature loop
    - title: "Compatibile con Molti Formati"
      content: "Lavora con file come documenti MS Office, PDF, HTML, file OpenOffice e email. Unisci più documenti quando necessario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Esempio: Generare un Codice a Barre Programmaticamente"
      content: |
        Questo esempio dimostra come generare e inserire programmaticamente un codice a barre in un documento XLSX.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Progetta un modello con un segnaposto per il codice a barre
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Specifica il percorso del file modello
          const template = "barcode_template.xlsx";

          // Recupera i dati dalla tua fonte
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Crea un oggetto data source con i dettagli richiesti
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Inizializza un'istanza di DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Configura il codice a barre
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Salva il documento con il codice a barre incluso
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: "Esplora le Funzionalità Chiave"
    exclude: "barcode"
    description: "Semplifica l'elaborazione dei documenti con strumenti avanzati e capacità di automazione."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formati di File Supportati per la Creazione di Report"
    exclude: "XLSX"
    description: "Node.js via Java gestisce oltre 50 tipi di files, semplificando l'unione dei dati e l'elaborazione dei modelli per risultati di alta qualità."
    items: 
          
        # format loop 1
        - name: "Aggiungi un codice a barre a un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Aggiungi un codice a barre a un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Aggiungi un codice a barre a un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Aggiungi un codice a barre a un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---