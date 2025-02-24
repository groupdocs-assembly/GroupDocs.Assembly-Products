



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:09
draft: false
lang: fr
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Créer des listes dans des documents PPTX en utilisant Java"
head_description: "Concevez et intégrez facilement des listes dynamiques dans vos modèles PPTX avec l'API GroupDocs.Assembly for Java."

############################# Header ############################
title: "Ajoutez des listes dynamiques aux fichiers PPTX avec notre API Java" 
description: "GroupDocs.Assembly for Java fournit des outils flexibles pour générer et insérer des listes riches en données directement dans des documents PPTX."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essayez gratuitement"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Assembly for Java ?"
    link: "/assembly/java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) facilite la conception de documents professionnels en extrayant des données de multiples sources. Utilisez-le pour créer des listes, des tableaux, des graphiques ou du texte, et placez ces éléments exactement où vous le souhaitez grâce à des fonctionnalités avancées de modèle. Avec le support de plus de 50 formats, y compris les fichiers PDF, MS Office et documents email, il aide à automatiser et rationaliser votre flux de travail.

############################# Steps ############################
steps:
    enable: true
    title: "Comment ajouter une liste basée sur des données à un document PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) vous permet d'insérer rapidement des listes riches en données dans des modèles PPTX. Personnalisez et organisez le contenu sans difficulté.
      
      1. Créez un modèle PPTX et marquez les emplacements des espaces réservés pour la liste.
      2. Définissez le chemin d'accès au modèle.
      3. Récupérez les données à partir de formats supportés comme JSON ou XML.
      4. Enregistrez le document final avec la liste ajoutée.
   
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
        // Incluez cette balise dans votre modèle à l'endroit où la liste doit apparaître
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Définissez le chemin d'accès du modèle
        String template = "list_template.pptx";

        // Tirez des données de votre source choisie
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Enregistrez le document avec la liste intégrée
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Générez des documents à partir de modèles avec intégration de données"
  description: "GroupDocs.Assembly for Java simplifie l'ajout de listes dynamiques, de tableaux, de graphiques et d'autres composants dans les modèles de documents."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Construisez des rapports avec des données provenant de diverses sources"
      content: "Utilisez des données provenant de formats comme JSON, XML et CSV pour peupler efficacement les listes et autres composants."

    # feature loop
    - title: "Ajoutez des listes et d'autres éléments de données de manière fluide"
      content: "GroupDocs.Assembly permet d'incorporer des listes, des graphiques, des tableaux, et plus encore, aux côtés de texte, d'images et de liens pour créer des documents soignés."

    # feature loop
    - title: "Contrôlez précisément où les données apparaissent"
      content: "Les modèles basés sur LINQ vous permettent de définir des emplacements exacts pour vos listes et données. Utilisez des boucles pour créer automatiquement des listes détaillées et appliquer un formatage personnalisé."

    # feature loop
    - title: "Prend en charge divers formats de documents"
      content: "Créez ou éditez des fichiers dans des formats tels que MS Office, PDF, OpenOffice, HTML et email. Fusionnez le contenu de plusieurs documents selon vos besoins."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment créer une liste par programmation"
      content: |
        Cet exemple montre comment ajouter dynamiquement une liste dans un fichier PPTX en utilisant GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Ajoutez une balise d'espace réservé dans votre modèle pour la liste
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Fournissez le chemin d'accès à votre modèle
          String template = "numlist_template.pptx";

          // Tirez les données nécessaires pour peupler la liste
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Préparez la source de données avec les détails requis
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Initialisez DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le document de sortie avec la liste complétée
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "Découvrez ce que GroupDocs.Assembly peut faire"
    exclude: "list"
    description: "Concevez et générez facilement des documents riches en contenu avec des outils d'intégration de données avancés."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produisez des documents dans divers formats"
    exclude: "PPTX"
    description: "Java prend en charge plus de 50 formats, vous permettant de créer des documents structurés en combinant des données et des modèles."
    items: 
          
        # format loop 1
        - name: "Créer une liste dans un PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Créer une liste dans un DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Créer une liste dans un PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Créer une liste dans un XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---