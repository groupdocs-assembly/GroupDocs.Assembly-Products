---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/assembly/net/document/pdf/"
otherformats: HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Insérer le contenu du document externe dans les e-mails et le fichier PDF via l'API .NET"
head_description: "L'API GroupDocs.Assembly .NET permet aux programmeurs d'insérer dynamiquement le contenu du document externe dans les formats de fichiers PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG et autres."

############################# Header ############################
title: "Insérer le contenu du document externe dans les fichiers Office et les messages électroniques via l'API .NET"
description: "L'API GroupDocs.Assembly .NET prend entièrement en charge l'insertion dynamique du contenu du document externe dans les rapports, les e-mails et les documents Office tels que PDF DOCX, XLSX, CSV, PPTX, MSG, etc."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment insérer le contenu d'un document externe dans d'autres fichiers, rapports et e-mails via .NET ?"
    content: |
      Un document ou un fichier de document fait référence à un ensemble d'informations numériques et non numériques qui peuvent être récupérées ultérieurement par l'utilisateur. Un ordinateur ou un document numérique est un fichier créé par une application logicielle qui peut être stocké dans un système informatique. Habituellement, un traitement de texte ou un éditeur de texte est utilisé pour créer un document électronique sur un système informatique. GroupDocs.Assembly pour .NET est une API très utile qui aide les développeurs de logiciels à créer un logiciel d'application puissant qui peut être utilisé pour créer et gérer facilement leurs documents. Il permet aux développeurs de logiciels d'insérer dynamiquement le contenu d'un document externe dans des rapports, des e-mails et des documents Office. Il a fourni des supports pour certains types de documents très couramment utilisés tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint et bien d'autres. De plus, certaines fonctionnalités avancées liées à l'insertion et à l'édition de contenu de documents sont entièrement prises en charge, telles que l'insertion de contenu dans une page de document, l'insertion dans des cellules de feuille de calcul, la modification ou le remplacement de contenu, l'insertion de contenu dans une diapositive de présentation, etc. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Insérer le contenu du document externe dans un fichier Word via .NET"
      content_left: |
       L'API GroupDocs.Assembly .NET permet aux développeurs de logiciels d'insérer facilement le contenu d'un document externe dans différents types de documents et de messages électroniques. L'exemple de code .NET ci-dessous montre comment insérer le contenu d'un document externe dans un document de traitement de texte avec seulement quelques lignes de code.

      title_right: "Comment ajouter le contenu du document au fichier PDF"
      content_right: |
        * Définir le modèle de document ouvert source
        * Définir le rapport de document ouvert de destination
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) pour générer un rapport au format de document ouvert. Elle supporte
          * Charge un modèle de document à partir du chemin source spécifié
          * Remplit le modèle de document avec des données provenant des sources uniques ou multiples spécifiées
          * Stocke le document de résultat dans le chemin cible en utilisant les LoadSaveOptions donnés.
          * Informations sur les objets de source de données.

      gisthash: "c4dc0be4f8ab8c2ba4ee6a78673ca1cd"
      gistfile: "dynamic_documents_insertion_to_word_processing.cs"

    - title_left: "Insérer le contenu du document externe dans les e-mails via .NET"
      content_left: |
       L'API GroupDocs.Assembly .NET permet l'ajout et la gestion de divers types de types de documents et de contenus à l'intérieur des documents. Il permet d'insérer dynamiquement le contenu d'un document externe dans différents types de documents et formats de fichiers de courrier électronique. Le code C # suivant montre avec quelle facilité les utilisateurs peuvent insérer le contenu d'un document externe dans leurs documents et messages électroniques dans leurs propres applications .NET. 

      title_right: "Ajouter le contenu du document à un message électronique via C#"
      content_right: |
        * Définir le modèle de document ouvert source
        * Définir le rapport de document ouvert de destination
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Appelez la méthode [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) pour générer un rapport au format de document ouvert. Elle supporte
          * Charge un modèle de document à partir du chemin source spécifié
          * Remplit le modèle de document avec des données provenant des sources uniques ou multiples spécifiées
          * Stocke le document de résultat dans le chemin cible en utilisant les LoadSaveOptions donnés.
          * Informations sur les objets de source de données.

      gisthash: "8fe014550c5f05467da6910a7ee16f18"
      gistfile: "dynamic_documents_insertion_to_emails_dotnet.cs"

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