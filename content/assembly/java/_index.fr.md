---
############################# Static ############################
layout: "landing"
date: 2025-03-17T13:11:11
draft: false

lang: fr
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "Bibliothèque Java pour la création, l'automatisation et le reporting de documents"
head_description: "Bibliothèque Java pour automatiser la création de documents et générer des rapports. Créez des documents PDF, Word, Excel, PPTX, HTML et email à l'aide de modèles personnalisés."

############################# Header ############################
title: "API Java pour l'automatisation des rapports et des documents"
description: "Simplifiez la génération de rapports en Java en fusionnant des données avec des modèles."
words:
  for: "pour"

actions:
  main: "Obtenir un essai via Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence."

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Générer un graphique dans DOCX avec Java"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Chemin vers le modèle principal
    String template = "chart_template.docx";

    // Récupérer les données de productivité des managers à partir de la source
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Créer une instance de DataSourceInfo avec les données
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Définir les couleurs du graphique à l'aide d'un autre DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Remplir le modèle avec des données et l'enregistrer en sortie
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Aperçu de GroupDocs.Assembly"
  description: "Une bibliothèque Java conçue pour la création automatisée de documents et l'intégration de données sans effort."
  features:
    # feature loop
    - title: "Fusionner des données commerciales dans des modèles avec Java"
      content: "Créez facilement des rapports professionnels en intégrant des données provenant de JSON, XML ou d'autres sources dans des modèles préconçus en utilisant GroupDocs.Assembly for Java."

    # feature loop
    - title: "Travailler avec des objets intégrés"
      content: "Remplissez automatiquement des éléments tels que des tableaux, graphiques et diagrammes dans des documents en utilisant des données provenant de sources externes."

    # feature loop
    - title: "Personnalisation avancée"
      content: "GroupDocs.Assembly for Java offre des fonctionnalités flexibles telles que la génération de codes-barres, l'extraction de données en ligne via des URL, et l'exportation de la sortie dans différents formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Assembly for Java fonctionne sans effort avec des systèmes d'exploitation, frameworks et gestionnaires de paquets populaires."
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
    GroupDocs.Assembly for Java prend en charge une large gamme de [formats de documents](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Capacités clés de GroupDocs.Assembly"
  description: "Créez des documents et des rapports professionnels avec une gestion avancée des données."

  items:
    # feature loop
    - icon: "preview"
      title: "Éléments de données visuels"
      content: "Ajoutez et formatez des éléments tels que des graphiques, tableaux, images et listes directement dans vos documents."

    # feature loop
    - icon: "manipulate"
      title: "Transformation des données"
      content: "Utilisez des formules, des tris, et d'autres outils pour organiser et présenter vos données efficacement."

    # feature loop
    - icon: "two_pages"
      title: "Prise en charge de plusieurs formats"
      content: "Travaillez facilement avec des types de fichiers courants pour les modèles et les fichiers de sortie."

    # feature loop
    - icon: "document_settings"
      title: "Formatage amélioré des modèles"
      content: "Personnalisez les modèles avec des options de formatage numérique, alphabétique et autres."

    # feature loop
    - icon: "text"
      title: "Génération dynamique de codes-barres"
      content: "Créez et insérez rapidement des images de codes-barres dans les documents selon les besoins."

    # feature loop
    - icon: "add"
      title: "Style de texte flexible"
      content: "Appliquez des transformations de texte comme majuscules, minuscules, casse de titre, ou d'autres styles dans les modèles."

    # feature loop
    - icon: "manipulate"
      title: "Importer du contenu externe"
      content: "Intégrez dynamiquement du contenu provenant de fichiers externes lors de la génération de documents."

    # feature loop
    - icon: "convert"
      title: "Exporter dans plusieurs formats"
      content: "Enregistrez les documents finaux dans divers formats de fichiers en utilisant des extensions ou configurations spécifiées."

    # feature loop
    - icon: "update"
      title: "Incorporation dynamique de médias"
      content: "Insérez des images ou d'autres contenus en utilisant des données encodées en Base64 lors de la création des documents."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Explorez le code d'exemple pour des tâches courantes avec GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Créer une liste à puces dans Word"
      content: |
        Découvrez comment ajouter des [listes à puces](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) aux documents Word pour une représentation organisée des données. Cet exemple montre comment générer une liste dans Word en utilisant GroupDocs.Assembly.
        {{< landing/code title="Créer une liste à puces dans Word">}}
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
    - title: "Créer des graphiques circulaires dans PPTX"
      content: |
        Utilisez des modèles et XML pour ajouter [des graphiques circulaires](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) à vos présentations. Rendez vos rapports plus engageants en incluant des graphiques circulaires pour visualiser les données.
        {{< landing/code title="Créer des graphiques circulaires dans PPTX">}}
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