



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: fr
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Créer des listes dynamiques en DOCX avec JavaScript"
head_description: "Concevez et insérez facilement des listes dans des modèles DOCX en utilisant l'API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Intégrez des listes pilotées par les données dans des fichiers DOCX avec Node.js" 
description: "GroupDocs.Assembly for Node.js via Java offre des outils puissants pour ajouter des listes flexibles alimentées par des données dans des documents DOCX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencer gratuitement"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "À propos de GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) simplifie la création de documents en extrayant des données provenant de diverses sources et en les intégrant dans des modèles. Utilisez-le pour créer des listes, des tableaux, des graphiques et d'autres éléments, avec des options de positionnement et de mise en forme précises. Supportant plus de 50 formats, y compris PDF, MS Office, et emails, il aide à automatiser votre processus de génération de documents.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour insérer une liste dans un fichier DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilite l'ajout de listes détaillées et pilotées par les données à vos modèles DOCX.
      
      1. Créez un modèle DOCX et définissez des espaces réservés pour la liste.
      2. Fournissez le chemin d'accès du fichier du modèle.
      3. Chargez des données à partir de sources prises en charge comme JSON ou XML.
      4. Enregistrez le document avec la liste générée.
   
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
        // Placez cette balise dans votre modèle pour indiquer où la liste sera insérée
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Définissez le chemin d'accès du fichier pour votre modèle
        const template = "list_template.docx";

        // Récupérez les données de la source que vous souhaitez utiliser
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Enregistrez le fichier avec la liste intégrée
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Générez facilement des documents avec des données intégrées"
  description: "Avec GroupDocs.Assembly for Node.js via Java, vous pouvez intégrer des listes, des tableaux, des graphiques et d'autres éléments dans des modèles, économisant ainsi du temps et des efforts."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Points forts de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Générez des rapports à partir de plusieurs sources de données"
      content: "Importez des données à partir de JSON, XML, CSV, ou d'autres formats pour remplir efficacement des listes et d'autres composants."

    # feature loop
    - title: "Ajoutez des listes et d'autres éléments visuels"
      content: "GroupDocs.Assembly vous permet d'incorporer sans effort des listes, des tableaux, des graphiques et plus encore aux côtés de textes, d'images et de liens pour un résultat soigné."

    # feature loop
    - title: "Placez et stylisez les données avec précision"
      content: "Des modèles basés sur LINQ vous permettent de contrôler exactement où apparaissent les listes et d'autres données, d'utiliser des boucles pour les éléments répétés et de personnaliser les styles selon vos besoins."

    # feature loop
    - title: "Fonctionne avec plusieurs formats"
      content: "Créez des documents dans des formats tels que MS Office, PDF, OpenOffice, HTML, et emails. Fusionnez le contenu de diverses sources dans un seul fichier."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Créer une liste dans un document par programmation"
      content: |
        Cet exemple montre comment ajouter dynamiquement une liste à un document DOCX en utilisant GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Ajoutez un espace réservé dans votre modèle pour la liste
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Spécifiez le chemin d'accès du modèle
          const template = "numlist_template.docx";

          // Chargez les données pour remplir la liste
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Préparez la source de données avec les détails nécessaires
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Initialisez le DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Enregistrez le document final avec la liste incluse
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "Explorez les fonctionnalités de GroupDocs.Assembly"
    exclude: "list"
    description: "Concevez et générez des documents riches en données sans effort en utilisant des outils d'intégration puissants."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Créez des documents dans plusieurs formats"
    exclude: "DOCX"
    description: "Node.js via Java prend en charge plus de 50 formats de fichiers, facilitant la fusion de modèles et de données dans des résultats professionnels."
    items: 
          
        # format loop 1
        - name: "Créer une liste dans un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Créer une liste dans un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Créer une liste dans un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Créer une liste dans un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---