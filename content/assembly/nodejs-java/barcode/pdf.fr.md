



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:03:59
draft: false
lang: fr
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Ajouter des codes-barres aux fichiers PDF avec JavaScript"
head_description: "Générez et intégrez facilement des codes-barres dans vos documents et e-mails avec l'API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Créer des codes-barres pour les fichiers PDF avec Node.js" 
description: "Avec GroupDocs.Assembly for Node.js via Java, vous pouvez générer, personnaliser et intégrer dynamiquement des codes-barres dans des documents PDF."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencer"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction à GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) vous permet de créer des documents professionnels en combinant des données de plusieurs sources. Ajoutez des graphiques, des tableaux, des listes, des images et des codes-barres à vos fichiers. Utilisez des modèles pour organiser le contenu exactement où il doit être. Compatible avec plus de 50 formats, y compris PDF, documents Office et e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour ajouter un code-barres dans des fichiers PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) permet d'intégrer des codes-barres dans les documents PDF. Il prend en charge plus de 60 types de codes-barres, y compris les formats 1D et 2D.
      
      1. Concevez un modèle avec des espaces réservés pour les codes-barres (les modèles PDF ne sont pas pris en charge).
      2. Récupérez des données d'une source compatible.
      3. Définissez les options du code-barres telles que la taille et la résolution.
      4. Exportez le document avec le code-barres en tant que fichier PDF.
   
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
        // Utilisez cette balise dans le modèle pour inclure un code-barres dans le document de sortie
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Précisez le chemin vers le fichier modèle
        // Remarque : les modèles PDF ne sont actuellement pas pris en charge.
        const template = "barcode_template.docx";

        // Chargez les données requises depuis votre source
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Exportez le document avec le code-barres en tant que fichier PDF.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Générez des documents avec des modèles basés sur des données"
  description: "Avec GroupDocs.Assembly for Node.js via Java, vous pouvez créer des fichiers professionnels dans des formats populaires en intégrant sans effort des graphiques, tableaux, listes, liens, images et codes-barres."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Fonctionnalités principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Établir des rapports avec des données commerciales"
      content: "Utilisez l'API pour remplir rapidement et avec précision des modèles avec des données provenant de formats comme JSON, XML et CSV."

    # feature loop
    - title: "Ajouter des éléments visuels"
      content: "GroupDocs.Assembly prend en charge l'insertion d'éléments tels que des graphiques, des tableaux, des listes, du texte, des liens, des images et des codes-barres en temps réel."

    # feature loop
    - title: "Contrôler le placement des données"
      content: "Avec des modèles basés sur LINQ, vous pouvez positionner avec précision les données, parcourir des tableaux et appliquer un formatage personnalisé par programme."

    # feature loop
    - title: "Compatible avec de nombreux formats"
      content: "Travaillez avec des fichiers comme des documents MS Office, des PDF, HTML, fichiers OpenOffice et e-mails. Fusionnez plusieurs documents si nécessaire."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemple : Générer un code-barres par programme"
      content: |
        Cet exemple démontre comment générer par programme et insérer un code-barres dans un document PDF.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Concevez un modèle avec un espace réservé pour le code-barres
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Précisez le chemin du fichier modèle
          // Remarque : les modèles PDF ne sont actuellement pas pris en charge.
          const template = "barcode_template.docx";

          // Récupérez des données depuis votre source
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Créez un objet source de données avec les détails requis
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Initialisez une instance de DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Configurez les options du code-barres
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Enregistrez le document avec le code-barres inclus
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "Explorer les fonctionnalités clés"
    exclude: "barcode"
    description: "Simplifiez le traitement de documents avec des outils avancés et des capacités d'automatisation."
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
    title: "Formats de fichiers pris en charge pour la création de rapports"
    exclude: "PDF"
    description: "Node.js via Java gère plus de 50 types de fichiers, facilitant la fusion de données et le traitement de modèles pour des résultats de haute qualité."
    items: 
          
        # format loop 1
        - name: "Ajouter un code-barres à un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Ajouter un code-barres à un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ajouter un code-barres à un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Ajouter un code-barres à un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---