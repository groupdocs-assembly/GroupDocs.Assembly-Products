---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
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
head_title: "{index-content-nodejs-java.head_title}"
head_description: "{index-content-nodejs-java.head_description}"

############################# Header ############################
title: "{index-content-nodejs-java.title}"
description: "{index-content-nodejs-java.description}"
words:
  for: "pour"

actions:
  main: "{index-content-nodejs-java.actions_main}"
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
  title: "{index-content-nodejs-java.code_title}"
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
  description: "{index-content-nodejs-java.overview_description}"
  features:
    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_1.title}"
      content: "{index-content-nodejs-java.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_2.title}"
      content: "{index-content-nodejs-java.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_3.title}"
      content: "{index-content-nodejs-java.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "{index-content-nodejs-java.platforms_description}"
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
    {index-content-nodejs-java.formats_description}
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
  title: "{index-content-nodejs-java.features.title}"
  description: "{index-content-nodejs-java.features.description}"

  items:
    # feature loop
    - icon: "preview"
      title: "{index-content-nodejs-java.features.feature_1.title}"
      content: "{index-content-nodejs-java.features.feature_1.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_2.title}"
      content: "{index-content-nodejs-java.features.feature_2.content}"

    # feature loop
    - icon: "two_pages"
      title: "{index-content-nodejs-java.features.feature_3.title}"
      content: "{index-content-nodejs-java.features.feature_3.content}"

    # feature loop
    - icon: "document_settings"
      title: "{index-content-nodejs-java.features.feature_4.title}"
      content: "{index-content-nodejs-java.features.feature_4.content}"

    # feature loop
    - icon: "text"
      title: "{index-content-nodejs-java.features.feature_5.title}"
      content: "{index-content-nodejs-java.features.feature_5.content}"

    # feature loop
    - icon: "add"
      title: "{index-content-nodejs-java.features.feature_6.title}"
      content: "{index-content-nodejs-java.features.feature_6.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_7.title}"
      content: "{index-content-nodejs-java.features.feature_7.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-nodejs-java.features.feature_8.title}"
      content: "{index-content-nodejs-java.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-nodejs-java.features.feature_9.title}"
      content: "{index-content-nodejs-java.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
        ```java {style=abap}
        // Insérez ce modèle sur une page de document :
        // Indicateurs de performance des managers
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Spécifiez le chemin du modèle
        String template = "Bulleted List Template.docx";

        // Définissez le chemin du fichier de sortie
        String result = "Result Report.docx"

        // Récupérez les données des managers à partir d'une source JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Générez le rapport avec les données remplies
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
        ```java {style=abap}   
        // Ajoutez le modèle de titre du graphique à la présentation :
        // Revenus des clients <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Incluez également le modèle de données du graphique :
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Spécifiez le chemin du modèle de graphique
        String template = "Pie Chart Template.pptx";

        // Définissez le chemin du fichier de sortie
        String result = "Result Report.pptx"

        // Récupérez les données des clients à partir d'une source XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Générez le graphique et enregistrez le résultat
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---