



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: fr
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajoutez des tableaux aux documents DOCX en utilisant Java"
head_description: "Avec GroupDocs.Assembly for Java, les développeurs peuvent rapidement intégrer des tableaux dans des documents et des e-mails, en extrayant des données de sources dynamiques."

############################# Header ############################
title: "Remplissez des tableaux dans des fichiers DOCX avec notre API Java" 
description: "GroupDocs.Assembly for Java simplifie le processus de remplissage des tableaux dans les documents DOCX avec des données provenant de diverses sources."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenez votre essai gratuit"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) est un outil de génération de documents et de rapports en insérant automatiquement des données dans des modèles prédéfinis. Vous pouvez ajouter des tableaux, des listes, des graphiques et des images sans effort. Ses fonctionnalités avancées vous permettent de placer précisément le contenu dans vos documents. Compatible avec plus de 50 types de fichiers, y compris PDF, MS Office et formats de messagerie.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour insérer des données dans un tableau DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) vous aide à remplir des modèles de tableaux pour DOCX et d'autres formats. Utilisez des données dynamiques provenant de vos sources pour créer des tableaux sans effort.
      
      1. Configurez un modèle DOCX avec des espaces réservés pour les lignes et les colonnes du tableau.
      2. Récupérez des données de n'importe quelle source d'entrée prise en charge.
      3. Filtrez ou prétraitez les données pour répondre à vos besoins.
      4. Générez le document final avec le tableau complété.
   
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
        // Utilisez ces balises dans un espace réservé de ligne de tableau dans votre modèle
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Définissez le chemin vers le fichier modèle
        String template = "table_template.docx";

        // Chargez des données à partir de votre source choisie
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Enregistrez le fichier de sortie avec le tableau rempli
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Créez des documents avec des tableaux remplis de données"
  description: "GroupDocs.Assembly for Java facilite l'automatisation de la création de tableaux dans vos documents. Il prend également en charge l'ajout d'éléments tels que des graphiques, des listes et des images à l'aide de modèles."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Fonctionnalités principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Générez des rapports à partir de plusieurs formats de données"
      content: "L'API fonctionne sans problème avec JSON, XML, CSV et d'autres formats pour remplir des tableaux dans vos documents avec des données organisées."

    # feature loop
    - title: "Présentez les informations de manière visuelle"
      content: "GroupDocs.Assembly vous aide à créer des tableaux, des listes et des graphiques professionnels, ainsi qu'à insérer des liens, du texte et des images, pour un rendu soigné."

    # feature loop
    - title: "Placez le contenu des tableaux avec précision"
      content: "Utilisez une syntaxe flexible basée sur LINQ pour ajouter des lignes et des colonnes dynamiquement. Personnalisez l'apparence, comme les styles de police et les couleurs, par programmation."

    # feature loop
    - title: "Compatible avec plusieurs formats"
      content: "Travaillez avec MS Office, OpenOffice, PDF, HTML, et plus encore. Fusionnez des tableaux dans n'importe quel format de fichier pris en charge sans effort."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Créez dynamiquement un tableau rempli de données"
      content: |
        Cet exemple montre comment remplir un tableau dans un document DOCX en utilisant des données d'entrée dynamiques.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Conception d'un modèle avec un espace réservé pour le tableau
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Définissez l'emplacement du fichier modèle
          String template = "table_template.docx";

          // Chargez des données à partir de votre source préférée
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Préparez un objet de données contenant les champs nécessaires
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Créez une instance de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le document avec le tableau rempli
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    title: "Fonctionnalités clés en un coup d'œil"
    exclude: "table"
    description: "Notre API simplifie la création de documents professionnels en automatisant le peuplement des tableaux aux côtés d'autres composants puissants."
    items: 
          
        # operation loop 1
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "Créer et ajouter dynamiquement des codes-barres aux documents"

        # operation loop 2
        - name: "Visualiser des données avec des diagrammes"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "Remplir divers types de diagrammes avec des données"

        # operation loop 3
        - name: "Fusionner des documents"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "Combiner le contenu d'un document dans un autre"

        # operation loop 4
        - name: "Afficher des données avec des listes"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "Générer des listes dans les documents en utilisant des données spécifiques"

        # operation loop 5
        - name: "Organiser des données dans des tableaux"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "Récupérer des données de n'importe quelle source et peupler des tableaux"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produisez des tableaux détaillés dans divers formats"
    exclude: "DOCX"
    description: "Avec Java, vous pouvez remplir des modèles avec des données et générer des rapports détaillés dans plus de 50 types de fichiers."
    items: 
          
        # format loop 1
        - name: "Ajouter un tableau à un PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Ajouter un tableau à un DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ajouter un tableau à un PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Ajouter un tableau à un XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---