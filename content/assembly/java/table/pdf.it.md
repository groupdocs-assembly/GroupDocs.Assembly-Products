



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:57
draft: false
lang: it
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Aggiungi tabelle ai documenti PDF utilizzando Java"
head_description: "Con GroupDocs.Assembly for Java, gli sviluppatori possono integrare rapidamente tabelle in documenti e email, estraendo dati da fonti dinamiche."

############################# Header ############################
title: "Popola facilmente le tabelle nei file PDF con la nostra API Java" 
description: "GroupDocs.Assembly for Java semplifica il processo di riempimento delle tabelle nei documenti PDF con dati provenienti da vari input."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Ottieni la tua prova gratuita"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) è uno strumento per generare documenti e report inserendo automaticamente dati in modelli pre-progettati. Puoi aggiungere tabellet, elenchi, grafici e immagini senza sforzo. Le sue funzionalità avanzate ti consentono di posizionare con precisione contenuti all'interno dei tuoi documenti. Compatibile con oltre 50 tipi di file, tra cui PDF, MS Office e formati email.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per inserire i dati in una tabella PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ti aiuta a popolare i modelli di tabella per PDF e altri formati. Utilizza dati dinamici dalle tue fonti per creare tabelle senza difficoltà.
      
      1. Progetta un modello con segnaposti per la tabella (i modelli PDF non sono attualmente supportati).
      2. Estrai dati da qualsiasi fonte di input supportata.
      3. Filtra o pre-processa i dati per soddisfare le tue esigenze.
      4. Salva il documento con la tabella completata come file PDF.
   
    code:
      platform: "java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento di esempio"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Utilizza questi tag in un segnaposto di riga della tabella all'interno del tuo modello
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Definisci il percorso al file del modello
        // I modelli PDF non sono supportati al momento.
        String template = "table_template.docx";

        // Carica i dati dalla sorgente scelta
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Salva il file di output con la tabella popolata
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Crea documenti con tabelle popolate da dati"
  description: "GroupDocs.Assembly for Java rende semplice automatizzare la creazione di tabelle nei tuoi documenti. Supporta anche l'aggiunta di elementi come grafici, elenchi e immagini utilizzando modelli."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera report da più formati di dati"
      content: "L'API funziona senza problemi con JSON, XML, CSV e altri formati per riempire le tabelle nei tuoi documenti con dati organizzati."

    # feature loop
    - title: "Presenta le informazioni in modo visivo"
      content: "GroupDocs.Assembly ti aiuta a costruire tabelle professionali, elenchi e grafici, nonché ad inserire link, testo e immagini, per un aspetto curato."

    # feature loop
    - title: "Posiziona il contenuto della tabella con precisione"
      content: "Utilizza una sintassi flessibile basata su LINQ per aggiungere righe e colonne dinamicamente. Personalizza l'aspetto, come stili dei caratteri e colori, programmaticamente."

    # feature loop
    - title: "Compatibile con più formati"
      content: "Lavora con MS Office, OpenOffice, PDF, HTML e altro. Unisci tabelle in qualsiasi formato di file supportato senza difficoltà."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crea dinamicamente una tabella riempita di dati"
      content: |
        Questo esempio mostra come popolare una tabella in un documento PDF utilizzando dati di input dinamici.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Progetta un modello con un segnaposto per la tabella
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Imposta la posizione del file del modello
          // I modelli PDF non sono supportati al momento.
          String template = "table_template.docx";

          // Carica i dati dalla tua fonte preferita
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Prepara un oggetto dati contenente i campi necessari
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Crea un'istanza di DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il documento con la tabella popolata
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "Copia"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Esplora le funzionalità di GroupDocs.Assembly gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Scarica da Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Scopri di più sulle licenze"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Caratteristiche chiave a colpo d'occhio"
    exclude: "table"
    description: "La nostra API semplifica la creazione di documenti professionali automatizzando il riempimento delle tabelle insieme ad altri componenti potenti."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produci tabelle dettagliate in vari formati"
    exclude: "PDF"
    description: "Con Java, puoi popolare modelli con dati e generare report dettagliati in oltre 50 tipi di file."
    items: 
          
        # format loop 1
        - name: "Aggiungi una tabella a un PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Aggiungi una tabella a un DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Aggiungi una tabella a un PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Aggiungi una tabella a un XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---