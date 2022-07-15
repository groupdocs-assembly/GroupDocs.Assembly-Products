---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/assembly/java/document/pptx"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "API Java : ajouter le contenu d'un document externe aux formats de fichier PPTX"
head_description: "L'API Java GroupDocs.Assembly permet l'insertion dynamique du contenu d'un document externe dans divers formats de fichiers tels que PDF, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG, etc."

############################# Header ############################
title: "API Java pour insérer le contenu d'un document externe dans d'autres formats de fichiers pris en charge"
description: "GroupDocs.Assembly pour Java fournit des fonctionnalités permettant d'insérer le contenu d'un document externe dans des rapports, des e-mails et divers formats de fichiers pris en charge tels que PDF, DOC, DOCX, XLSX, CSV, PPTX, EML, MSG, etc."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment insérer le contenu d'un document externe dans d'autres formats de fichiers populaires via Java?"
    content: |
      Un document ou un fichier est une copie électronique ou une copie papier contenant des informations qui peuvent être récupérées ultérieurement par l'utilisateur. Selon Wikipedia, un document peut être structuré, comme des documents tabulaires, des listes, des formulaires ou un tableau scientifique, semi-structuré comme un livre ou un article de journal, ou non structuré comme une note manuscrite. GroupDocs.Assembly pour Java est une API très utile qui permet aux développeurs de logiciels de créer des applications puissantes pour l'automatisation des documents et la création de rapports. Il prend entièrement en charge l'identification et l'utilisation de nombreux formats de documents tels que PDF, Microsoft Word, feuilles de calcul Excel, PowerPoint, , HTML, e-mail Outlook et bien d'autres. Il prend en charge de nombreuses fonctionnalités avancées pour travailler avec des rapports tels que la manipulation d'éléments de modèle, des rapports de listes, des rapports de graphique, des rapports de tableau, etc. De plus, l'API prend également entièrement en charge plusieurs fonctionnalités avancées liées à l'ajout et à la modification de contenu de documents, telles que l'ajout de contenu à une page de document, l'insertion de données dans des cellules de feuille de calcul, le remplacement de contenu, l'ajout de contenu à une diapositive de présentation et bien d'autres.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Ajouter le contenu du fichier externe au document Word via Java"
      content_left: |
       L'API Java GroupDocs.Assembly aide les programmeurs informatiques à gérer les tâches de manipulation de documents dans leurs propres applications Java. Il prend entièrement en charge le contenu du fichier d'un document externe pour différents types de types de documents. L'exemple de code Java suivant montre comment ajouter le contenu d'un fichier externe à un document de traitement de texte avec seulement quelques lignes de code.

      title_right: "Comment insérer le contenu du document dans le fichier PPTX"
      content_right: |
        * Définition du modèle de document source
        * Définition du rapport de document de destination
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) méthode pour assembler le document. Elle supporte
          * Le flux à partir duquel lire un modèle de document.
          * Le flux pour écrire un document de résultat.
          * Spécifie des options supplémentaires pour le chargement et l'enregistrement de documents.
          * Fournit des informations sur les objets de source de données à utiliser.

      gisthash: "abb65f9e514add59870865121ed3c526"
      gistfile: "insert_documents_to_word_processing.java"

    - title_left: "Ajouter le contenu du fichier externe aux messages électroniques via Java"
      content_left: |
       L'API Java GroupDocs.Assembly a inclus une fonctionnalité d'insertion de contenu de document externe dynamique dans plusieurs formats de fichiers de documents et messages électroniques populaires. Le code Java ci-dessous montre comment les programmeurs peuvent ajouter le contenu d'un document externe à leurs documents de courrier électronique sans aucune application externe.

      title_right: "Comment ajouter le contenu du fichier au document PPTX"
      content_right: |
        * Définition du modèle de document source
        * Définition du rapport de document de destination
        * Créer une instance de la classe [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Appelez [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) méthode pour assembler le document. Elle supporte
          * Le flux à partir duquel lire un modèle de document.
          * Le flux pour écrire un document de résultat.
          * Spécifie des options supplémentaires pour le chargement et l'enregistrement de documents.
          * Fournit des informations sur les objets de source de données à utiliser.

      gisthash: "b72d7608548993ffbe62f97c798ba021"
      gistfile: "Insert_dynamic_documents_to_emails.java"

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