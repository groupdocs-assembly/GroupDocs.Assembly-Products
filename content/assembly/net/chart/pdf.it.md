



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: it
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Crea grafici in file PDF con C#"
head_description: "L'API GroupDocs.Assembly for .NET consente agli sviluppatori di generare e inserire grafici o diagrammi nei documenti in modo dinamico utilizzando dati in tempo reale."

############################# Header ############################
title: "Incorpora grafici in file PDF con API .NET" 
description: "GroupDocs.Assembly for .NET offre un modo potente per popolare file PDF con dati dinamici e integrare grafici senza sforzo."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prova Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Che cos'è GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) è uno strumento progettato per semplificare la creazione di documenti e report integrando dati provenienti da varie fonti. Genera dinamicamente grafici, tabelle, elenchi, codici a barre e immagini. Opzioni di formattazione avanzate consentono un posizionamento preciso e la personalizzazione dei contenuti. Supporta oltre 50 formati di file, inclusi PDF, documenti MS Office e email.

############################# Steps ############################
steps:
    enable: true
    title: "Come aggiungere un grafico a un documento PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) semplifica la generazione e l'incorporazione di grafici nei tuoi modelli PDF. Supporta una varietà di tipi di grafico, come grafici a barre, a torta e a linee.
      
      1. Progetta un modello con spazi designati per il grafico (i modelli PDF non sono supportati).
      2. Recupera i tuoi dati da una fonte compatibile.
      3. Definisci le opzioni del grafico come tipo, etichette e schema colori.
      4. Esporta il documento con il grafico come file PDF.
   
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
        // Inserisci questo tag nel tuo modello per generare un grafico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Specifica il percorso del file per il tuo modello
        // Attualmente, i modelli PDF non sono supportati.
        string template = "chart_template.docx";

        // Carica i dati dalla tua fonte preferita
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Salva il documento con il grafico incorporato
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Aggiungi grafici dinamici ai tuoi documenti senza sforzo"
  description: "GroupDocs.Assembly for .NET semplifica la creazione di documenti basati su dati in formati ampiamente utilizzati. Utilizza modelli per inserire grafici, tabelle, codici a barre, elenchi, collegamenti ipertestuali e immagini con integrazione di dati dinamici avanzata."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Trasforma i dati in grafici professionali"
      content: "Converti dati da JSON, XML, CSV e altre fonti in grafici visivamente attraenti con pochi passaggi utilizzando la nostra API."

    # feature loop
    - title: "Crea contenuti visivamente coinvolgenti"
      content: "GroupDocs.Assembly supporta vari tipi di grafico come istogrammi, grafici a torta e grafici a linee. Combina questi con tabelle, codici a barre, immagini e altri elementi per creare report professionali."

    # feature loop
    - title: "Posiziona e personalizza i grafici con precisione"
      content: "Con la sintassi LINQ, puoi generare e posizionare dinamicamente grafici esattamente dove necessario. Personalizza facilmente stili, colori e layout in base alle tue esigenze."

    # feature loop
    - title: "Funziona con vari formati di file"
      content: "Produci documenti in formati popolari come MS Office, PDF, OpenOffice e HTML. Incorpora grafici senza soluzione di continuità in qualsiasi formato supportato con piena compatibilità."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crea un grafico programmaticamente"
      content: |
        Questo esempio dimostra come creare dinamicamente e incorporare un grafico in un documento PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepara un modello con un segnaposto per il grafico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Fornisci il percorso al file del modello
          // Attualmente, i modelli PDF non sono supportati.
          string template = "table_template.docx";

          // Recupera i dati dalla tua fonte
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Costruisci un oggetto dati con le informazioni necessarie
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Imposta le proprietà del grafico come tipo e aspetto
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inizializza DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Esporta il documento con il grafico incluso
          asm.AssembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "Scopri le capacità chiave"
    exclude: "chart"
    description: "La nostra piattaforma ti aiuta a creare documenti coinvolgenti e basati su dati, adattati alle tue esigenze."
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
    title: "Crea report visivamente ricchi in più formati"
    exclude: "PDF"
    description: ".NET ti consente di generare documenti con grafici integrati in oltre 50 formati supportati, combinando modelli con i tuoi dati senza sforzo."
    items: 
          
        # format loop 1
        - name: "Grafici in PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Grafici in DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Grafici in PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Grafici in XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---