



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:09
draft: false
lang: it
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Crea elenchi nei documenti PPTX utilizzando Java"
head_description: "Progetta e inserisci facilmente elenchi dinamici nei tuoi modelli PPTX con l'API GroupDocs.Assembly for Java."

############################# Header ############################
title: "Aggiungi elenchi dinamici ai file PPTX con la nostra API Java" 
description: "GroupDocs.Assembly for Java offre strumenti flessibili per generare e inserire elenchi ricchi di dati direttamente nei documenti PPTX."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Provalo gratuitamente"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) consente di progettare documenti professionali estraendo dati da più fonti. Utilizzalo per creare elenchi, tabelle, grafici o testo, e posizionare questi elementi esattamente dove necessario utilizzando funzioni avanzate dei modelli. Con supporto per oltre 50 formati, inclusi PDF, file MS Office e documenti email, aiuta ad automatizzare e semplificare il tuo flusso di lavoro.

############################# Steps ############################
steps:
    enable: true
    title: "Come aggiungere un elenco guidato dai dati a un documento PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ti consente di inserire rapidamente elenchi ricchi di dati nei modelli PPTX. Personalizza e organizza i contenuti senza sforzo.
      
      1. Crea un modello PPTX e contrassegna i punti di segnaposto per l'elenco.
      2. Imposta il percorso del file per il modello.
      3. Estrai dati da formati supportati come JSON o XML.
      4. Salva il documento finale con l'elenco aggiunto.
   
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
        // Include questo tag nel tuo modello dove deve apparire l'elenco
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Definisci il percorso del file del modello
        String template = "list_template.pptx";

        // Estrai i dati dalla tua fonte scelta
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Salva il documento con l'elenco incorporato
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Genera documenti da modelli con integrazione dei dati"
  description: "GroupDocs.Assembly for Java semplifica l'aggiunta di elenchi dinamici, tabelle, grafici e altri componenti nei modelli di documento."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crea report con dati provenienti da varie fonti"
      content: "Utilizza dati provenienti da formati come JSON, XML e CSV per popolare elenchi e altri componenti in modo efficiente."

    # feature loop
    - title: "Aggiungi elenchi e altri elementi di dati senza soluzione di continuità"
      content: "GroupDocs.Assembly consente l'inserimento di elenchi, grafici, tabelle e altro, insieme a testo, immagini e link per creare documenti curati."

    # feature loop
    - title: "Controlla con precisione dove appaiono i dati"
      content: "I modelli basati su LINQ consentono di definire posizioni esatte per i tuoi elenchi e i dati. Utilizza loop per creare elenchi dettagliati automaticamente e applica formattazioni personalizzate."

    # feature loop
    - title: "Supporta vari formati di documento"
      content: "Crea o modifica file in formati come MS Office, PDF, OpenOffice, HTML e email. Unisci contenuti da più documenti secondo necessità."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come creare un elenco programmaticamente"
      content: |
        Questo esempio mostra come aggiungere dinamicamente un elenco a un file PPTX utilizzando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Aggiungi un tag segnaposto nel tuo modello per l'elenco
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Fornisci il percorso del file per il tuo modello
          String template = "numlist_template.pptx";

          // Estrai i dati richiesti per popolare l'elenco
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Prepara la fonte di dati con i dettagli necessari
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inizializza DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il documento di output con l'elenco completato
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "Scopri cosa può fare GroupDocs.Assembly"
    exclude: "list"
    description: "Progetta e genera facilmente documenti ricchi di contenuti con avanzati strumenti di integrazione dei dati."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produci documenti in vari formati"
    exclude: "PPTX"
    description: "Java supporta oltre 50 formati, permettendoti di creare documenti strutturati combinando dati e modelli."
    items: 
          
        # format loop 1
        - name: "Crea un elenco in un PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Crea un elenco in un DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Crea un elenco in un PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Crea un elenco in un XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---