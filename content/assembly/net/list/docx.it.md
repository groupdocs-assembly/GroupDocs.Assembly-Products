



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: it
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Genera el documento di liste in DOCX con C#"
head_description: "L'API GroupDocs.Assembly for .NET consente agli sviluppatori di creare dinamicamente e incorporare liste piene di dati all'interno di documenti e modelli."

############################# Header ############################
title: "Aggiungi liste orientate ai dati ai documenti DOCX usando la nostra API .NET" 
description: "GroupDocs.Assembly for .NET offre strumenti potenti per generare e incorporare dinamicamente liste nei documenti DOCX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica la Versione di Prova Gratuita"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica di GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) è progettato per semplificare la creazione di documenti e report integrando senza soluzione di continuità i dati provenienti da varie fonti. Popola i modelli con liste, grafici, tabelle, codici a barre o testo, e posiziona il contenuto con precisione utilizzando markup avanzato. Con il supporto per oltre 50 formati—compresi PDF, file MS Office e email—è ideale per automatizzare i flussi di lavoro documentali.

############################# Steps ############################
steps:
    enable: true
    title: "Passi per aggiungere una lista riempita di dati a un documento DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) semplifica l'inserimento di liste orientate ai dati nei modelli DOCX. Crea e personalizza le liste con precisione.
      
      1. Prepara un modello DOCX con segnaposto per la lista.
      2. Imposta il percorso per il modello.
      3. Recupera i dati da fonti supportate come JSON o XML.
      4. Salva il documento finale con la lista incorporata.
   
    code:
      platform: "net"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento di esempio"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Aggiungi questo tag al tuo modello per segnare dove apparirà la lista
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Specifica il percorso del file modello
        string template = "list_template.docx";

        // Recupera i dati dalla tua fonte scelta
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Salva il documento con la lista generata
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Crea documenti riempiendo modelli con dati strutturati"
  description: "GroupDocs.Assembly for .NET semplifica la creazione di documenti orientati ai dati. Aggiungi dinamicamente liste, tabelle, codici a barre, grafici, immagini e altri elementi con modelli avanzati."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Caratteristiche di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera report da dati aziendali"
      content: "L'API popola documenti in formati popolari utilizzando dati provenienti da fonti come JSON, XML, CSV, ecc. con precisione ed efficienza."

    # feature loop
    - title: "Usa liste e altri elementi per presentare dati"
      content: "GroupDocs.Assembly ti consente di incorporare liste, tabelle e grafici insieme a testo, codici a barre, collegamenti ipertestuali e immagini per creare documenti ben strutturati."

    # feature loop
    - title: "Inserisci i dati esattamente dove necessario"
      content: "Sfrutta la sintassi basata su LINQ per posizionare liste e altri elementi di dati con precisione. Utilizza i cicli per popolare le liste dinamicamente e applica formattazioni personalizzate in modo programmato."

    # feature loop
    - title: "Supporta più formati di documento"
      content: "Genera e gestisci documenti in vari formati come MS Office, OpenOffice, PDF, HTML e file email. Integra facilmente più documenti in uno."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come generare una lista dinamicamente"
      content: |
        Questo esempio dimostra come incorporare una lista generata dinamicamente in un documento DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Aggiungi un tag segnaposto al tuo modello per la lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Specifica il percorso del file modello
          string template = "numlist_template.docx";

          // Recupera i dati per popolare la lista
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Crea un oggetto sorgente dati con le informazioni necessarie
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inizializza DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il documento finale con la lista generata
          asm.AssembleDocument(template, "result.docx", data);
          ```
        platform: "net"
        copy_title: "Copia"
        install:
          command: "dotnet add package GroupDocs.Assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Esplora le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Scarica da Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Scopri di più sulle licenze"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Esplora le capacità principali"
    exclude: "list"
    description: "La nostra piattaforma è costruita per semplificare la creazione e l'integrazione dei contenuti documentali orientati ai dati."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crea documenti strutturati in formati popolari"
    exclude: "DOCX"
    description: ".NET supporta oltre 50 formati, permettendo di unire senza difficoltà dati e modelli per produrre risultati strutturati e raffinati."
    items: 
          
        # format loop 1
        - name: "Crea un elenco in un PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Crea un elenco in un DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Crea un elenco in un PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Crea un elenco in un XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---