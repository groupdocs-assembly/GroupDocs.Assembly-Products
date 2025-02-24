



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: it
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Crea elenchi dinamici in DOCX con JavaScript"
head_description: "Progetta e inserisci facilmente elenchi nei modelli DOCX utilizzando l'API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Incorpora elenchi basati su dati nei file DOCX con Node.js" 
description: "GroupDocs.Assembly for Node.js via Java offre strumenti potenti per aggiungere elenchi flessibili e alimentati da dati ai documenti DOCX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inizia gratuitamente"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) semplifica la creazione di documenti estraendo dati da diverse fonti e incorporandoli nei modelli. Utilizzalo per costruire elenchi, tabelle, grafici e altri elementi, con opzioni di posizionamento e formattazione precise. Supportando oltre 50 formati, inclusi PDF, MS Office e email, aiuta ad automatizzare il processo di generazione dei documenti.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per inserire un elenco in un file DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) rende semplice aggiungere elenchi dettagliati e alimentati da dati ai tuoi modelli DOCX.
      
      1. Crea un modello DOCX e definisci i segnaposto per l'elenco.
      2. Fornisci il percorso del file del modello.
      3. Carica dati da sorgenti supportate come JSON o XML.
      4. Salva il documento con l'elenco generato.
   
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
        // Posiziona questo tag nel tuo modello per indicare dove andrà l'elenco
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Imposta il percorso del file per il tuo modello
        const template = "list_template.docx";

        // Recupera dati dalla fonte che desideri utilizzare
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Salva il file con l'elenco incorporato
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Genera facilmente documenti con dati integrati"
  description: "Con GroupDocs.Assembly for Node.js via Java, puoi integrare elenchi, tabelle, grafici e altri elementi nei modelli, risparmiando tempo e sforzi."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Punti salienti di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera report da più fonti di dati"
      content: "Importa dati da JSON, XML, CSV o altri formati per popolare elenchi e componenti in modo efficiente."

    # feature loop
    - title: "Aggiungi elenchi e altri elementi visivi"
      content: "GroupDocs.Assembly ti consente di incorporare senza soluzione di continuità elenchi, tabelle, grafici e altro accanto a testi, immagini e collegamenti per risultati raffinati."

    # feature loop
    - title: "Posiziona e stila i dati con precisione"
      content: "I modelli basati su LINQ ti permettono di controllare esattamente dove appaiono elenchi e altri dati, utilizzare cicli per elementi ripetuti e personalizzare gli stili in base alle tue esigenze."

    # feature loop
    - title: "Funziona su più formati"
      content: "Crea documenti in formati come MS Office, PDF, OpenOffice, HTML e email. Unisci contenuti provenienti da diverse fonti in un unico file."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crea programmaticamente un elenco in un documento"
      content: |
        Questo esempio dimostra come aggiungere dinamicamente un elenco a un documento DOCX utilizzando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Aggiungi un segnaposto nel tuo modello per l'elenco
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Specifica il percorso del file del modello
          const template = "numlist_template.docx";

          // Carica dati per popolare l'elenco
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Prepara la sorgente dati con i dettagli richiesti
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Inizializza il DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salva il documento finale con l'elenco incluso
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "Esplora le funzionalità di GroupDocs.Assembly"
    exclude: "list"
    description: "Progetta e genera documenti ricchi di dati senza sforzo utilizzando potenti strumenti di integrazione."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crea documenti in diversi formati"
    exclude: "DOCX"
    description: "Node.js via Java supporta oltre 50 formati di file, semplificando la fusione di modelli e dati per risultati professionali."
    items: 
          
        # format loop 1
        - name: "Crea un elenco in un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Crea un elenco in un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Crea un elenco in un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Crea un elenco in un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---