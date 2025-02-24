



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: it
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Unisci Documenti in PDF con JavaScript"
head_description: "Combina file PDF utilizzando JavaScript. GroupDocs.Assembly semplifica la fusione dei documenti in pochi e semplici passaggi."

############################# Header ############################
title: "Combina Contenuti in File PDF" 
description: "Con GroupDocs.Assembly for Node.js via Java, integrare un file PDF in un altro è rapido e preciso. Goditi strumenti flessibili e affidabili per una fusione senza interruzioni."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Provalo Gratis"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica di GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) offre un modo potente per gestire documenti. Unisci un file in un altro mentre supporti oltre 50 formati, come PDF e MS Office. Personalizza i layout, modifica il contenuto e organizza i documenti esattamente come necessario.

############################# Steps ############################
steps:
    enable: true
    title: "Come Unire un Documento in un File PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) rende semplice inserire un file PDF in un altro con opzioni personalizzabili.
      
      1. Progetta un modello con segnaposto per il contenuto incorporato (i modelli PDF non sono supportati).
      2. Imposta il percorso del file per il modello.
      3. Fornisci il percorso per il documento da unire.
      4. Salva il documento completato con il contenuto unito come file PDF.
   
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
        // Inserisci questo tag nel tuo modello per definire dove verrà incorporato il documento
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Imposta il percorso del file per il modello principale
        // Attualmente, i modelli PDF non sono supportati.
        const template = "doc_template.docx";

        // Fornisci il percorso per il documento che desideri unire
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // Salva l'output finale con il documento incorporato
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Strumenti Potenti per l'Integrazione dei Documenti"
  description: "GroupDocs.Assembly for Node.js via Java rende l'incorporamento di file attraverso vari formati facile e completamente personalizzabile. Offri risultati coerenti e professionali ogni volta."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Funzionalità Chiave di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera Report con Dati Aziendali"
      content: "Estrai dati da fonti JSON, XML o CSV per creare rapidamente report e documenti completi e accurati."

    # feature loop
    - title: "Aggiungi Elementi Visivi Ricchi"
      content: "GroupDocs.Assembly ti consente di includere tabelle, grafici, elenchi, immagini e codici a barre insieme a testo e collegamenti ipertestuali."

    # feature loop
    - title: "Posizionamento Dati Preciso"
      content: "Utilizza modelli LINQ per posizionare i dati esattamente dove devono stare, gestisci elementi ripetuti come array e personalizza gli stili senza sforzo."

    # feature loop
    - title: "Funziona con una Vasta Gamma di Formati"
      content: "Unisci contenuti senza interruzioni attraverso formati come PDF, file MS Office, HTML e OpenOffice, offrendo flessibilità per tutti i progetti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Incorpora un'Immagine in un Documento Programmaticamente"
      content: |
        Questo esempio dimostra come inserire un'immagine in un file PDF utilizzando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Aggiungi un segnaposto nel modello per l'immagine
          // <<image [expression]>>

          // Specifica il percorso del file del modello
          // Attualmente, i modelli PDF non sono supportati.
          String template = "template.docx";
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Imposta il percorso dell'immagine che desideri incorporare
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Inizializza l'oggetto DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salva il documento con l'immagine inclusa
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "Caratteristiche Principali a Colpo d'Occhio"
    exclude: "document"
    description: "Esplora gli strumenti completi che GroupDocs.Assembly offre per una fusione documentale efficiente e fluida."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Combina Documenti in Molti Formati"
    exclude: "PDF"
    description: "Usa Node.js via Java per unire contenuti in oltre 50 formati di file, garantendo risultati professionali e rifiniti."
    items: 
          
        # format loop 1
        - name: "Incorpora un documento in un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Incorpora un documento in un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Incorpora un documento in un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Incorpora un documento in un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---