



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: fr
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Insérer des graphiques dans des fichiers PPTX avec JavaScript"
head_description: "Avec GroupDocs.Assembly for Node.js via Java, les développeurs peuvent rapidement créer et intégrer des graphiques dynamiques dans des documents utilisant des sources de données en direct."

############################# Header ############################
title: "Ajoutez des graphiques à des fichiers PPTX en utilisant Node.js" 
description: "GroupDocs.Assembly for Node.js via Java simplifie le processus d'intégration de graphiques dans des documents PPTX avec des entrées de données en temps réel."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencez gratuitement aujourd'hui"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Présentation de GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) est une solution robuste pour la création de documents automatisés et de rapports. Ajoutez des graphiques, des tableaux, des images, des codes-barres et des listes aux fichiers avec précision. Cette plateforme polyvalente prend en charge plus de 50 formats, y compris les PDF, les documents Office et les e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour ajouter un graphique à un document PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilite l'ajout de graphiques aux fichiers PPTX. Choisissez parmi des types de graphiques tels que les graphiques à barres, linéaires ou circulaires.
      
      1. Concevez un modèle PPTX avec des espaces réservés pour les graphiques.
      2. Chargez les données d'une source prise en charge.
      3. Configurez les options du graphique, y compris le type, les couleurs et les étiquettes.
      4. Exportez le document avec le graphique intégré.
   
    code:
      platform: "java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Document d'exemple"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Incluez ce tag dans votre modèle pour générer un graphique
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Spécifiez le chemin du fichier modèle
        const template = "chart_template.pptx";

        // Extrayez les données de votre système source
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Enregistrez le document final avec le graphique intégré
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Intégrez sans effort des graphiques dans vos documents"
  description: "GroupDocs.Assembly for Node.js via Java facilite la génération de documents riches en fonctionnalités dans des types de fichiers populaires. Utilisez des modèles pour ajouter des graphiques, des tableaux, des codes-barres, des listes, des images, et plus encore avec des mises à jour de données en temps réel."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Caractéristiques principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Transformez les données en graphiques professionnels"
      content: "Convertissez des données provenant de sources telles que JSON, XML ou CSV en graphiques de haute qualité pouvant être intégrés directement dans des documents."

    # feature loop
    - title: "Créez des visuels époustouflants"
      content: "Générez des graphiques à barres, des graphiques circulaires et des graphiques linéaires qui s'intègrent parfaitement aux autres éléments des documents comme des images, des tableaux et des codes-barres."

    # feature loop
    - title: "Style et placement flexibles des graphiques"
      content: "Utilisez des modèles LINQ pour contrôler le positionnement et le style des graphiques, y compris les couleurs, les mises en page et les étiquettes, pour une présentation impeccable."

    # feature loop
    - title: "Prend en charge de nombreux formats de fichiers"
      content: "Générez des documents dans des formats tels que MS Office, PDF, OpenOffice et HTML, avec des graphiques parfaitement intégrés pour un rendu professionnel."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Générez et insérez des graphiques dynamiquement"
      content: |
        Cet exemple illustre comment créer et intégrer des graphiques dans des fichiers PPTX par programmation.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Configurez un modèle avec un espace réservé pour le graphique
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Définissez le chemin d'accès au fichier modèle
          const template = "table_template.pptx";

          // Récupérez les données d'une source choisie
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Préparez un objet de données contenant les informations du graphique
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Choisissez le type de graphique et personnalisez son apparence
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Initialisez DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Enregistrez le document mis à jour avec le graphique intégré
          asm.assembleDocument(template, "result.pptx", data, design);
          ```
        platform: "java"
        copy_title: "Copier"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.pptx"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Découvrez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Télécharger depuis NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "En savoir plus sur les licences"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez des fonctionnalités avancées"
    exclude: "chart"
    description: "Cette plateforme simplifie la création de documents avec des outils conçus pour la visualisation de données et l'intégration fluide."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Générez des rapports dans plusieurs formats de fichiers"
    exclude: "PPTX"
    description: "Node.js via Java prend en charge plus de 50 formats, facilitant ainsi la combinaison de modèles avec des données pour produire des documents soignés."
    items: 
          
        # format loop 1
        - name: "Graphiques dans PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Graphiques dans DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Graphiques dans PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Graphiques dans XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---