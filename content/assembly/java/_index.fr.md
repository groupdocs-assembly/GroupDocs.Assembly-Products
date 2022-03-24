---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API d'assemblage d'automatisation de documents Java et de générateur de rapports dynamiques"
head_description: "API Java pour l'automatisation des documents, l'assemblage et la création de rapports. Créer des rapports à partir de modèles personnalisés. Assembler PDF Word Excel PPTX HTML à partir de sources de données DB, JSON, OData et XML."

############################# Header ############################
title: "API Java pour automatiser les documents et les rapports"
description: "Créer des applications d'automatisation de documents pour récupérer des données ; mettez-le dans des modèles personnalisables et générez des rapports dynamiques via l'API Java."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "/border/groupdocs-assembly-java.svg"
        product: "GroupDocs.Assembly"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Aperçu"

            # button loop
            - link: "#features"
              text: "Caractéristiques"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/assembly"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      L'API GroupDocs.Assembly pour Java vous aide à développer rapidement des applications d'automatisation de documents et de création de rapports en Java pour générer des rapports personnalisés à partir de modèles sans installer de logiciel externe. Le moteur de génération de rapports récupère les données du document modèle, les assemble et génère des rapports dans le format de sortie spécifié selon la syntaxe définie. Il vous permet de configurer et d'insérer dynamiquement les propriétés de mise en forme des éléments de modèle et prend en charge diverses sources de données (JSON, XML, OData, bases de données, CSV, tableur en tant que table de données, table de traitement de texte en tant que table de données et bases de données) pour récupérer des données.

      La bibliothèque d'assemblage de documents reconnaît plusieurs formats de documents et vous permet de créer des modèles dans tous les types de fichiers pris en charge tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint et texte. Il prend en charge la syntaxe de modèle basée sur LINQ et les utilisateurs peuvent également configurer et insérer dynamiquement les propriétés de mise en forme des éléments de modèle.

      GroupDocs.Assembly pour Java est facile à intégrer aux applications Java nouvelles ou existantes. Il est hautement compatible avec toutes les versions de Java et prend en charge les systèmes d'exploitation populaires (Windows, Linux, Mac OS) capables d'exécuter l'environnement d'exécution Java.

    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Assembly pour Java :

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Aperçu"
          content: |
            * Formulation des données
            * Formatage des données
            * Automatisation des données
            * Créer un modèle
            * Formatage des éléments du modèle
            * Génération de rapports
      
      ## TAB TWO ##
      tab_two:
        description: |
          Les [formats de fichiers de documents](https://docs.groupdocs.com/assembly/java/supported-document-formats/) pris en charge pour l'API de génération de documents Java sont répertoriés ci-dessous.

        left:
          enable: true
          table:
            # table loop
            - title: "Formats Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            # table loop
            - title: "Sources de données prises en charge"
              content: |
                * Base de données
                * XML
                * OData
                * JSON
                * CSV
                * Objets .NET personnalisés
                * Feuille de calcul sous forme de tableau de données
                * Table de traitement de texte comme table de données

        right:
          enable: true
          table:
            # table loop
            - title: "Autres formats"
              content: |
                * **OpenOffice Document Formats**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **Markdown Documentation File**: MD
                * **Other**: TXT

            # table loop
            - title: "Prise en charge de l'assemblage inter-formats"
              content: |
                * Traitement de texte **TO** Traitement de texte, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Tableur **TO** Tableur, HTML, PDF, XPS, TIFF, MHTML
                * Présentation **TO** Présentation, HTML, PDF, XPS, TIFF
                * Courriel **À** Traitement de texte, Courriel, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Traitement de texte HTML et TXT **TO**, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Assembly for Java prend en charge la suite Systèmes d'exploitation, Frameworks & Directeur chargé d'emballages:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Microsoft Windows
                * Serveur Microsoft Windows
                * Linux
                * Mac OS

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * Java 7 (1.7) et supérieur

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Environnements de développement"
              content: |
                * NetBeans
                * IDÉE IntelliJ
                * Éclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Outil d'automatisation de construction"
              content: |
                * Maven

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Assembly pour les fonctionnalités Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Ajustez l'image dans la zone de texte de Word, Excel, présentations et e-mails tout en préservant le rapport d'image"

      # feature loop
      - icon: "fas fa-eye"
        content: "Utiliser des formules et effectuer des opérations de données séquentielles - Appliquer la formule lors de l'assemblage de la feuille de calcul"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Appliquer le formatage supérieur, inférieur, majuscule, FirstCap aux chaînes dans la syntaxe du modèle"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Prise en charge de la syntaxe du modèle Formatage de la nature numérique ordinale, cardinale et alphabétique"

      # feature loop
      - icon: "fas fa-code"
        content: "Prend en charge les modèles de documents avec des variables personnalisées et des commentaires de texte dans les balises de syntaxe de modèle"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Insérer dynamiquement le contenu du document dans le rapport"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Configurer dynamiquement la couleur d'arrière-plan des documents HTML et générer un code-barres dans les rapports"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Insérer dynamiquement des hyperliens dans les rapports et appliquer des attributs au corps du message électronique"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Joindre dynamiquement des pièces jointes aux e-mails et mettre à jour les champs lors de l'assemblage du document de traitement de texte"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Prise en charge de NEXT Field Analogue de Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Ajouter dynamiquement des liens et des signets aux formats de document et nommer les plages de cellules des feuilles de calcul Excel"

      # feature loop
      - icon: "fas fa-columns"
        content: "Chargement et enregistrement des formats de documents de présentation POT et OTP assemblés"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Formatage de modèle pour les éléments numériques, texte, image, date-heure et graphiques"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Insérer dynamiquement des images et des documents à partir d'octets encodés en Base64"

      # feature loop
      - icon: "fas fa-print"
        content: "Syntaxe de modèle basée sur LINQ"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Modifier le format du fichier assemblé à l'aide de spécifications explicites ou d'une extension de fichier"

      # feature loop
      - icon: "fas fa-lock"
        content: "Liste ordonnée prise en charge pour Markdown - Enregistrer les e-mails et les documents Word nouvellement assemblés dans Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Générez divers types de rapports, par exemple, des graphiques, des images, des tableaux, des listes, etc."
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Erreurs de syntaxe de modèle en ligne dans les documents générés au lieu de lancer des exceptions"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Redémarrer dynamiquement une liste numérotée dans des documents Word ainsi que des e-mails avec des corps HTML et RTF"

      # feature loop
      - icon: "fas fa-heading"
        content: "Prise en charge des tableaux, des liens automatiques, des liens en ligne et des images pour les documents Markdown assemblés"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Génération dynamique de codes-barres (GS1-128 AI 8102 Coupon Extended et UPCA & GS1 Databar Coupon"

      # feature loop
      - icon: "fas fa-cube"
        content: "Chargez des documents modèles à partir de HTML avec des ressources et enregistrez Word, Excel, PowerPoint et des e-mails assemblés au format HTML avec des ressources"

    more_feature :
      # more_feature_loop
      - title: "Manipuler les éléments du modèle"
        content: |
          Manipulez de nombreux éléments de modèle avec GroupDocs.Assembly pour l'API Java. Les éléments de modèle avec lesquels vous pouvez travailler incluent les blocs de texte, les images, les hyperliens, les blocs HTML, les codes-barres (via les polices de code-barres) et les graphiques. Vous pouvez également appliquer des blocs répétés et des blocs conditionnels pour les éléments de liste et les lignes de tableau. Fusion dynamique de cellules de tableau contenant le même texte, basée sur des expressions de modèle pour les documents, les présentations, les feuilles de calcul et les e-mails avec des corps HTML et RTF.
      
      # more_feature_loop
      - title: "Manipuler les rapports de liste"
        content: |
          L'utilisation de l'API GroupDocs.Assembly pour Java prend en charge les types de rapports de liste suivants :

          * Liste à puces
          * Liste numérotée
          * Colored Liste numérotée

      # more_feature_loop
      - title: "Manipuler les rapports graphiques"
        content: |
          GroupDocs.Assembly pour Java prend en charge les types de rapports graphiques suivants :

          * Graphique à bulles, qui affiche trois dimensions de données
          * Graphique à colonnes
          * Diagramme circulaire
          * Diagramme de dispersion
          * Tableau des séries (en couleur)

      # more_feature_loop
      - title: "Manipuler les rapports de table"
        content: |
          GroupDocs.Assembly pour Java prend en charge les types de rapports de table suivants :

          * Tableau maître-détail
          * Tableau avec lignes en surbrillance
          * Tableau avec contenu alternatif
          * Tableau avec filtrage, regroupement et classement

          Vous pouvez également utiliser des bandes de données dans les lignes du tableau.

      # more_feature_loop
      - title: "Manipuler les rapports graphiques"
        content: |
          L'intégration de GroupDocs.Assembly pour l'API Java avec votre application Java est un jeu d'enfant. Ce qui suit est un exemple de bloc de code qui génère un rapport au format OpenDocument à l'aide de Java : 

          ```java
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Assembly propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "/border/groupdocs-assembly-net.svg"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---