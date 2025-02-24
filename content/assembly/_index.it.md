---
############################# Static ############################
layout: "family"
date:  2025-02-24T17:52:12
draft: false

product: "Assembly"
product_tag: "assembly"

lang: it

############################# Head ############################
head_title: "API e App per l'Assemblaggio di Documenti per .NET, Java, Node.js di GroupDocs"
head_description: "Ottieni una soluzione di automazione e reporting documentale tutto-in-uno per applicazioni .NET, Java e Node.js. Genera tutti i documenti comuni da modelli personalizzati e dati."

############################# Header ############################
title: "Soluzione di Automazione Documentale e Reporting"
description:  |
  Crea report dettagliati utilizzando modelli e fonti di dati con le nostre app e API multipiattaforma.

  Genera report in formati come Word, Excel, Presentazioni e molti altri utilizzando modelli con markup flessibile.

  Popola grafici, codici a barre, tabelle e altri elementi con dati provenienti da fonti come JSON, XML, CSV, ecc.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Scegli la tua piattaforma"
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Assembly è compatibile con i seguenti sistemi operativi e framework:"
  details_link_title: "Scopri di più"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualsiasi altro editor di testo
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Caratteristiche principali di GroupDocs.Assembly"
  description: "Questa soluzione ti aiuta a creare report in formati documentali popolari, automaticamente riempiti con i tuoi dati aziendali. Automatizza i tuoi compiti di generazione documentale."

  items:
    # items loop
    - icon: "additional"
      title: "Popola i modelli con i dati"
      content: "Compila report utilizzando dati provenienti da fonti supportate."

    # items loop
    - icon: "manipulate"
      title: "Markup flessibile"
      content: "Aggiungi dati ai documenti in modo personalizzabile."

    # items loop
    - icon: "structure"
      title: "Caratteristiche documentali native"
      content: "Visualizza i dati utilizzando tabelle, grafici e codici a barre."

    # items loop
    - icon: "merge"
      title: "Tutti i formati popolari"
      content: "Supporta tutti i formati documentali comunemente utilizzati."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Genera report ben personalizzati"
  description: "GroupDocs.Assembly esempi di codice"
  items:
    # code sample loop
    - title: "Utilizzo di Codici a Barre Generati"
      content: |
       GroupDocs.Assembly consente il markup dei codici a barre nei modelli di report. Durante la creazione di un report, un codice a barre viene generato in base al markup e ai dati forniti. Specifica il percorso del modello contenente il testo, gli oggetti dati e il markup. Specifica anche la fonte dei dati per riempire il codice a barre con il contenuto.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Crea un'istanza della classe DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Specifica il percorso del modello
            var tmp_path = "barcode_template.docx";

            //Specifica il percorso per il documento di risultato
            var res_path = "result.docx";

            //Crea un'istanza della fonte dati
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Chiama AssembleDocument per generare il report
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Crea un'istanza della classe DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Specifica il percorso del modello
            String tmp_path = "barcode_template.docx";

            //Specifica il percorso per il documento di risultato
            String res_path = "result.docx";

            //Crea un'istanza della fonte dati
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Chiama AssembleDocument per generare il report
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // Crea un'istanza della classe DocumentAssembler
            const assembler = new assemblyLib.DocumentAssembler();
            
            //Specifica il percorso del modello
            const tmp_path = "barcode_template.docx";

            //Specifica il percorso per il documento di risultato
            const res_path = "result.docx";

            //Crea un'istanza della fonte dati
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // Chiama AssembleDocument per generare il report
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Supporta più di 50 formati di file"
  description: "GroupDocs.Assembly lavora praticamente con tutti i formati di file popolari"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistiche del nostro prodotto"
  description: "Esplora le metriche del prodotto per ottenere informazioni sui nostri progressi, impatti e crescita."

  items:
    # items loop
    - number: "50+"
      title: "Formati Supportati"
      content: "Supportiamo oltre 50 dei formati documentali più utilizzati."

    # items loop
    - number: "650k"
      title: "Download NuGet"
      content: "GroupDocs.Assembly per .NET è una libreria popolare con oltre 650.000 download su NuGet."

    # items loop
    - number: "18k"
      title: "Download Maven"
      content: "Gli sviluppatori Java hanno scaricato GroupDocs.Assembly su Maven oltre 18.000 volte."

    # items loop
    - number: "150+"
      title: "Clienti Soddisfatti"
      content: "I nostri prodotti sono affidati da sviluppatori individuali e da aziende leader in tutto il mondo per creare soluzioni innovative."


############################# Customers ###############################
customers:
  enable: true
  title: "I Nostri Clienti Soddisfatti"
  description: "Le librerie di GroupDocs sono utilizzate da alcuni dei marchi più rinomati e rispettati a livello globale."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Pronto per Cominciare?"
  description: "Testa le funzionalità di GroupDocs.Assembly gratuitamente sulla tua piattaforma."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Domande Frequenti"
  description: "Esplora le nostre Domande Frequenti."

  items:
    # items loop
    - question: "Richiede GroupDocs.Assembly librerie esterne per la composizione dei documenti?"
      answer: "No, GroupDocs.Assembly funziona in modo indipendente e non richiede librerie di terzi come Adobe Acrobat o Microsoft Office."

    # items loop
    - question: "Posso testare le funzionalità di GroupDocs.Assembly prima di acquistare?"
      answer: "Sì, puoi! GroupDocs.Assembly offre una prova gratuita. Installala ed esplora le sue funzionalità. La versione di prova aggiunge 'badge di prova' ai tuoi documenti e elabora solo le prime 3 pagine. Per l'esperienza completa, ottieni una licenza temporanea gratuita di 30 giorni per accedere a tutte le funzionalità. Maggiori dettagli sono disponibili sotto [licenza temporanea](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quali tipi di licenze sono disponibili?"
      answer: "Cerchi una licenza GroupDocs.Assembly? Offriamo diverse opzioni per soddisfare le tue esigenze. Scegli in base alle dimensioni del tuo team, posizione di distribuzione (ufficio singolo o remoto) e se desideri condividere l'SDK/API con i clienti per la distribuzione. In alternativa, scegli una licenza di utilizzo mensile con piani tariffari basati sull'uso: paga solo per ciò che utilizzi. Scopri l'opzione migliore per te nella sezione [prezzi](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "API Low-Code di GroupDocs.Assembly"
  description: "Genera documenti utilizzando la tua applicazione attraverso la nostra API REST basata su cloud."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Utilizza l'API RESTful cURL per aggiungere dati a Word, Excel, PowerPoint e a molti altri modelli."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Migliora le tue applicazioni .NET generando report attraverso il Cloud SDK. Visualizza i dati aziendali nel tuo formato personalizzato."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "Il SDK di GroupDocs.Assembly offre diverse opzioni per le applicazioni Java per generare vari tipi di documenti."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Web Apps di GroupDocs.Assembly"
  description: "GroupDocs.Assembly offre un'applicazione web gratuita per generare documenti. Puoi elaborare più di 50 formati di file popolari direttamente nel tuo browser, GRATIS."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Genera report in Excel, Word, PowerPoint e in molti altri tipi di file direttamente dal tuo browser web."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Crea documenti Microsoft Word da modelli e fonti di dati."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Carica un modello e una fonte di dati per generare report Excel gratuitamente."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---