



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: it
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Crea tabelle in documenti PDF con C#"
head_description: "L'API GroupDocs.Assembly for .NET consente agli sviluppatori di aggiungere e popolare senza sforzo tabelle in documenti ed email con dati da fonti dinamiche."

############################# Header ############################
title: "Genera tabelle di dati in documenti PDF utilizzando la nostra API .NET" 
description: "GroupDocs.Assembly for .NET consente di riempire dinamicamente tabelle in documenti PDF con dati provenienti da varie fonti."
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
       [GroupDocs.Assembly for .NET](/assembly/net/) è progettato per creare documenti e report riempiendo i modelli con dati provenienti da più fonti. Inserisci senza sforzo dati strutturati in tabelle, elenchi e grafici, oppure incorpora immagini in modo dinamico. La sintassi avanzata garantisce un posizionamento accurato dei dati. Supporta oltre 50 formati, inclusi PDF, documenti MS Office e file email.

############################# Steps ############################
steps:
    enable: true
    title: "Come popolare una tabella in un documento PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ti consente di popolare dinamicamente tabelle in modelli per formati come PDF. Inserisci dati provenienti da varie fonti nelle tue tabelle.
      
      1. Crea un modello e aggiungi segnaposto per la tabella (i modelli PDF non sono attualmente supportati).
      2. Recupera dati da qualsiasi fonte supportata.
      3. Filtra i dati per includere solo le informazioni necessarie.
      4. Salva il documento con la tabella completata come file PDF.
   
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
        // Aggiungi questi tag in una riga di tabella del modello
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Imposta il percorso del file per il modello
        // I modelli PDF non sono disponibili al momento.
        string template = "table_template.docx";

        // Recupera dati da una fonte supportata
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Salva il documento con la tabella riempita con dati
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Genera documenti con tabelle dinamiche"
  description: "GroupDocs.Assembly for .NET semplifica la creazione di documenti automatizzando la popolazione delle tabelle e supportando elementi aggiuntivi come grafici, elenchi e immagini tramite modelli e markup avanzato."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crea report da dati strutturati"
      content: "L'API elabora dati provenienti da fonti come JSON, XML e CSV per popolare le tabelle nei documenti d'ufficio in modo efficiente e preciso."

    # feature loop
    - title: "Visualizza i dati"
      content: "GroupDocs.Assembly consente di creare tabelle, elenchi e grafici, insieme all'incorporamento di testi, collegamenti e immagini per un design professionale del documento."

    # feature loop
    - title: "Posiziona precisamente i dati della tabella"
      content: "Utilizza la sintassi basata su LINQ per aggiungere dinamicamente righe e colonne alla tabella. Personalizza gli stili, comprese le colorazioni e il formato, programmaticamente."

    # feature loop
    - title: "Supporta un'ampia gamma di formati"
      content: "Gestisci senza problemi formati di file popolari come MS Office, OpenOffice, PDF e HTML. Inserisci senza soluzione di continuità tabelle popolate nei tipi di documenti supportati."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come popolare dinamicamente una tabella di dati"
      content: |
        Questo esempio dimostra come riempire una tabella in un documento PDF utilizzando dati dinamici.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepara un modello con un segnaposto per la tabella
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Specifica il percorso del file per il modello
          // I modelli PDF non sono disponibili al momento.
          string template = "table_template.docx";

          // Recupera dati dalla tua fonte scelta
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crea un oggetto sorgente dati con i dati necessari
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Inizializza DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il documento completato con la tabella popolata
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    title: "Esplora le caratteristiche chiave"
    exclude: "table"
    description: "La nostra soluzione semplifica la creazione di documenti professionali con tabelle popolate dinamicamente e elementi aggiuntivi."
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
    title: "Crea report con tabelle dettagliate"
    exclude: "PDF"
    description: ".NET consente la creazione di report completi riempiendo i modelli con tabelle e altri elementi di dati in oltre 50 formati supportati."
    items: 
          
        # format loop 1
        - name: "Aggiungi una tabella a un PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Aggiungi una tabella a un DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Aggiungi una tabella a un PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Aggiungi una tabella a un XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---