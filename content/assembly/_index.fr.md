---
############################# Static ############################
layout: "family"
date:  2025-01-16T13:04:05
draft: false

product: "Assembly"
product_tag: "assembly"

lang: fr

############################# Head ############################
head_title: "APIs & Applications en ligne d'assemblage de documents pour .NET, Java, Node.js par GroupDocs"
head_description: "Obtenez une solution d'automatisation et de reporting de documents tout-en-un pour les applications .NET, Java et Node.js. Générez tous les documents courants à partir de modèles et de données personnalisées."

############################# Header ############################
title: "Solution d'automatisation des documents et de reporting"
description:  |
  Créez des rapports détaillés en utilisant des modèles et des sources de données avec nos applications et APIs multiplateformes.

  Générez des rapports dans des formats tels que Word, Excel, Présentations, et bien d'autres en utilisant des modèles avec un balisage flexible.

  Remplissez des graphiques, codes-barres, tableaux et autres éléments avec des données provenant de sources telles que JSON, XML, CSV, etc.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choisissez votre plateforme"
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Assembly est compatible avec les systèmes d'exploitation et frameworks suivants :"
  details_link_title: "En savoir plus"

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
                    Atom <br> Visual Studio Code <br> Tout autre éditeur de texte
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Fonctionnalités clés de GroupDocs.Assembly"
  description: "Cette solution vous aide à créer des rapports dans des formats de documents populaires, remplis automatiquement avec vos données commerciales. Automatisez vos tâches de génération de documents."

  items:
    # items loop
    - icon: "additional"
      title: "Remplir des modèles avec des données"
      content: "Remplissez les rapports en utilisant des données provenant de sources prises en charge."

    # items loop
    - icon: "manipulate"
      title: "Balisage flexible"
      content: "Ajoutez des données aux documents de manière personnalisable."

    # items loop
    - icon: "structure"
      title: "Fonctionnalités documentaires natives"
      content: "Affichez des données à l'aide de tableaux, graphiques et codes-barres."

    # items loop
    - icon: "merge"
      title: "Tous les formats populaires"
      content: "Prend en charge tous les formats de documents couramment utilisés."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Générez des rapports bien personnalisés"
  description: "Exemples de code GroupDocs.Assembly"
  items:
    # code sample loop
    - title: "Utilisation de codes-barres générés"
      content: |
       GroupDocs.Assembly permet le balisage de codes-barres dans les modèles de rapport. Lors de la création d'un rapport, un code-barres est généré en fonction du balisage et des données fournies. Spécifiez le chemin vers le modèle contenant le texte, les objets de données et le balisage. Indiquez également la source de données pour remplir le code-barres avec du contenu.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Créer une instance de la classe DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Spécifiez le chemin vers le modèle
            var tmp_path = "barcode_template.docx";

            //Spécifiez le chemin pour le document résultant
            var res_path = "result.docx";

            //Créer une instance de la source de données
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Appelez AssembleDocument pour générer le rapport
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Créer une instance de la classe DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Spécifiez le chemin vers le modèle
            String tmp_path = "barcode_template.docx";

            //Spécifiez le chemin pour le document résultant
            String res_path = "result.docx";

            //Créer une instance de la source de données
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Appelez AssembleDocument pour générer le rapport
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // Créer une instance de la classe DocumentAssembler
            const assembler = new assemblyLib.DocumentAssembler();
            
            //Spécifiez le chemin vers le modèle
            const tmp_path = "barcode_template.docx";

            //Spécifiez le chemin pour le document résultant
            const res_path = "result.docx";

            //Créer une instance de la source de données
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // Appelez AssembleDocument pour générer le rapport
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Prise en charge de plus de 50 formats de fichiers"
  description: "GroupDocs.Assembly fonctionne avec presque tous les formats de fichiers populaires"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Nos statistiques produit"
  description: "Explorez les métriques du produit pour obtenir des informations sur nos progrès, notre impact et notre croissance."

  items:
    # items loop
    - number: "50+"
      title: "Formats pris en charge"
      content: "Nous prenons en charge plus de 50 des formats de documents les plus utilisés."

    # items loop
    - number: "650k"
      title: "Téléchargements NuGet"
      content: "GroupDocs.Assembly pour .NET est une bibliothèque populaire avec plus de 650 000 téléchargements sur NuGet."

    # items loop
    - number: "18k"
      title: "Téléchargements Maven"
      content: "Les développeurs Java ont téléchargé GroupDocs.Assembly sur Maven plus de 18 000 fois."

    # items loop
    - number: "150+"
      title: "Clients satisfaits"
      content: "Nos produits sont de confiance pour les développeurs individuels et les grandes entreprises à travers le monde pour créer des solutions innovantes."


############################# Customers ###############################
customers:
  enable: true
  title: "Nos clients satisfaits"
  description: "Les bibliothèques GroupDocs sont utilisées par certaines des marques les plus renommées et respectées au monde."

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
  title: "Prêt à commencer ?"
  description: "Testez les fonctionnalités de GroupDocs.Assembly gratuitement sur votre plateforme."

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
  title: "Questions Fréquemment Posées"
  description: "Parcourez nos questions fréquemment posées."

  items:
    # items loop
    - question: "Est-ce que GroupDocs.Assembly nécessite des bibliothèques externes pour la composition de documents ?"
      answer: "Non, GroupDocs.Assembly fonctionne de manière indépendante et ne nécessite pas de bibliothèques tierces comme Adobe Acrobat ou Microsoft Office."

    # items loop
    - question: "Puis-je tester les fonctionnalités de GroupDocs.Assembly avant d'acheter ?"
      answer: "Oui, vous pouvez ! GroupDocs.Assembly propose un essai gratuit. Installez-le et explorez ses fonctionnalités. La version d'essai ajoute des 'badges d'essai' à vos documents et ne traite que les 3 premières pages. Pour une expérience complète, obtenez une licence temporaire gratuite de 30 jours pour accéder à toutes les fonctionnalités. Plus de détails sont disponibles dans [licence temporaire](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quels types de licences sont disponibles ?"
      answer: "Vous recherchez une licence GroupDocs.Assembly ? Nous proposons une variété d'options pour répondre à vos besoins. Choisissez en fonction de la taille de votre équipe, de l'emplacement de déploiement (bureau unique ou à distance), et si vous devez partager le SDK/API avec des clients pour distribution. Alternativement, choisissez une licence d'utilisation mensuelle avec des plans à la mesure—payez uniquement pour ce que vous utilisez. Trouvez la meilleure option pour vous sous [tarification](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "APIs à faible code de GroupDocs.Assembly"
  description: "Générez des documents en utilisant votre application via notre API REST basée sur le cloud."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Utilisez l'API REST cURL pour ajouter des données à Word, Excel, PowerPoint, et de nombreux autres modèles."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Améliorez vos applications .NET en générant des rapports via le Cloud SDK. Affichez les données commerciales dans votre format personnalisé."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK offre différentes options pour les applications Java afin de générer divers types de documents."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Applications Web GroupDocs.Assembly"
  description: "GroupDocs.Assembly propose une application web gratuite pour générer des documents. Vous pouvez traiter plus de 50 formats de fichiers populaires directement dans votre navigateur, GRATUITEMENT."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Générez des rapports dans Excel, Word, PowerPoint et de nombreux autres types de fichiers directement depuis votre navigateur web."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Créez des documents Microsoft Word à partir de modèles et de sources de données."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Téléchargez un modèle et une source de données pour générer des rapports Excel gratuitement."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---