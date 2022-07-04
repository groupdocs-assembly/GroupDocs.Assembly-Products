---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/assembly/java/hyperlink/otp/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Ajouter des hyperliens aux documents et rapports Office OTP via l'API Java"
head_description: "GroupDocs.Assembl pour Java prend en charge l'insertion dynamique d'hyperliens vers des documents de bureau et de courrier électronique tels que PDF DOCX, RTF, XLSX, PPTX, EML, MSG et plus encore dans les applications Java."

############################# Header ############################
title: "Ajouter des hyperliens aux documents Office et aux e-mails via l'API Java"
description: "L'API Java GroupDocs.Assembly permet aux professionnels du logiciel d'ajouter par programmation des hyperliens aux messages électroniques et aux documents Office tels que PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, MSG, etc."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment utiliser l'API Java pour ajouter des hyperliens aux documents Office et e-mails ?"
    content: |
       Un lien hypertexte est un mot, une phrase ou une image sur laquelle vous pouvez cliquer pour accéder à un nouveau document ou à une nouvelle section du document actuel. Les hyperliens sont l'épine dorsale du Web mondial et sont utilisés pour de nombreuses fonctions nécessaires sur le World Wide Web. GroupDocs.Assembly pour Java est une API d'automatisation de documents et de génération de rapports qui aide les développeurs de logiciels à insérer dynamiquement des hyperliens dans leurs documents ou rapports. L'API est très stable et prend entièrement en charge plusieurs fonctionnalités avancées liées à la gestion des hyperliens, telles que l'ajout d'hyperliens à une page de document, l'ajout de liens à une diapositive de présentation, l'ajout d'hyperliens aux cellules de la feuille de calcul, la modification du contenu des hyperliens, l'insertion dynamique de liens à partir de signets, la suppression des indésirables. liens, afficher du texte au lieu d'un lien hypertexte, et bien d'autres. Certains types de documents très courants tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, etc. sont entièrement pris en charge.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Insérer des hyperliens vers des documents de traitement de texte via Java"
      content_left: |
       L'API Java GroupDocs.Assembly prend entièrement en charge l'insertion et la modification d'hyperliens dans divers formats de documents couramment utilisés. L'exemple de code Java ci-dessous montre comment insérer des liens hypertexte dans un document Microsoft Word.

      title_right: "Insérer des liens hypertexte dans le document OTP via Java"
      content_right: |
        * Paramétrage des documents source et destination
        * Définir l'expression Uri ainsi que l'expression de texte d'affichage
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) méthode pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "Ajouter des hyperliens dans les feuilles de calcul via Java"
      content_left: |
       L'API Java GroupDocs.Assembly permet aux programmeurs informatiques d'insérer et de modifier facilement des hyperliens dans leurs feuilles de calcul. Ils peuvent facilement y accéder, modifier son emplacement ou le remplacer par un nouveau. Le code Java suivant montre avec quelle facilité les programmeurs peuvent ajouter des hyperliens dans leurs feuilles de calcul.

      title_right: "Comment insérer des liens hypertexte dans le fichier OTP"
      content_right: |
        * Configuration des fichiers de feuille de calcul source et cible
        * Définir l'expression Uri ainsi que l'expression de texte d'affichage
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) méthode pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "Insérer des liens hypertexte vers une présentation PowerPoint via Java"
      content_left: |
       L'API Java GroupDocs.Assembly permet aux programmeurs de gérer facilement leurs tâches liées à la gestion des documents. Voici un exemple de code Java qui montre avec quelle facilité les programmeurs de logiciels peuvent accéder à leurs documents de présentation PowerPoint et y ajouter des hyperliens.

      title_right: "Comment insérer des hyperliens dans les présentations"
      content_right: |
        * Configuration des fichiers de présentation source et destination
        * Définir Uri et afficher les expressions textuelles
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) méthode pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "Utiliser l'API Java pour ajouter des hyperliens dans les e-mails"
      content_left: |
       GroupDocs.Assembly pour Java permet aux développeurs de logiciels d'ajouter facilement des hyperliens à leurs messages électroniques avec seulement quelques lignes de code Java. L'exemple suivant montre avec quelle facilité les développeurs peuvent insérer des liens hypertexte dans leurs documents de courrier électronique et les envoyer à d'autres utilisateurs dans leurs propres applications Java.

      title_right: "Comment ajouter des hyperliens aux e-mails"
      content_right: |
        * Configuration des fichiers de feuille de calcul source et cible
        * Définir Uri et afficher les expressions textuelles
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) méthode pour assembler le document. Elle supporte
          * Stream pour lire un modèle de document.
          * Stream pour écrire le document résultant.
          * Options supplémentaires pour le chargement et l'enregistrement de documents.
          * Informations sur les objets de source de données.

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

    - title_left: "Configuration requise"
      content_left: |
        Les API Java GroupDocs.Assembly sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Il peut générer des documents dans Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice et plus de 50 autres formats. Pour un guide complet de la configuration système requise, veuillez visiter [système requis](https://docs.groupdocs.com/assembly/java/system-requirements/) Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système:
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