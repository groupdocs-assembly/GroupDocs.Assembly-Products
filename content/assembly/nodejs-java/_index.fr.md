---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: fr
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Boîte à outils Node.js pour la création, l'automatisation et la personnalisation de documents"
head_description: "Bibliothèque Node.js pour automatiser les workflows de documents. Générez des fichiers PDF, Word, Excel, PowerPoint, HTML et email à partir de vos modèles."

############################# Header ############################
title: "API Node.js pour l'automatisation simplifiée de documents et de rapports"
description: "Rationalisez la génération de rapports JavaScript en fusionnant vos données avec des modèles préconstruits."
words:
  for: "pour"

actions:
  main: "Commencez votre essai sur NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence."

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Créer un graphique dans un document Word en utilisant Node.js"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Chemin vers le modèle principal
    const template = "chart_template.docx";

    // Récupérer les données de productivité des managers à partir de la source
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Créer une instance de DataSourceInfo avec les données
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Définir les couleurs du graphique à l'aide d'un autre DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Remplir le modèle avec des données et l'enregistrer en sortie
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Aperçu de GroupDocs.Assembly"
  description: "Bibliothèque Node.js conçue pour créer des documents de manière programmatique avec gestion des données intégrée."
  features:
    # feature loop
    - title: "Intégrer les données commerciales dans des modèles avec JavaScript"
      content: "Générez des rapports soignés en intégrant des données JSON, XML ou autres dans des modèles avec GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Gérer le contenu intégré"
      content: "Remplissez automatiquement tables, graphiques et autres visuels dans vos documents en utilisant des données externes."

    # feature loop
    - title: "Options personnalisables"
      content: "GroupDocs.Assembly for Node.js via Java vous permet d'ajouter des fonctionnalités telles que des codes-barres, de récupérer des données à partir d'URLs et d'exporter des fichiers dans divers formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Assembly for Node.js via Java s'intègre parfaitement avec les systèmes d'exploitation, frameworks et gestionnaires de paquets les plus utilisés."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Assembly for Node.js via Java prend en charge un large éventail de [formats de documents](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formats Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Images & Autres Formats
        * **Portable:** PDF
        * **Images:** SVG, TIFF
        * **Autres formats de bureau:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Autres formats
        * **Web:** HTML, MHTML
        * **Emails:** EML, MSG, EMLX
        * **Autre:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Fonctionnalités principales de GroupDocs.Assembly"
  description: "Créez des documents et des rapports dynamiques avec des outils de gestion de données puissants."

  items:
    # feature loop
    - icon: "preview"
      title: "Visuels de données riches"
      content: "Insérez des graphiques, tableaux, images et listes dans vos documents avec une personnalisation complète."

    # feature loop
    - icon: "manipulate"
      title: "Transformez vos données"
      content: "Utilisez des outils comme des formules et le tri pour structurer et afficher les informations efficacement."

    # feature loop
    - icon: "two_pages"
      title: "Large compatibilité de formats"
      content: "Travaillez sans effort avec des formats de fichiers populaires pour les modèles et les sorties."

    # feature loop
    - icon: "document_settings"
      title: "Personnalisation avancée des modèles"
      content: "Formatez les modèles avec des options de style numériques, alphabétiques et autres."

    # feature loop
    - icon: "text"
      title: "Générez des codes-barres dynamiquement"
      content: "Créez et intégrez des images de codes-barres directement dans vos documents à la demande."

    # feature loop
    - icon: "add"
      title: "Style de texte flexible"
      content: "Appliquez facilement des styles de texte tels que la capitalisation ou la casse de titre dans vos modèles."

    # feature loop
    - icon: "manipulate"
      title: "Insertion dynamique de contenu"
      content: "Incluez dynamiquement du contenu à partir de fichiers externes lors de la génération de documents."

    # feature loop
    - icon: "convert"
      title: "Export vers divers formats"
      content: "Enregistrez des documents dans plusieurs formats avec vos configurations spécifiées."

    # feature loop
    - icon: "update"
      title: "Intégrez dynamiquement des médias"
      content: "Insérez des images ou d'autres éléments en utilisant des données Base64 lors de la création de documents."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Découvrez des exemples pratiques de l'utilisation de GroupDocs.Assembly pour des tâches courantes."
  items:
    # code sample loop
    - title: "Ajouter une liste à puces dans des documents Word"
      content: |
        Voir comment créer des [listes à puces](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) dans des documents Word pour organiser les données efficacement. Cet exemple démontre comment générer une liste à puces en utilisant GroupDocs.Assembly.
        {{< landing/code title="Ajouter une liste à puces dans des documents Word">}}
        ```javascript {style=abap}
        // Insérez ce modèle sur une page de document :
        // Indicateurs de performance des managers
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Spécifiez le chemin du modèle
        const template = "Bulleted List Template.docx";

        // Définissez le chemin du fichier de sortie
        const result = "Result Report.docx"

        // Récupérez les données des managers à partir d'une source JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Générez le rapport avec les données remplies
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Insérer des graphiques circulaires dans PowerPoint"
      content: |
        Apprenez à utiliser des modèles et XML pour ajouter des [graphiques circulaires](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) dans vos présentations. Améliorez vos rapports avec des graphiques circulaires pour présenter les données visuellement et clairement.
        {{< landing/code title="Insérer des graphiques circulaires dans PowerPoint">}}
        ```javascript {style=abap} 
        // Ajoutez le modèle de titre du graphique à la présentation :
        // Revenus des clients <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Incluez également le modèle de données du graphique :
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Spécifiez le chemin du modèle de graphique
        const template = "Pie Chart Template.pptx";

        // Définissez le chemin du fichier de sortie
        const result = "Result Report.pptx"

        // Récupérez les données des clients à partir d'une source XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Générez le graphique et enregistrez le résultat
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---