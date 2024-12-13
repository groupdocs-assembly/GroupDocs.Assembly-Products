



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: fr
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Insérer un document dans un autre en DOCX à l'aide de Java"
head_description: "Combinez des fichiers DOCX avec Java. GroupDocs.Assembly simplifie le processus de fusion de documents en seulement quelques lignes de code."

############################# Header ############################
title: "Intégrez du contenu dans des fichiers DOCX sans effort" 
description: "Utilisez GroupDocs.Assembly for Java pour insérer facilement un document DOCX dans un autre. Obtenez des résultats précis avec des outils flexibles et fiables."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenez-le gratuitement"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Assembly for Java ?"
    link: "/assembly/java/"
    link_title: "En savoir plus"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) est une solution polyvalente pour la gestion de documents. Elle vous permet d'intégrer un document dans un autre, prenant en charge plus de 50 formats tels que des PDF et des fichiers MS Office. Personnalisez votre sortie en fusionnant, modifiant et organisant le contenu exactement comme vous le souhaitez.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour insérer un document dans un fichier DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) rend l'insertion d'un document DOCX dans un autre simple et personnalisable.
      
      1. Préparez un modèle DOCX avec des espaces réservés pour le contenu intégré.
      2. Spécifiez le chemin du fichier pour le modèle.
      3. Indiquez le chemin du document à intégrer.
      4. Enregistrez le fichier de sortie avec le contenu fusionné.
   
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
        // Utilisez cette balise dans votre modèle pour marquer l'emplacement du document intégré
        // <<doc [doc_expression]>>

        // Définissez le chemin du fichier pour le modèle principal
        String template = "doc_template.docx";

        // Indiquez le chemin du document que vous souhaitez insérer
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Enregistrez le fichier final avec le contenu intégré
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Outils avancés pour simplifier l'intégration de documents"
  description: "Avec GroupDocs.Assembly for Java, l'intégration de documents est simple et personnalisable, peu importe le type de fichier. Obtenez des résultats clairs et cohérents dans vos projets."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Fonctionnalités de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Créer des rapports à l'aide de données commerciales"
      content: "Remplissez les documents avec des données provenant de sources comme JSON, XML ou CSV rapidement et de manière fiable, rationalisant ainsi vos flux de travail."

    # feature loop
    - title: "Améliorer les documents avec du contenu visuel"
      content: "GroupDocs.Assembly vous permet d'insérer des tableaux, des graphiques et des listes aux côtés de texte, d'hyperliens, d'images et même de codes-barres dynamiques."

    # feature loop
    - title: "Placez les données exactement où elles doivent être"
      content: "Les modèles LINQ aident à positionner vos données avec précision, à gérer des éléments répétitifs comme des tableaux et à appliquer des styles personnalisés sans effort."

    # feature loop
    - title: "Compatible avec divers formats de fichiers"
      content: "Fusionnez des documents de différents formats, y compris des PDF, HTML, des fichiers MS Office et OpenOffice, garantissant flexibilité pour vos projets."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment insérer programmatique un image dans un document"
      content: |
        Cet exemple montre comment intégrer une image dans un fichier DOCX en utilisant GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Ajoutez une balise d'espace réservé dans le fichier modèle
          // <<image [expression]>>

          // Définissez le chemin vers le modèle
          String template = "template.docx";

          // Spécifiez le chemin vers l'image
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Initialisez l'instance DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Enregistrez le fichier avec l'image intégrée
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "Capacités clés en un coup d'œil"
    exclude: "document"
    description: "Découvrez les fonctionnalités étendues que GroupDocs.Assembly offre pour rendre l'intégration et la fusion de documents efficaces et sans tracas."
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
    title: "Fusionnez différents types de documents"
    exclude: "DOCX"
    description: "Avec Java, vous pouvez intégrer et combiner du contenu dans plus de 50 formats de fichiers. Ajoutez des fichiers sans effort pour créer des résultats professionnels."
    items: 
          
        # format loop 1
        - name: "Intégrer un document dans un PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Intégrer un document dans un DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Document Microsoft Word Open XML"
          
        # format loop 3
        - name: "Intégrer un document dans un PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Présentation PowerPoint Open XML"
          
        # format loop 4
        - name: "Intégrer un document dans un XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Tableur Microsoft Excel Open XML"


          

---