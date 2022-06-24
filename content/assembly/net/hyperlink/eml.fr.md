---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/assembly/net/text/eml/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EMLX MSG 

############################# Head ############################
head_title: "API .NET pour insérer dynamiquement des hyperliens dans EML Documents"
head_description: "L'API GroupDocs.Assembly .NET permet aux développeurs d'insérer dynamiquement des hyperliens vers des e-mails, des rapports ou des documents tels que PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG, etc."

############################# Header ############################
title: "Insérer dynamiquement des hyperliens vers EML Documents et rapports via l'API .NET"
description: "L'API GroupDocs.Assembly .NET permet aux programmeurs d'insérer dynamiquement des hyperliens vers des rapports, des e-mails et des documents Office tels que PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, EML, HTML, MSG, etc."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment insérer dynamiquement des hyperliens dans des rapports, des e-mails et divers documents ?"
    content: |
       Cette page Web explique comment les utilisateurs peuvent insérer dynamiquement des hyperliens vers leur rapport, leur message électronique et divers types de documents dans leurs propres applications .NET. Les hyperliens sont l'épine dorsale du World Wide Web et peuvent être utilisés pour lier différentes pages, documents ou cliquer sur pour accéder à une nouvelle section dans le document actuel. GroupDocs.Assembly .NET est une API très puissante qui aide les développeurs de logiciels à ajouter dynamiquement des hyperliens dans leurs documents ou rapports avec seulement quelques lignes de code. Il a inclus la prise en charge de certains types de documents très populaires tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint et bien d'autres. Il a pris en charge plusieurs fonctionnalités avancées telles que l'insertion de liens vers la page du document, l'insertion de liens vers des cellules, la modification d'hyperliens, l'affichage de texte à la place de l'hyperlien, l'insertion dynamique de liens à partir de signets, l'insertion d'un hyperlien vers une diapositive de présentation et bien d'autres.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Insertion d'hyperliens dans des documents de traitement de texte via .NET"
      content_left: |
       L'API GroupDocs.Assembly .NET fournit une prise en charge complète pour l'insertion et la modification d'hyperliens dans divers types de documents. L'exemple de code C# .NET suivant montre comment ajouter facilement des liens hypertexte dans un document Word.

      title_right: "Comment ajouter des hyperliens dans un fichier Word"
      content_right: |
        * Paramétrage des documents source et destination
        * Définir l'expression Uri ainsi que l'expression de texte d'affichage
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "f4a8031406d44941d400088b718f7730"
      gistfile: "insert_hyperlinks_to_word_document.cs"

    - title_left: "Insérer dynamiquement des hyperliens dans des feuilles de calcul via .NET"
      content_left: |
       L'API GroupDocs.Assembly .NET prend entièrement en charge l'ajout et le traitement des hyperliens dans les fichiers de feuille de calcul. Vous pouvez facilement modifier son emplacement ou le remplacer par un nouveau. Le code C# suivant montre avec quelle facilité les utilisateurs peuvent insérer des liens hypertexte dans leurs fichiers de feuille de calcul dans leurs propres applications .NET. 

      title_right: "Ajouter des hyperliens aux documents de feuille de calcul"
      content_right: |
        * Configuration des fichiers de feuille de calcul source et cible
        * Définir l'expression Uri ainsi que l'expression de texte d'affichage
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "c2f9cd8bb06f9a7a2c444621ebf82696"
      gistfile: "insert_hyperlinks_in_spreadsheet_documents.cs"

    - title_left: "Ajouter des hyperliens à la présentation PowerPoint via l'API .NET"
      content_left: |
       GroupDocs.Assembly pour .NET aide les professionnels du logiciel à créer des applications pour gérer divers types de documents. L'exemple de code suivant montre comment les développeurs de logiciels peuvent ajouter des liens hypertexte dans leurs documents de présentation PowerPoint.

      title_right: "Comment ajouter des hyperliens dans les présentations"
      content_right: |
        * Configuration des fichiers de présentation source et destination
        * Définir Uri et afficher les expressions textuelles
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "49e1ca9eccc41942372c23c14f98ecef"
      gistfile: "insert_hyperlinks_in_presentation_documents.cs"

    - title_left: "API .NET pour insérer des hyperliens dans les e-mails"
      content_left: |
       L'API GroupDocs.Assembly .NET permet aux professionnels du logiciel d'insérer des hyperliens dans leurs documents de courrier électronique. Le code .NET suivant montre avec quelle facilité les programmeurs peuvent ajouter des liens hypertexte à leurs messages électroniques et les envoyer à d'autres utilisateurs à partir de leurs propres applications .NET.

      title_right: "Ajouter des hyperliens aux documents par courrier électronique"
      content_right: |
        * Configuration des fichiers de feuille de calcul source et cible
        * Définir Uri et afficher les expressions textuelles
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "8c119b4faa0334179854e164d87d3e7b"
      gistfile: "insert_hyperlinks_in_email_documents.cs"  

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