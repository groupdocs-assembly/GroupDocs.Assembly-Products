



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: it
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Incorpora un documento in un altro in PPTX con l'API C#"
head_description: "Unisci documenti PPTX utilizzando C#. Con GroupDocs.Assembly, combina file senza soluzione di continuità in pochi passaggi."

############################# Header ############################
title: "Combina documenti nel formato PPTX" 
description: "Con GroupDocs.Assembly for .NET, puoi rapidamente incorporare un documento PPTX in un altro. Questa API offre strumenti robusti per unire documenti con precisione."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Scopri di più"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) è uno strumento potente per la composizione e la manipolazione di documenti. Permette agli utenti di incorporare un documento in un altro, consentendo l'unione fluida dei contenuti. Con supporto per oltre 50 formati, tra cui PDF, file MS Office e altro, puoi organizzare, modificare e personalizzare il risultato finale per soddisfare le tue esigenze.

############################# Steps ############################
steps:
    enable: true
    title: "Come unire un documento in un file PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) ti consente di incorporare un documento in un altro file PPTX senza sforzo. Unisci e personalizza i contenuti.
      
      1. Progetta un modello PPTX con segnaposto per il documento incorporato.
      2. Definisci il percorso del file per il modello.
      3. Specifica il percorso del documento da incorporare.
      4. Salva il file finale con il contenuto incorporato.
   
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
        // Aggiungi questo tag al tuo modello per contrassegnare il punto di inserimento
        // <<doc [doc_expression]>>

        // Specifica il percorso del file per il modello
        string template = "doc_template.pptx";

        // Fornisci il percorso del documento da incorporare
        DataSourceInfo data 
            = new DataSourceInfo("insert.pptx", "doc_expression");

        // Salva il documento unito
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ottimizza l'unione dei documenti con strumenti avanzati"
  description: "La libreria GroupDocs.Assembly for .NET semplifica l'incorporamento di un documento in un altro, supportando vari formati di file e offrendo personalizzazioni per un'integrazione senza soluzione di continuità."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera report dai tuoi dati aziendali"
      content: "Popola automaticamente i documenti con dati provenienti da JSON, XML, CSV o altre fonti, garantendo flussi di lavoro accurati ed efficienti."

    # feature loop
    - title: "Arricchisci i documenti con elementi visivi"
      content: "GroupDocs.Assembly ti consente di includere tabelle, grafici e elenchi, oltre a testo, collegamenti, immagini e codici a barre generati dinamicamente."

    # feature loop
    - title: "Posiziona e formatta i dati con precisione"
      content: "I modelli basati su LINQ ti offrono controllo sul posizionamento dei dati, permettendoti di gestire cicli per gli array e consentendo stilizzazioni come la personalizzazione dei colori."

    # feature loop
    - title: "Funziona con più formati di file"
      content: "Incorpora facilmente documenti l'uno nell'altro tra formati come MS Office, PDF, HTML, OpenOffice e altro."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come incorporare un'immagine in un documento programmaticamente"
      content: |
        Questo esempio dimostra come inserire un'immagine in un documento PPTX utilizzando GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Aggiungi un tag segnaposto nel tuo modello
          // <<image [expression]>>

          // Specifica il percorso del file per il modello
          string template = "template.pptx";

          // Imposta il percorso del file immagine
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inizializza un'istanza di DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salva il documento con l'immagine incorporata
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Scopri i nostri potenti strumenti"
    exclude: "document"
    description: "Esplora le funzionalità che GroupDocs.Assembly offre per l'incorporamento e l'unione di documenti con precisione."
    items: 
          
        # operation loop 1
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Crea dinamicamente e aggiungi codici a barre ai documenti"

        # operation loop 2
        - name: "Visualizza dati con diagrammi"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Compila vari tipi di diagrammi con dati"

        # operation loop 3
        - name: "Unisci documenti"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Combina il contenuto di un documento in un altro"

        # operation loop 4
        - name: "Mostra dati con elenchi"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Genera elenchi nei documenti utilizzando dati specifici"

        # operation loop 5
        - name: "Organizza dati in tabelle"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Recupera dati da qualsiasi fonte e popolari tabelle"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Unisci documenti in vari formati"
    exclude: "PPTX"
    description: "Con l'API .NET, puoi combinare documenti in oltre 50 formati supportati. Incorpora senza sforzo file o sezioni nei tuoi documenti finali."
    items: 
          
        # format loop 1
        - name: "Incorpora un documento in un PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 2
        - name: "Incorpora un documento in un DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Incorpora un documento in un PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Presentazione PowerPoint Open XML"
          
        # format loop 4
        - name: "Incorpora un documento in un XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Foglio di Calcolo Microsoft Excel Open XML"


          

---