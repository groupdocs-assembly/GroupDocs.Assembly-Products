



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: fr
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Créez des graphiques dans des fichiers PPTX avec C#"
head_description: "L'API GroupDocs.Assembly for .NET permet aux développeurs de générer et d'insérer des graphiques ou des diagrammes dans des documents de manière dynamique en utilisant des données en temps réel."

############################# Header ############################
title: "Intégrez des graphiques dans des fichiers PPTX avec l'API .NET" 
description: "GroupDocs.Assembly for .NET offre un moyen puissant de remplir des fichiers PPTX avec des données dynamiques et d'intégrer des graphiques sans effort."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essayer Gratuitement"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Assembly for .NET ?"
    link: "/assembly/net/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) est un outil conçu pour rationaliser la création de documents et de rapports en intégrant des données provenant de diverses sources. Générez des graphiques, des tableaux, des listes, des codes-barres et des images de manière dynamique. Des options de formatage avancées permettent un placement et une personnalisation précis de votre contenu. Il prend en charge plus de 50 formats de fichiers, y compris les PDF, les documents MS Office et les courriels.

############################# Steps ############################
steps:
    enable: true
    title: "Comment ajouter un graphique à un document PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilite la génération et l'intégration de graphiques dans vos modèles PPTX. Prend en charge une variété de types de graphiques, tels que des graphiques à barres, circulaires et linéaires.
      
      1. Concevez un modèle PPTX avec des espaces réservés pour les graphiques.
      2. Récupérez vos données à partir d'une source compatible.
      3. Définissez les options de graphique telles que le type, les étiquettes et le schéma de couleurs.
      4. Enregistrez le fichier mis à jour avec le graphique intégré.
   
    code:
      platform: "net"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Document d'exemple"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Incluez cette balise dans votre modèle pour générer un graphique
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Spécifiez le chemin du fichier pour votre modèle
        string template = "chart_template.pptx";

        // Chargez des données depuis votre source préférée
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Enregistrez le document avec le graphique intégré
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ajoutez des graphiques dynamiques à vos documents sans effort"
  description: "GroupDocs.Assembly for .NET simplifie la création de documents basés sur des données dans des formats largement utilisés. Utilisez des modèles pour insérer des graphiques, des tableaux, des codes-barres, des listes, des hyperliens et des images avec une intégration de données dynamique avancée."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Convertir des données en graphiques professionnels"
      content: "Transformez les données provenant de JSON, XML, CSV, et d'autres sources en graphiques attrayants en quelques étapes grâce à notre API."

    # feature loop
    - title: "Créer un contenu visuellement engageant"
      content: "GroupDocs.Assembly prend en charge plusieurs types de graphiques tels que des graphiques à barres, des graphiques circulaires et des graphiques linéaires. Combinez-les avec des tableaux, des codes-barres, des images et d'autres éléments pour créer des rapports professionnels."

    # feature loop
    - title: "Positionner et personnaliser les graphiques avec précision"
      content: "Avec la syntaxe LINQ, vous pouvez générer et placer les graphiques dynamiquement exactement là où ils sont nécessaires. Personnalisez facilement les styles, les couleurs et la mise en page pour répondre à vos exigences."

    # feature loop
    - title: "Compatible avec divers formats de fichiers"
      content: "Produisez des documents dans des formats populaires tels que MS Office, PDF, OpenOffice et HTML. Intégrez des graphiques de manière transparente dans tout format pris en charge avec une compatibilité totale."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Créer un graphique par programme"
      content: |
        Cet exemple démontre comment créer et intégrer dynamiquement un graphique dans un document PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Préparez un modèle avec un espace réservé pour le graphique
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Fournissez le chemin vers le fichier modèle
          string template = "table_template.pptx";

          // Récupérez les données de votre source
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Construisez un objet de données avec les informations nécessaires
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configurez les propriétés du graphique telles que le type et l'apparence
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Initialisez DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Exportez le document avec le graphique inclus
          asm.AssembleDocument(template, "result.pptx", data, design);
          ```
        platform: "net"
        copy_title: "Copier"
        install:
          command: "dotnet add package GroupDocs.Assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Découvrez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Télécharger depuis Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "En savoir plus sur les licences"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez les capacités clés"
    exclude: "chart"
    description: "Notre plateforme vous aide à créer des documents captivants, basés sur des données, adaptés à vos besoins."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Créez des rapports visuellement riches dans plusieurs formats"
    exclude: "PPTX"
    description: ".NET vous permet de générer des documents avec des graphiques intégrés dans plus de 50 formats pris en charge, combinant des modèles avec vos données de manière transparente."
    items: 
          
        # format loop 1
        - name: "Graphiques dans PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Graphiques dans DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Graphiques dans PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Graphiques dans XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---