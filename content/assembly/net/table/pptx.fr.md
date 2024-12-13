



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: fr
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Créer des tables dans des documents PPTX avec C#"
head_description: "L'API GroupDocs.Assembly for .NET permet aux développeurs d'ajouter et de remplir sans effort des tables dans des documents et des e-mails avec des données provenant de sources dynamiques."

############################# Header ############################
title: "Générer des tables de données dans des documents PPTX en utilisant notre API .NET" 
description: "GroupDocs.Assembly for .NET permet de remplir dynamiquement des tables dans des documents PPTX avec des données de diverses sources."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger l'essai gratuit"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Aperçu de GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) est conçu pour créer des documents et des rapports en remplissant des modèles avec des données provenant de plusieurs sources. Insérez sans effort des données structurées dans des tables, listes et graphiques, ou intégrez dynamiquement des images. Une syntaxe avancée garantit un placement précis des données. Prend en charge plus de 50 formats, y compris les PDF, documents MS Office et fichiers e-mail.

############################# Steps ############################
steps:
    enable: true
    title: "Comment peupler une table dans un document PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) vous permet de peupler dynamiquement des tables dans des modèles pour des formats comme PPTX. Insérez des données provenant de diverses sources dans vos tables.
      
      1. Créez un modèle PPTX avec des espaces réservés pour la table.
      2. Récupérez des données depuis n'importe quelle source prise en charge.
      3. Filtrez les données pour inclure uniquement les informations nécessaires.
      4. Enregistrez le document avec la table peuplée.
   
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
        // Ajoutez ces balises dans une ligne de table de modèle
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Définissez le chemin du fichier pour le modèle
        string template = "table_template.pptx";

        // Récupérez les données d'une source prise en charge
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Enregistrez le document avec la table remplie de données
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Générez des documents avec des tables dynamiques"
  description: "GroupDocs.Assembly for .NET simplifie la création de documents en automatisant le peuplement des tables et en prenant en charge des éléments supplémentaires comme des graphiques, des listes et des images via des modèles et une balisage avancé."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Créer des rapports à partir de données structurées"
      content: "L'API traite les données provenant de sources telles que JSON, XML et CSV pour remplir efficacement et avec précision les tables dans les documents bureautiques."

    # feature loop
    - title: "Afficher les données visuellement"
      content: "GroupDocs.Assembly permet la création de tables, listes et graphiques, ainsi que l'intégration de textes, liens et images pour un design professionnel des documents."

    # feature loop
    - title: "Positionner avec précision les données des tables"
      content: "Utilisez une syntaxe basée sur LINQ pour ajouter dynamiquement des lignes et des colonnes dans les tables. Personnalisez les styles, y compris les couleurs et la mise en forme, par programmation."

    # feature loop
    - title: "Prend en charge une large gamme de formats"
      content: "Gérez facilement des formats de fichiers populaires comme MS Office, OpenOffice, PDF et HTML. Insérez en toute transparence des tables peuplées dans les types de documents pris en charge."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment peupler dynamiquement une table de données"
      content: |
        Cet exemple démontre comment remplir une table dans un document PPTX en utilisant des données dynamiques.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Préparez un modèle avec un espace réservé pour la table
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Spécifiez le chemin du fichier vers le modèle
          string template = "table_template.pptx";

          // Récupérez les données de votre source choisie
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Créez un objet source de données avec les données nécessaires
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Initialisez DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le document finalisé avec la table peuplée
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "Explorez les fonctionnalités clés"
    exclude: "table"
    description: "Notre solution simplifie la création de documents professionnels avec des tables peuplées dynamiquement et d'autres éléments."
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
    title: "Créer des rapports avec des tables détaillées"
    exclude: "PPTX"
    description: ".NET permet la création de rapports complets en remplissant des modèles avec des tables et d'autres éléments de données dans plus de 50 formats pris en charge."
    items: 
          
        # format loop 1
        - name: "Ajouter un tableau à un PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Ajouter un tableau à un DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ajouter un tableau à un PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Ajouter un tableau à un XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---