



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: fr
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Fusionner des documents en XLSX avec JavaScript"
head_description: "Combinez des fichiers XLSX rapidement avec JavaScript. GroupDocs.Assembly simplifie la fusion de documents en quelques étapes simples."

############################# Header ############################
title: "Combinez sans effort le contenu dans des fichiers XLSX" 
description: "Avec GroupDocs.Assembly for Node.js via Java, l'intégration d'un fichier XLSX dans un autre est rapide et précise. Profitez d'outils flexibles et fiables pour une fusion sans faille."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essayez-le gratuitement"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Aperçu de GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) offre une méthode puissante pour gérer les documents. Fusionnez un fichier dans un autre tout en prenant en charge plus de 50 formats, tels que PDF et MS Office. Personnalisez les mises en page, modifiez le contenu et organisez les documents exactement comme vous le souhaitez.

############################# Steps ############################
steps:
    enable: true
    title: "Comment fusionner un document dans un fichier XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilite l'insertion d'un fichier XLSX dans un autre avec des options personnalisables.
      
      1. Concevez un modèle XLSX avec des espaces réservés pour le contenu.
      2. Définissez le chemin du fichier pour le modèle.
      3. Fournissez le chemin du fichier à fusionner.
      4. Exportez le fichier final avec le contenu combiné.
   
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
        // Insérez cette balise dans votre modèle pour définir où le document sera intégré
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Définissez le chemin du fichier pour le modèle principal
        const template = "doc_template.xlsx";

        // Fournissez le chemin pour le document que vous souhaitez fusionner
        const data 
            = new assemblyLib.DataSourceInfo("insert.xlsx", "doc_expression");

        // Enregistrez la sortie finale avec le document intégré
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Outils puissants pour l'intégration de documents"
  description: "GroupDocs.Assembly for Node.js via Java facilite l'intégration de fichiers à travers divers formats de manière entièrement personnalisable. Fournissez des résultats cohérents et professionnels à chaque fois."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Générer des rapports avec des données commerciales"
      content: "Récupérez des données à partir de sources JSON, XML ou CSV pour créer rapidement et avec précision des rapports et des documents complets."

    # feature loop
    - title: "Ajouter des éléments visuels riches"
      content: "GroupDocs.Assembly vous permet d'inclure des tableaux, des graphiques, des listes, des images et des codes-barres aux côtés de texte et de liens hypertextes."

    # feature loop
    - title: "Placement de données précis"
      content: "Utilisez des modèles LINQ pour positionner les données exactement là où elles doivent être, gérez les éléments répétitifs comme les tableaux et personnalisez les styles sans effort."

    # feature loop
    - title: "Compatible avec une variété de formats"
      content: "Fusionnez le contenu de manière transparente à travers des formats tels que les fichiers PDF, MS Office, HTML et OpenOffice, offrant flexibilité pour tous les projets."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Intégrer une image dans un document par programme"
      content: |
        Cet exemple démontre comment insérer une image dans un fichier XLSX en utilisant GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Ajoutez un espace réservé dans le modèle pour l'image
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Spécifiez le chemin vers le fichier modèle
          const template = "template.xlsx";

          // Définissez le chemin vers l'image que vous souhaitez intégrer
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Initialisez l'objet DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Enregistrez le document avec l'image incluse
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "Fonctionnalités principales en un coup d'œil"
    exclude: "document"
    description: "Découvrez les outils complets que GroupDocs.Assembly offre pour une fusion de documents efficace et sans faille."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Combinez des documents dans de nombreux formats"
    exclude: "XLSX"
    description: "Utilisez Node.js via Java pour fusionner du contenu à travers plus de 50 formats de fichiers, garantissant des résultats professionnels et soignés."
    items: 
          
        # format loop 1
        - name: "Intégrer un document dans un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Intégrer un document dans un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Intégrer un document dans un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Intégrer un document dans un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---