---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/assembly/java/barcode/eml/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OXPS MD EMLX MSG 

############################# Head ############################
head_title: "API Java pour générer des documents d'images de codes à barres et des messages électroniques"
head_description: "L'API Java GroupDocs.Assembly permet aux programmeurs de créer et d'ajouter des codes-barres dans les documents (PDF, DOC, DOCX, RTF, XLSX, CSV, PPTX) et les messages électroniques (EML EMLX MSG)."

############################# Header ############################
title: "API Java Barcodes Generator - Créer des codes-barres 1D et 2D dans EML Documents"
description: "L'API Java GroupDocs.Assembly permet de générer et d'ajouter des images de codes-barres 1D et 2D dans des messages PDF HTML, XPS, PS, TXT, EPUB, PCL, SVG, Documents et e-mails (EML, EMLX, MSG)."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment générer et insérer des codes-barres dans des documents et des e-mails ?"
    content: |
       Les codes-barres deviennent populaires et sont utilisés partout de nos jours. Il a commencé à apparaître dans les épiceries au milieu des années 1970 et se trouve aujourd'hui dans les livres, les billets, les hôpitaux pour le suivi des médicaments, les magasins de pièces automobiles et bien d'autres. Cette page Web explique comment créer et ajouter dynamiquement des images de codes à barres dans des documents et des e-mails dans des applications Java. GroupDocs.Assembly pour Java est une API très utile qui aide les développeurs de logiciels à créer de puissantes applications d'automatisation de documents et de création de rapports. Il prend en charge la gestion de nombreux formats de documents populaires tels que PDF, HTML, XPS, Microsoft Office Word, les feuilles de calcul Excel, les présentations PowerPoint, les e-mails Outlook et bien d'autres. L'API Java facilite la création et l'insertion d'images de codes-barres dans des documents ainsi que dans des messages électroniques avec seulement quelques lignes de code. Il prend également en charge la modification des propriétés de l'image du code-barres, telles que la mise à l'échelle de l'image du code-barres, la modification des couleurs avant et arrière, la modification de la résolution de l'image du code-barres, le placement du texte du code-barres, la modification des polices, etc. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Créez des codes-barres dans EML Documents via Java"
      content_left: |
       GroupDocs.Assembly Java a inclus une fonctionnalité complète pour insérer et modifier des codes-barres dans les documents EML. L'exemple de code Java suivant montre comment créer et utiliser des images de code-barres dans un document EML avec seulement quelques lignes de code. 

      title_right: "Comment ajouter des codes-barres dans les fichiers EML ?"
      content_right: |
       * Créez une instance de [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
       * Créer un exemple d'objet de source de données
       * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.DataSourceInfo...-) méthode avec les paramètres suivants
           * Diffusez pour lire un modèle de document à partir de.
           * Stream pour écrire le document résultant.
           * Options de chargement et d'enregistrement de documents.
           * Détails Informations sur les objets de source de données à utiliser.

      gisthash: "ebb6d8215f329f457f843e9a9fc48c9c"
      gistfile: "generate_barcodes_in_presentations.java"     

    - title_left: "Configuration requise"
      content_left: |
       Les API Java GroupDocs.Assembly sont prises en charge sur toutes les principales plateformes et systèmes d'exploitation. Il peut générer des documents dans Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice et plus de 50 autres formats. Pour un guide complet de la configuration système requise, veuillez visiter [système requis](https://docs.groupdocs.com/assembly/java/system-requirements/) Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système:
         * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
         * Prise en charge des versions Java : J2SE 7.0 (1.7), J2SE 8.0 (1.8) ou supérieur
         * Obtenez la dernière version des API Java GroupDocs.Assembly de [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/)
        
      title_right: "Pourquoi utiliser GroupDocs.Assembly"
      content_right: |
        * Créez des documents personnalisés à partir de modèles.
        * Joindre dynamiquement des pièces jointes aux e-mails.
        * Aucun logiciel supplémentaire n'est requis pour créer et automatiser des documents.
        * Génère un document de sortie basé sur la source de données.
        * Insérer dynamiquement le contenu du document dans le rapport
        * Appliquer la formule lors de l'assemblage de la feuille de calcul.
        * Fournit un support pour plusieurs formats de données
        * Prise en charge des opérations de données séquentielles.
demos:
    enable: true

more_formats:
    enable: true


back_to_top:
    enable: true
---