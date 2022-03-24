---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API pour l'automatisation des documents, l'assemblage et la génération de rapports"
head_description: "C# .NET API d'automatisation de documents, d'assemblage et de génération de rapports. Créez des documents PDF Word Excel PPTX HTML et e-mail à partir de modèles personnalisés."

############################# Header ############################
title: ".NET Document Automation & Reporting API"
description: "Générer des rapports dans des applications .NET en définissant des modèles et en fusionnant les données."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "/border/groupdocs-assembly-net.svg"
        product: "GroupDocs.Assembly"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly pour l'API .NET vous aide à créer de puissantes applications d'automatisation de documents et de génération de rapports avec des capacités pour générer des rapports à partir de modèles personnalisés en C#, ASP.NET et d'autres applications liées à .NET. Avec seulement quelques lignes de code, la bibliothèque de rapports .NET assemble intelligemment les données fournies à partir du modèle de document défini et génère de beaux rapports dans le format de sortie préféré en récupérant les données de diverses sources de données (bases de données, XML, JSON, ODATA, CSV, Objets .NET personnalisés).

      Il prend en charge la syntaxe de modèle basée sur LINQ et les utilisateurs peuvent facilement générer des documents de sortie dans tous les formats de fichiers professionnels couramment utilisés tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint et diapositives. Les propriétés de formatage des éléments de modèle sont également configurables en manipulant du texte, des blocs HTML et conditionnels, des images, des graphiques, des codes-barres, des hyperliens, des tableaux croisés dynamiques, etc.

      GroupDocs.Assembly pour .NET peut être utilisé pour développer des applications dans n'importe quel environnement de développement qui cible la plate-forme .NET. Il est compatible avec tous les langages basés sur .NET et prend en charge les systèmes d'exploitation populaires (Windows, Linux, Mac OS) sur lesquels les frameworks Mono ou .NET (y compris .NET Core) peuvent être installés.

    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Assembly pour .NET :
      
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
          Les [formats de fichiers de documents](https://docs.groupdocs.com/assembly/net/supported-document-formats/) pris en charge pour l'API de génération de documents .NET sont répertoriés ci-dessous.

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
          GroupDocs.Assembly for .NET prend en charge la suite Systèmes d'exploitation, Frameworks & Directeur chargé d'emballages:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Windows
                * Serveur Windows
                * windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * .NET Framework 2.0 ou supérieur
                * Mono Framework 1.2 ou supérieur

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Directeur chargé d'emballage"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Environnements de développement"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Assembly pour les fonctionnalités .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Fonctionne avec plusieurs formats de données"

      # feature loop
      - icon: "fas fa-eye"
        content: "Capable de manipuler des données à l'aide de formules et d'opérations de données séquentielles"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Formater les chaînes dans la syntaxe du modèle pour qu'elles soient supérieures, inférieures, majuscules, FirstCap"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Effectuer un formatage numérique ordinal, cardinal et alphabétique dans la syntaxe du modèle"

      # feature loop
      - icon: "fas fa-code"
        content: "Définir des variables dans les modèles de documents et prendre en charge les commentaires de texte dans les balises de syntaxe de modèle"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Insérer dynamiquement le contenu des documents externes dans vos rapports"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Générer dynamiquement une image de code-barres dans les rapports et définir la couleur d'arrière-plan pour les documents HTML"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Attribuer dynamiquement des attributs au corps du message électronique et insérer des hyperliens dans les rapports"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Créer dynamiquement des pièces jointes aux e-mails"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Prise en charge du champ NEXT analogique de Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Mettre à jour les champs lors de l'assemblage de documents de traitement de texte"

      # feature loop
      - icon: "fas fa-columns"
        content: "Calculer une formule lors de l'assemblage de feuilles de calcul"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Format Numérique, Texte, Image, Graphique, Date-Heure Éléments du modèle"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Chargement et enregistrement des formats de documents de présentation POT et OTP assemblés"

      # feature loop
      - icon: "fas fa-print"
        content: "Utiliser la syntaxe basée sur LINQ pour le modèle et effectuer le formatage de texte conditionnel des éléments de modèle"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Modifier le format de fichier du document assemblé à l'aide de l'extension de fichier ou des spécifications explicites"

      # feature loop
      - icon: "fas fa-lock"
        content: "Liste ordonnée prise en charge pour Markdown - Enregistrer les e-mails et les documents Word nouvellement assemblés dans Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Prend en charge les rapports de nombreux types, par exemple, les graphiques, les listes, les tableaux, les images, etc."
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Erreurs de syntaxe de modèle en ligne dans les documents générés au lieu de lancer des exceptions"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Chargez des documents modèles à partir de HTML avec des ressources et enregistrez Word, Excel, PowerPoint et des e-mails assemblés au format HTML avec des ressources"

      # feature loop
      - icon: "fas fa-heading"
        content: "Ajouter dynamiquement la numérotation des listes de redémarrage dans les formats de document Word et les e-mails avec des corps HTML et RTF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Insérer dynamiquement des images et des documents à partir d'octets encodés en Base64 and adjust checkbox value settings of Word documents"

      # feature loop
      - icon: "fas fa-cube"
        content: "Étirer l'image dans la zone de texte de Word, Excel, présentations et e-mails tout en préservant le rapport d'image"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Ajouter dynamiquement des liens et des signets aux formats de document et nommer les plages de cellules des feuilles de calcul Excel"

    more_feature :
      # more_feature_loop
      - title: "Prise en charge des éléments de modèle"
        content: |
          GroupDocs.Assembly pour l'API .NET vous permet de contrôler l'utilisation de nombreux éléments de modèle. Vous pouvez travailler avec des blocs de texte formatés, des blocs HTML, des images, des graphiques, des hyperliens et des codes à barres (via les polices de codes à barres). Les blocs répétés et les blocs conditionnels sont également pris en charge, y compris les éléments de liste et les lignes de tableau. Vous pouvez également fusionner dynamiquement des cellules de tableau contenant le même texte en fonction d'expressions de modèle pour des feuilles de calcul, des présentations, des documents et des e-mails avec des corps HTML et RTF.

      # more_feature_loop
      - title: "Utilisation des rapports de liste"
        content: |
          À l'aide de l'API GroupDocs.Assembly pour .NET, vous pouvez utiliser les rapports de liste des trois types suivants :

          * Liste à puces
          * Liste numérotée
          * Colored Liste numérotée

      # more_feature_loop
      - title: "Utilisation des rapports de graphique"
        content: |
          GroupDocs.Assembly pour .NET prend en charge les types de rapports graphiques suivants :

          * Graphique à bulles, qui affiche trois dimensions de données
          * Graphique à colonnes
          * Diagramme circulaire
          * Diagramme de dispersion
          * Tableau des séries (en couleur)

      # more_feature_loop
      - title: "Utilisation des rapports de tableau"
        content: |
          GroupDocs.Assembly pour .NET prend en charge les types de rapports de table suivants :

          * Tableau maître-détail
          * Tableau avec lignes en surbrillance
          * Tableau avec contenu alternatif
          * Tableau avec filtrage, regroupement et classement
          
          Vous pouvez également utiliser des bandes de données dans les lignes du tableau.

      # more_feature_loop
      - title: "Intégration facile"
        content: |
          Vous pouvez facilement intégrer l'API GroupDocs.Assembly pour .NET à votre application .NET en utilisant seulement quelques lignes de code. Voici un exemple de code pour générer un rapport dans un document ouvert format:

          ```cs
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
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
        - img_alt: "GroupDocs.Assembly for Java"
          image: "/border/groupdocs-assembly-java.svg"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
