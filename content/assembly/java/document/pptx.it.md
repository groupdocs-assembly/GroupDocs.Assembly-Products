



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: it
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Inserisci un documento in un altro in PPTX utilizzando Java"
head_description: "Combina file PPTX rapidamente con Java. GroupDocs.Assembly semplifica il processo di fusione dei documenti in poche righe di codice."

############################# Header ############################
title: "Incorpora contenuti nei file PPTX senza sforzi" 
description: "Utilizza GroupDocs.Assembly for Java per inserire senza problemi un documento PPTX in un altro. Ottieni risultati precisi con strumenti flessibili e affidabili."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Provalo Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) è una soluzione versatile per la gestione dei documenti. Ti consente di integrare un documento in un altro, supportando oltre 50 formati come PDF e file MS Office. Personalizza il tuo output unendo, modificando e organizzando i contenuti esattamente come desideri.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per inserire un documento in un file PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) rende semplice e personalizzabile l'incorporamento di un documento PPTX in un altro.
      
      1. Prepara un modello PPTX con segnaposto per il contenuto incorporato.
      2. Specifica il percorso del file per il modello.
      3. Fornisci il percorso del documento da incorporare.
      4. Salva il file di output con il contenuto unito.
   
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
        // Utilizza questo tag nel tuo modello per contrassegnare il punto per il documento incorporato
        // <<doc [doc_expression]>>

        // Imposta il percorso del file per il modello principale
        String template = "doc_template.pptx";

        // Fornisci il percorso del documento che desideri inserire
        DataSourceInfo data 
            = new DataSourceInfo("insert.pptx", "doc_expression");

        // Salva il file finale con il contenuto incorporato
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Strumenti avanzati per semplificare l'integrazione dei documenti"
  description: "Con GroupDocs.Assembly for Java, incorporare documenti è semplice e personalizzabile, indipendentemente dal tipo di file. Ottieni risultati puliti e coerenti nei tuoi progetti."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crea report utilizzando dati aziendali"
      content: "Compila documenti con dati provenienti da fonti come JSON, XML o CSV rapidamente e in modo affidabile, ottimizzando i tuoi flussi di lavoro."

    # feature loop
    - title: "Migliora i documenti con contenuti visivi"
      content: "GroupDocs.Assembly consente di inserire tabelle, grafici e liste insieme a testo, link, immagini e persino codici a barre dinamici."

    # feature loop
    - title: "Posiziona i dati esattamente dove servono"
      content: "I modelli LINQ aiutano a posizionare i tuoi dati con precisione, gestire elementi ripetitivi come array e applicare stili personalizzati senza difficoltà."

    # feature loop
    - title: "Compatibile con diversi formati di file"
      content: "Unisci documenti di vari formati, inclusi PDF, HTML, file MS Office e OpenOffice, garantendo flessibilità per i tuoi progetti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come inserire programmaticamente un'immagine in un documento"
      content: |
        Questo esempio mostra come incorporare un'immagine in un file PPTX utilizzando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Aggiungi un tag segnaposto nel file del modello
          // <<image [expression]>>

          // Definisci il percorso per il modello
          String template = "template.pptx";

          // Specifica il percorso dell'immagine
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inizializza l'istanza di DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il file con l'immagine incorporata
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Principali capacità a colpo d'occhio"
    exclude: "document"
    description: "Scopri le ampie funzionalità che GroupDocs.Assembly offre per rendere l'incorporamento e la combinazione di documenti efficienti e senza problemi."
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
    title: "Unisci diversi tipi di documenti"
    exclude: "PPTX"
    description: "Con Java, puoi incorporare e combinare contenuti in oltre 50 formati di file. Aggiungi file senza sforzi per creare risultati professionali."
    items: 
          
        # format loop 1
        - name: "Incorpora un documento in un PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Incorpora un documento in un DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Incorpora un documento in un PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Incorpora un documento in un XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---