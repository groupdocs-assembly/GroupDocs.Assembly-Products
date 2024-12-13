



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: fr
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Générez des graphiques dans des documents PDF en utilisant Java"
head_description: "L'API GroupDocs.Assembly for Java permet aux développeurs de créer et d'insérer des graphiques dynamiques ou des diagrammes dans des documents de manière transparente, alimentés par des données en temps réel."

############################# Header ############################
title: "Ajoutez des graphiques aux documents PDF avec l'API Java" 
description: "GroupDocs.Assembly for Java simplifie le processus d'intégration de graphiques dans des documents PDF en utilisant des données en temps réel."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencez gratuitement"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction à GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) est une solution polyvalente pour automatiser la création de documents et de rapports. Elle vous permet d'ajouter des graphiques, des tableaux, des listes, des codes-barres et des images directement dans vos fichiers, avec des outils avancés pour un formatage précis et une intégration des données. La plateforme prend en charge plus de 50 formats, y compris PDF, fichiers Microsoft Office et e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour intégrer un graphique dans un document PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) simplifie le processus d'insertion de graphiques dans des modèles PDF. Choisissez parmi une variété de styles de graphiques, y compris les graphiques en barres, en secteurs et en lignes.
      
      1. Créez un modèle avec des espaces réservés pour le graphique (les modèles PDF ne sont pas pris en charge).
      2. Chargez vos données depuis une source compatible.
      3. Définissez les options du graphique, telles que le type, les étiquettes et les couleurs.
      4. Enregistrez le document contenant le graphique en tant que fichier PDF.
   
    code:
      platform: "java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Document d'exemple"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Ajoutez ce tag à votre modèle pour inclure un graphique
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Fournissez le chemin d'accès à votre modèle
        // Les modèles PDF ne sont pas pris en charge pour le moment.
        String template = "chart_template.docx";

        // Extraire les données nécessaires de votre source
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Enregistrez le document final avec le graphique intégré
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Intégrez sans effort des graphiques dynamiques dans vos documents"
  description: "GroupDocs.Assembly for Java offre un moyen simple de créer des documents riches en données dans des formats populaires. Utilisez des modèles pour insérer des graphiques, des tableaux, des codes-barres, des listes, des liens et des images avec des mises à jour dynamiques provenant de vos données."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Transformez facilement des données en graphiques"
      content: "Utilisez l'API pour transformer des données provenant de JSON, XML, CSV ou d'autres sources en graphiques propres et professionnels pour vos documents."

    # feature loop
    - title: "Créez un contenu visuellement percutant"
      content: "GroupDocs.Assembly prend en charge divers formats visuels, y compris des graphiques en barres, des graphiques à secteurs et des graphiques linéaires, qui peuvent être combinés avec des tableaux, des codes-barres, des images, et plus encore pour des rapports améliorés."

    # feature loop
    - title: "Placement et style de graphiques personnalisables"
      content: "Avec une syntaxe basée sur LINQ, vous pouvez générer et positionner dynamiquement des graphiques dans le document, tout en ajustant facilement les styles, les couleurs et les mises en page pour répondre à vos besoins de conception."

    # feature loop
    - title: "Prend en charge plusieurs formats de documents"
      content: "Générez des documents dans des formats tels que MS Office, PDF, OpenOffice et HTML. Les graphiques s'intègrent parfaitement dans tout format pris en charge pour des résultats professionnels."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Générez et intégrez des graphiques par programmation"
      content: |
        Cet exemple montre comment créer et intégrer un graphique dans un document PDF par programmation.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Préparez un modèle avec un espace réservé pour le graphique
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Spécifiez le chemin d'accès au modèle
          // Les modèles PDF ne sont pas pris en charge pour le moment.
          String template = "table_template.docx";

          // Chargez les données de votre source choisie
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Créez un objet de données avec les informations pertinentes
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configurez le type et l'apparence du graphique
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Initialisez DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le document final avec le graphique intégré
          asm.assembleDocument(template, "result.pdf", data, design);
          ```
        platform: "java"
        copy_title: "Copier"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.pdf"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Découvrez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Télécharger depuis Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "En savoir plus sur les licences"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explorez des capacités puissantes"
    exclude: "chart"
    description: "Cette plateforme simplifie le processus de conception de documents attrayants et axés sur les données, adaptés à vos besoins."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Générez des rapports complets dans divers formats"
    exclude: "PDF"
    description: "Java vous permet de créer des documents avec des graphiques intégrés dans plus de 50 formats de fichiers, garantissant une fusion transparente des modèles et des données."
    items: 
          
        # format loop 1
        - name: "Graphiques dans PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Graphiques dans DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Graphiques dans PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Graphiques dans XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---