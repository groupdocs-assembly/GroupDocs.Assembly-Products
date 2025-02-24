



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: it
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Genera codici a barre in documenti PDF con C#"
head_description: "L'API GroupDocs.Assembly for .NET consente agli sviluppatori di generare e incorporare dinamicamente immagini di codici a barre in documenti ed email."

############################# Header ############################
title: "Aggiungi codici a barre a documenti PDF utilizzando la nostra API .NET" 
description: "GroupDocs.Assembly for .NET offre pieno supporto per creare e incorporare codici a barre in modo dinamico nei documenti PDF."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica la versione di prova gratuita"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica di GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) è progettato per aiutarti a generare documenti e report integrando dati provenienti da una vasta gamma di fonti. Popola documenti con dati testuali o numerici, crea grafici, tabelle e liste, o inserisci immagini e codici a barre al volo. Utilizza markup avanzati per posizionare i dati esattamente dove necessario. Supporta oltre 50 formati, tra cui PDF, file MS Office e email.

############################# Steps ############################
steps:
    enable: true
    title: "Passi per aggiungere un codice a barre generato a un documento PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) consente di inserire codici a barre in modelli in formati come PDF. Supporta oltre 60 tipi di codici a barre, inclusi formati unidimensionali e bidimensionali.
      
      1. Crea un modello con tag specifici per il posizionamento del codice a barre (nota: i modelli PDF non sono compatibili).
      2. Recupera i dati da qualsiasi fonte di dati supportata.
      3. Configura ulteriori proprietà come la dimensione o la risoluzione del codice a barre.
      4. Salva il documento finale con il codice a barre inserito come PDF.
   
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
        // Inserisci questa etichetta nel tuo modello per generare un codice a barre nel documento finale
        // <<barcode [barcode_expression] -barcode_type>>

        // Specifica il percorso del file del modello
        // Il supporto per modelli PDF non è attualmente disponibile.
        string template = "barcode_template.docx";

        // Recupera i dati dalla tua fonte
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Salva il documento con il codice a barre generato
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Genera documenti compilando modelli con dati"
  description: "GroupDocs.Assembly for .NET è progettato per semplificare la creazione di documenti in formati popolari. Aggiungi grafici, liste, tabelle, collegamenti ipertestuali, immagini e codici a barre utilizzando modelli e markup avanzati."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Caratteristiche di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crea report da dati aziendali"
      content: "La nostra API popola efficientemente documenti in formati office popolari utilizzando dati provenienti da fonti come JSON, XML e CSV."

    # feature loop
    - title: "Usa elementi visivi per visualizzare i dati"
      content: "GroupDocs.Assembly supporta l'incorporamento di elementi nativi come liste, tabelle e grafici, insieme a testo, collegamenti ipertestuali, immagini e codici a barre generati dinamicamente."

    # feature loop
    - title: "Inserisci dati ovunque nel documento"
      content: "Utilizza una sintassi basata su LINQ per posizionare i dati esattamente dove necessario. Gli array possono essere inseriti utilizzando cicli for-each, e il formato (ad es. colore) può essere personalizzato programmaticamente."

    # feature loop
    - title: "Supporta una vasta gamma di formati"
      content: "Elabora formati di file popolari come MS Office, OpenOffice, PDF, HTML e vari formati email. Incorpora un documento all'interno di un altro secondo necessità."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come generare dinamicamente un codice a barre"
      content: |
        Questo esempio dimostra come incorporare un codice a barre generato dinamicamente in un documento PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Utilizza questo modello per inserire un codice a barre nel documento
          // <<barcode [barcode_expression] -barcode_type>>

          // Specifica il percorso del file del modello
          // Il supporto per modelli PDF non è attualmente disponibile.
          string template = "barcode_template.docx";

          // Recupera i dati dalla tua fonte scelta
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Crea un oggetto sorgente dati con solo i dati necessari
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Inizializza DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Imposta proprietà aggiuntive del codice a barre
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // Salva il documento finale con il codice a barre incorporato
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "Esplora le caratteristiche principali"
    exclude: "barcode"
    description: "La nostra soluzione è progettata per semplificare le tue esigenze di elaborazione documenti aziendali."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crea report in formati popolari"
    exclude: "PDF"
    description: ".NET supporta la generazione di report in oltre 50 formati, permettendoti di fondere senza problemi dati e modelli per risultati eccezionali."
    items: 
          
        # format loop 1
        - name: "Aggiungi un codice a barre a un PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Aggiungi un codice a barre a un DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Aggiungi un codice a barre a un PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Aggiungi un codice a barre a un XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---