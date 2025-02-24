



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: fr
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Intégrer un document dans un autre au format DOCX avec l'API C#"
head_description: "Fusionnez les documents DOCX en utilisant C#. Avec GroupDocs.Assembly, combinez les fichiers de manière fluide en quelques étapes."

############################# Header ############################
title: "Combinez des documents au format DOCX" 
description: "Avec GroupDocs.Assembly for .NET, vous pouvez rapidement intégrer un document DOCX dans un autre. Cette API offre des outils performants pour un rapprochement précis des documents."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Assembly for .NET ?"
    link: "/assembly/net/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) est un outil puissant pour la composition et la manipulation de documents. Il permet aux utilisateurs d'incorporer un document dans un autre, facilitant ainsi la fusion de contenu. Avec le support de plus de 50 formats, y compris les fichiers PDF, MS Office, et bien d'autres, vous pouvez organiser, éditer et personnaliser le résultat final selon vos besoins.

############################# Steps ############################
steps:
    enable: true
    title: "Comment fusionner un document dans un fichier DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) vous permet d'incorporer un document dans un autre fichier DOCX sans effort. Fusionnez et personnalisez le contenu de manière fluide.
      
      1. Concevez un modèle DOCX avec des espaces réservés pour le document intégré.
      2. Définissez le chemin d'accès au fichier pour le modèle.
      3. Spécifiez le chemin d'accès du document à intégrer.
      4. Enregistrez le fichier final avec le contenu intégré.
   
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
        // Ajoutez cette balise à votre modèle pour marquer le point d'insertion
        // <<doc [doc_expression]>>

        // Spécifiez le chemin du fichier pour le modèle
        string template = "doc_template.docx";

        // Fournissez le chemin du document à intégrer
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Enregistrez le document fusionné
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimisez la fusion de documents avec des outils avancés"
  description: "La bibliothèque GroupDocs.Assembly for .NET simplifie l'intégration d'un document dans un autre, prenant en charge divers formats de fichiers et offrant des options de personnalisation pour une intégration fluide."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Fonctionnalités Clés de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Générez des rapports à partir de vos données professionnelles"
      content: "Remplissez automatiquement les documents avec des données provenant de JSON, XML, CSV ou d'autres sources, garantissant des flux de travail précis et efficaces."

    # feature loop
    - title: "Enrichissez les documents avec des éléments visuels"
      content: "GroupDocs.Assembly vous permet d'inclure des tableaux, des graphiques et des listes, ainsi que du texte, des liens, des images et des codes-barres générés dynamiquement."

    # feature loop
    - title: "Placez et formatez les données avec précision"
      content: "Les modèles basés sur LINQ vous donnent le contrôle sur le placement des données, vous permettant de gérer des boucles pour des tableaux et d'appliquer des styles tels que la personnalisation des couleurs."

    # feature loop
    - title: "Compatible avec plusieurs formats de fichiers"
      content: "Intégrez aisément des documents les uns dans les autres à travers des formats tels que MS Office, PDF, HTML, OpenOffice, et plus encore."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment intégrer une image dans un document par programme"
      content: |
        Cet exemple démontre comment insérer une image dans un document DOCX en utilisant GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Ajoutez une balise de remplissage à votre modèle
          // <<image [expression]>>

          // Spécifiez le chemin d'accès au fichier pour le modèle
          string template = "template.docx";

          // Définissez le chemin d'accès au fichier image
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Initialisez une instance de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le document avec l'image intégrée
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "Découvrez nos outils puissants"
    exclude: "document"
    description: "Explorez les fonctionnalités que GroupDocs.Assembly offre pour intégrer et fusionner des documents avec précision."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Fusionnez des documents dans divers formats"
    exclude: "DOCX"
    description: "Avec l'API .NET, vous pouvez combiner des documents dans plus de 50 formats pris en charge. Intégrez sans effort des fichiers ou des sections dans vos documents finaux."
    items: 
          
        # format loop 1
        - name: "Intégrer un document dans un PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Intégrer un document dans un DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Intégrer un document dans un PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Intégrer un document dans un XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---