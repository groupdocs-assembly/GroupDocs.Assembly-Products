



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: it
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Genera grafici in documenti DOCX utilizzando Java"
head_description: "L'API GroupDocs.Assembly for Java consente agli sviluppatori di creare e inserire grafici dinamici o diagrammi nei documenti in modo fluido, alimentati da dati in tempo reale."

############################# Header ############################
title: "Aggiungi grafici ai documenti DOCX con l'API Java" 
description: "GroupDocs.Assembly for Java semplifica il processo di incorporamento dei grafici nei documenti DOCX sfruttando dati in tempo reale."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inizia Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduzione a GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) è una soluzione versatile per automatizzare la creazione di documenti e report. Ti consente di aggiungere grafici, tabelle, elenchi, codici a barre e immagini direttamente nei tuoi file, con strumenti avanzati per un'accurata formattazione e integrazione dei dati. La piattaforma supporta oltre 50 formati, inclusi PDF, file di Microsoft Office e email.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per incorporare un grafico in un documento DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) semplifica il processo di inserimento di grafici nei template DOCX. Scegli tra una varietà di stili di grafico, inclusi grafici a barre, a torta e a linee.
      
      1. Crea un template DOCX con segnaposto per il grafico.
      2. Carica i tuoi dati da una fonte compatibile.
      3. Imposta le opzioni del grafico, come tipo, etichette e colori.
      4. Salva il documento con il grafico incluso.
   
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
        // Aggiungi questo tag al tuo template per includere un grafico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Fornisci il percorso del file per il tuo template
        String template = "chart_template.docx";

        // Estrai i dati necessari dalla tua sorgente
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Salva il documento finale con il grafico incorporato
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Incorpora facilmente grafici dinamici nei tuoi documenti"
  description: "GroupDocs.Assembly for Java offre un modo semplice per creare documenti ricchi di dati nei formati più diffusi. Usa template per inserire grafici, tabelle, codici a barre, elenchi, link e immagini con aggiornamenti dinamici dai tuoi dati."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Trasforma i dati in grafici"
      content: "Utilizza l'API per trasformare i dati provenienti da JSON, XML, CSV o altre fonti in grafici chiari e professionali per i tuoi documenti."

    # feature loop
    - title: "Crea contenuti visivamente impattanti"
      content: "GroupDocs.Assembly supporta vari formati visivi, tra cui grafici a barre, grafici a torta e grafici a linee, che possono essere combinati con tabelle, codici a barre, immagini e altro per report migliorati."

    # feature loop
    - title: "Posizionamento e stile dei grafici personalizzabili"
      content: "Con una sintassi basata su LINQ, puoi generare e posizionare dinamicamente grafici nel documento, mentre regoli facilmente stili, colori e layout per soddisfare le tue esigenze di design."

    # feature loop
    - title: "Supporta più formati di documento"
      content: "Genera documenti in formati come MS Office, PDF, OpenOffice e HTML. I grafici si integrano perfettamente in qualsiasi formato supportato per risultati professionali."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Genera e incorpora grafici programmaticamente"
      content: |
        Questo esempio dimostra come creare e incorporare un grafico in un documento DOCX in modo programmatico.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Prepara un template con un segnaposto per il grafico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Specifica il percorso del file per il template
          String template = "table_template.docx";

          // Carica i dati dalla tua sorgente scelta
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crea un oggetto dati con le informazioni rilevanti
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configura il tipo e l'aspetto del grafico
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inizializza DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il documento completato con il grafico incorporato
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "Esplora potenti capacità"
    exclude: "chart"
    description: "Questa piattaforma semplifica il processo di progettazione di documenti visivamente accattivanti e focalizzati sui dati, adattati alle tue esigenze."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Genera report completi in formati diversi"
    exclude: "DOCX"
    description: "Java ti consente di creare documenti con grafici integrati in oltre 50 formati di file, assicurando una fusione fluida di template e dati."
    items: 
          
        # format loop 1
        - name: "Grafici in PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Grafici in DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Grafici in PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Grafici in XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---