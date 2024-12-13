---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: fr
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

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
head_title: "API .NET pour l'automatisation des documents, assemblage et génération de rapports"
head_description: "API C# .NET pour l'automatisation des documents, l'assemblage et la génération de rapports. Créez des documents PDF, Word, Excel, PPTX, HTML et email à partir de modèles personnalisés."

############################# Header ############################
title: "API d'automatisation des documents et de reporting .NET"
description: "Générez des rapports dans des applications .NET en définissant des modèles et en fusionnant des données."
words:
  for: "pour"

actions:
  main: "Téléchargez l'essai via NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Assembly gratuitement ou demandez une licence."

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"

code:
  title: "Remplir un graphique dans DOCX en utilisant C#"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Chemin vers le modèle principal
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Aperçu de GroupDocs.Assembly"
  description: "Solution .NET pour automatiser la création de documents avec intégration de données avancée."
  features:
    # feature loop
    - title: "Ajouter des données commerciales aux modèles de documents avec C#"
      content: "Génération de rapports simplifiée : Avec GroupDocs.Assembly for .NET, vous pouvez insérer sans effort des données provenant de sources comme JSON ou XML dans des modèles prédéfinis."

    # feature loop
    - title: "Traiter des objets de données natifs"
      content: "Les types de documents pris en charge incluent des objets intégrés comme des diagrammes, graphiques, tableaux et listes qui peuvent être remplis automatiquement avec des données."

    # feature loop
    - title: "Fonctionnalités supplémentaires"
      content: "GroupDocs.Assembly for .NET offre d'importantes options de personnalisation. Concevez des objets de données par programmation, générez des codes-barres, utilisez des sources de données en ligne via des URL, et enregistrez la sortie dans divers formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Assembly for .NET est compatible avec les systèmes d'exploitation, frameworks et gestionnaires de paquets suivants."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Assembly for .NET peut traiter les [formats de fichiers suivants](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "Fonctionnalités de GroupDocs.Assembly"
  description: "Créez des documents et des rapports en utilisant des modèles de données avancés."

  items:
    # feature loop
    - icon: "preview"
      title: "Représentation avancée des données"
      content: "Prend en charge un large éventail d'objets de données tels que des graphiques, listes, tableaux, images, et plus encore."

    # feature loop
    - icon: "manipulate"
      title: "Manipulation des données"
      content: "Appliquez des formules et des opérations séquentielles pour formater et afficher les données efficacement."

    # feature loop
    - icon: "two_pages"
      title: "Large éventail de formats pris en charge"
      content: "Travaillez sans effort avec tous les formats de documents courants pour les modèles ou fichiers de sortie."

    # feature loop
    - icon: "document_settings"
      title: "Balisage riche des modèles"
      content: "Exploitez le formatage ordinal, cardinal et numérique alphabétique dans les modèles."

    # feature loop
    - icon: "text"
      title: "Incarner des codes-barres"
      content: "Générez des images de codes-barres dynamiquement et insérez-les dans vos documents."

    # feature loop
    - icon: "add"
      title: "Formatage des données"
      content: "Formatez les chaînes dans les modèles en majuscules, minuscules, capitalisées ou avec un style de première lettre en majuscule."

    # feature loop
    - icon: "manipulate"
      title: "Manipulation du contenu des documents"
      content: "Insérez dynamiquement du contenu provenant de documents externes dans vos rapports."

    # feature loop
    - icon: "convert"
      title: "Enregistrer dans plusieurs formats"
      content: "Spécifiez le format de fichier de sortie à l'aide d'extensions de fichiers ou de configurations détaillées."

    # feature loop
    - icon: "update"
      title: "Traitement des données flexible"
      content: "Insérez des images et des documents dynamiquement en utilisant des octets encodés en Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Exemples de code pour les opérations typiques de GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Liste à puces dans un document Microsoft Word"
      content: |
        [Les listes à puces](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) sont un moyen courant de présenter des données commerciales. Voici un exemple d'ajout d'une liste à un document Word en utilisant GroupDocs.Assembly.
        {{< landing/code title="Comment remplir une liste dans les documents">}}
        ```csharp {style=abap}
        // Insérez ce modèle sur une page de document :
        // Indicateurs de performance des managers
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Spécifiez le chemin du modèle
        string template = "Bulleted List Template.docx";

        // Définissez le chemin du fichier de sortie
        string result = "Result Report.docx"

        // Récupérez les données des managers à partir d'une source JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Générez le rapport avec les données remplies
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Graphiques circulaires dans des présentations PPTX"
      content: |
        Vous pouvez créer [des graphiques circulaires](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) en utilisant des modèles et des données XML. Améliorez vos rapports avec des représentations de données visuellement attrayantes.
        {{< landing/code title="Comment représenter des données dans un graphique circulaire">}}
        ```csharp {style=abap}
        // Ajoutez le modèle de titre du graphique à la présentation :
        // Revenus des clients <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Incluez également le modèle de données du graphique :
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Spécifiez le chemin du modèle de graphique
        string template = "Pie Chart Template.pptx";

        // Définissez le chemin du fichier de sortie
        string result = "Result Report.pptx"

        // Récupérez les données des clients à partir d'une source XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Générez le graphique et enregistrez le résultat
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---