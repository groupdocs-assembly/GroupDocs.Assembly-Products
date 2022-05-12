---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/assembly/net/barcode/emlx/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OXPS MD EML MSG 

############################# Head ############################
head_title: "Créer et ajouter des images de codes-barres dans des documents et des e-mails via .NET"
head_description: "L'API GroupDocs.Assembly .NET permet aux développeurs de générer et d'insérer dynamiquement des images de codes à barres dans des documents (PDF DOC, DOCX, RTF, XLSX, CSV, PPTX) et des messages électroniques en toute simplicité."

############################# Header ############################
title: "Générer et insérer des images de codes-barres dans les documents EMLX via l'API .NET"
description: "GroupDocs.Assembly .NET fournit une prise en charge complète de la création, de l'édition et de l'ajout dynamiques d'images de codes-barres dans les documents EMLX à l'aide de l'API C# et VB.NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment effectuer la génération d'images de codes-barres dans des documents ?"
    content: |
       Cette page aidera les utilisateurs à comprendre et à apprendre comment générer et insérer dynamiquement des images de codes-barres dans leurs documents et messages électroniques dans C #, ASP.NET et d'autres applications liées à .NET. GroupDocs.Assembly .NET est une API très puissante qui donne aux utilisateurs la possibilité d'automatiser et de générer des rapports dans de nombreux formats de fichiers à l'intérieur de leurs propres applications .NET sans aucune dépendance externe. Il prend en charge certains formats de fichiers très courants tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint et diapositives. Il prend entièrement en charge certaines symbologies de codes à barres linéaires et 2D courantes. Vous pouvez également personnaliser facilement la taille de l'image du code-barres, les couleurs d'avant et d'arrière-plan, la police et l'emplacement du texte du code-barres, définir la résolution de l'image du code-barres, etc. Il prend également en charge la création de documents personnalisés à partir de modèles et de données obtenues à partir de diverses sources telles que des bases de données, XML, JSON, OData, des objets, etc. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Génération de codes-barres dans les documents EMLX via .NET"
      content_left: |
       GroupDocs.Assembly .NET fournit une prise en charge complète pour l'ajout et la gestion des codes-barres dans les documents EMLX. L'exemple de code C# .NET suivant montre comment générer et insérer des images de code-barres dans un document EMLX. 

      title_right: "Comment utiliser les images de codes-barres dans EMLX"
      content_right: |
       * Créez une instance de [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
       * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) avec les paramètres suivants
           * Stream pour lire un modèle de document.
           * Stream pour écrire le document résultant.
           * Options supplémentaires pour le chargement et l'enregistrement de documents.
           * Informations sur les objets de source de données.

      gisthash: "8576f622912b355ce69966077033dcac"
      gistfile: "generate_barcodes_in_spreadsheets.cs"

    - title_left: "Définir la résolution de l'image du code-barres dans EMLX via .NET"
      content_left: |
       GroupDocs.Assembly .NET fournit une prise en charge complète pour l'ajout et la gestion des codes-barres dans les documents EMLX. Vous pouvez facilement définir la résolution du code-barres avec seulement quelques lignes de code. Le code suivant permet aux utilisateurs de définir la résolution horizontale et verticale sur 300 DPI. 

      title_right: "Résolution améliorée des codes-barres dans EMLX"
      content_right: |
       * Créez une instance de [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
       * Appelez la méthode BarcodeSettings.Resolution pour définir la résolution de l'image du code-barres sur 300 DPI.

      gisthash: "9d8d743bd67b4bce5a4a7f1250deef26"
      gistfile: "set_barcode_image_resolution.cs"
      

    - title_left: "Configuration requise"
      content_left: |
       Les API GroupDocs.Assembly .NET sont prises en charge sur toutes les principales plateformes et systèmes d'exploitation. Pour un guide complet de la configuration système requise, veuillez visiter [configuration système](https://docs.groupdocs.com/assembly/net/system-requirements/) Avant d'exécuter le code ci-dessous, assurez-vous que les conditions préalables suivantes sont installées sur votre système:
        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnement de développement : Visual Studio, Xamarin, MonoDevelop etc.
        * Frameworks : .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenez la dernière version des API GroupDocs.Assembly .NET à partir de [NuGet](https://www.nuget.org/packages/GroupDocs.Assembly/)
        
      title_right: "Pourquoi utiliser GroupDocs.Assembly"
      content_right: |
        * Autoriser les utilisateurs à créer des documents personnalisés à partir de modèles.
        * Aucun logiciel supplémentaire n'est requis pour créer et automatiser des documents
        * Possibilité de générer un document de sortie basé sur la source de données
        * Insérer dynamiquement le contenu du document dans le rapport
        * Joindre dynamiquement des pièces jointes aux e-mails et insérer des hyperliens dans les rapports
        * Suppression automatique des paragraphes vides
        * Prise en charge complète de plusieurs formats de données
        * Prise en charge des pièces jointes dynamiques

demos:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---