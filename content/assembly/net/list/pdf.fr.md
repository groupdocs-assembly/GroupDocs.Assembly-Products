



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: fr
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Générez des listes dans des documents PDF avec C#"
head_description: "L'API GroupDocs.Assembly for .NET permet aux développeurs de créer et d'intégrer dynamiquement des listes remplies de données dans des documents et des modèles."

############################# Header ############################
title: "Ajoutez des listes basées sur des données aux documents PDF en utilisant notre API .NET" 
description: "GroupDocs.Assembly for .NET offre des outils puissants pour générer et intégrer dynamiquement des listes dans des documents PDF."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez l'Essai Gratuit"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Présentation de GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) est conçu pour rationaliser la création de documents et de rapports en intégrant facilement des données de diverses sources. Remplissez des modèles avec des listes, des graphiques, des tableaux, des codes-barres ou du texte, et placez le contenu précisément à l'aide de balisage avancé. Avec le support de plus de 50 formats — y compris les fichiers PDF, MS Office, et les e-mails — c'est idéal pour automatiser les workflows de documents.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour ajouter une liste remplie de données à un document PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilite l'insertion de listes basées sur des données dans des modèles PDF. Créez et personnalisez des listes efficacement.
      
      1. Créez un modèle avec des emplacements désignés pour la liste (Les modèles PDF ne sont actuellement pas pris en charge).
      2. Définissez le chemin d'accès au modèle.
      3. Récupérez des données à partir de sources prises en charge telles que JSON ou XML.
      4. Exportez le document final avec la liste au format PDF.
   
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
        // Ajoutez cette balise à votre modèle pour marquer où la liste apparaîtra
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Spécifiez le chemin vers le fichier modèle
        // Le support des modèles PDF n'est pas disponible pour le moment.
        string template = "list_template.docx";

        // Récupérez les données de votre source choisie
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Enregistrez le document avec la liste générée
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Créez des documents en remplissant des modèles avec des données structurées"
  description: "GroupDocs.Assembly for .NET simplifie la construction de documents basés sur des données. Ajoutez dynamiquement des listes, des tableaux, des codes-barres, des graphiques, des images et d'autres éléments avec des modèles avancés."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Fonctionnalités de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Générez des rapports à partir de données commerciales"
      content: "L'API remplit des documents dans des formats populaires en utilisant des données provenant de sources comme JSON, XML, CSV, etc. avec précision et efficacité."

    # feature loop
    - title: "Utilisez des listes et d'autres éléments pour présenter des données"
      content: "GroupDocs.Assembly vous permet d'intégrer des listes, des tableaux et des graphiques avec du texte, des codes-barres, des hyperliens et des images pour créer des documents bien structurés."

    # feature loop
    - title: "Insérez des données précisément là où c'est nécessaire"
      content: "Exploitez une syntaxe basée sur LINQ pour positionner les listes et d'autres éléments de données avec précision. Utilisez des boucles pour peupler des listes dynamiquement et appliquez un formatage personnalisé par programmation."

    # feature loop
    - title: "Prend en charge plusieurs formats de documents"
      content: "Générez et gérez des documents dans divers formats tels que MS Office, OpenOffice, PDF, HTML et fichiers d'e-mail. Intégrez facilement plusieurs documents en un seul."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment générer une liste dynamiquement"
      content: |
        Cet exemple démontre comment intégrer une liste générée dynamiquement dans un document PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Ajoutez une balise de remplacement à votre modèle pour la liste
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Spécifiez le chemin vers le fichier modèle
          // Le support des modèles PDF n'est pas disponible pour le moment.
          string template = "numlist_template.docx";

          // Récupérez les données pour remplir la liste
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Créez un objet source de données avec les informations nécessaires
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Initialisez DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le document final avec la liste générée
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    exclude: "list"
    description: "Notre plateforme est conçue pour simplifier la création et l'intégration de contenu documentaire basé sur des données."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Créez des documents structurés dans des formats populaires"
    exclude: "PDF"
    description: ".NET prend en charge plus de 50 formats, ce qui vous permet de fusionner facilement des données et des modèles pour produire des résultats soignés et structurés."
    items: 
          
        # format loop 1
        - name: "Créer une liste dans un PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Créer une liste dans un DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Créer une liste dans un PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Créer une liste dans un XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---