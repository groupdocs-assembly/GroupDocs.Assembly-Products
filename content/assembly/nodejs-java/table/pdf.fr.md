



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: fr
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Insérer des tableaux dans des documents PDF avec JavaScript"
head_description: "Utilisez GroupDocs.Assembly for Node.js via Java pour intégrer rapidement des tableaux dans des documents ou des emails, en tirant des données de diverses sources."

############################# Header ############################
title: "Ajoutez facilement des tableaux aux fichiers PDF avec Node.js" 
description: "Avec GroupDocs.Assembly for Node.js via Java, remplir des tableaux dans des documents PDF est simple, en utilisant des données provenant de plusieurs sources."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencez votre essai gratuit"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction à GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) est un outil puissant pour automatiser la création de documents. Il vous permet d'insérer des tableaux, des graphiques, des listes et des images dans des modèles, avec un placement précis du contenu. Prisant en charge plus de 50 formats de fichiers, y compris PDF, Word et email, il simplifie la génération de rapports et d'autres tâches.

############################# Steps ############################
steps:
    enable: true
    title: "Comment ajouter des données à un tableau dans PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) vous permet de remplir rapidement des modèles de tableau pour des fichiers PDF en utilisant des sources de données dynamiques.
      
      1. Créez un modèle avec des espaces réservés pour le tableau (les modèles PDF ne sont pas actuellement pris en charge).
      2. Chargez des données à partir d'une source prise en charge, comme JSON ou CSV.
      3. Organisez et formatez les données selon vos besoins.
      4. Exportez le document avec le tableau rempli au format PDF.
   
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
        // Inclure ces balises dans les espaces réservés de lignes de tableau de votre modèle
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Spécifiez le chemin du fichier modèle
        // Les modèles PDF ne sont pas pris en charge pour le moment.
        const template = "table_template.docx";

        // Chargez vos données à partir d'une source choisie
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Enregistrez le document final avec le tableau complété
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Ajoutez des tableaux dynamiques à vos documents"
  description: "GroupDocs.Assembly for Node.js via Java permet aux utilisateurs de créer automatiquement des tableaux, tout en intégrant des graphiques, des images et des listes grâce à des flux de travail basés sur des modèles."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Principales fonctionnalités de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Générer des tableaux à partir de données structurées"
      content: "Récupérez des données à partir de JSON, XML, CSV et d'autres formats pour peupler automatiquement des tableaux de documents."

    # feature loop
    - title: "Créer du contenu visuel soigné"
      content: "Utilisez GroupDocs.Assembly pour concevoir des tableaux, des graphiques et des listes professionnels, et ajoutez des liens, des images et du texte pour une apparence raffinée du document."

    # feature loop
    - title: "Placement dynamique du contenu des tableaux"
      content: "Ajoutez des lignes et des colonnes programmatiquement en utilisant des modèles basés sur LINQ, et personnalisez des styles comme les polices, les couleurs et l'alignement."

    # feature loop
    - title: "Fonctionne sans accroc à travers les formats"
      content: "Créez ou modifiez facilement des tableaux dans MS Office, OpenOffice, PDF, HTML et d'autres formats, en les intégrant dans des fichiers selon les besoins."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment peupler un tableau par programmation"
      content: |
        Cet exemple démontre le remplissage d'un tableau dans un document PDF avec des données provenant d'une source externe.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Concevez un modèle avec des espaces réservés pour le tableau
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Spécifiez le chemin du fichier vers le modèle
          // Les modèles PDF ne sont pas pris en charge pour le moment.
          const template = "table_template.docx";

          // Chargez les données nécessaires depuis votre source
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Organisez les données dans la structure nécessaire
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Initialisez DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Enregistrez le document de sortie avec le tableau complété
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    title: "Fonctionnalités clés en un coup d'œil"
    exclude: "table"
    description: "Notre API automatise la création de tableaux et améliore la génération de documents avec des outils et des modèles polyvalents."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Générer des tableaux dans une variété de formats"
    exclude: "PDF"
    description: "Avec Node.js via Java, remplissez des modèles et créez des tableaux complets à travers plus de 50 types de fichiers pris en charge."
    items: 
          
        # format loop 1
        - name: "Ajouter un tableau à un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Ajouter un tableau à un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ajouter un tableau à un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Ajouter un tableau à un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---