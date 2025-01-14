---
############################# Static ############################
layout: "landing"
date: 2025-01-14T15:37:19
draft: false

lang: ja
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
  for: "のため"

actions:
  main: "{index-content-nodejs-java.actions_main}"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "始める準備はできましたか？"
  description: "GroupDocs.Assemblyの機能を無料で試すか、ライセンスをリクエストしてください。"

release:
  title: "バージョン{0}リリース"
  notes: "新機能を確認する"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "{index-content-nodejs-java.code_title}"
  more: "詳細な例"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // メインテンプレートへのパス
    const template = "chart_template.docx";

    // データソースからマネージャーの生産性データを取得
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // DataSourceInfoのインスタンスをデータで作成
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // 別のDataSourceInfoを使用してチャートの色を設定
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // テンプレートをデータで埋めて出力先に保存
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assemblyの概要"
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
  title: "プラットフォームの独立性"
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
  title: "サポートされているファイル形式"
  description: |
    {index-content-nodejs-java.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office形式
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### 画像およびその他の形式
        * **ポータブル:** PDF
        * **画像:** SVG, TIFF
        * **その他のオフィス形式:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### その他の形式
        * **ウェブ:** HTML, MHTML
        * **メール:** EML, MSG, EMLX
        * **その他:** EPUB, MD

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
  title: "コードサンプル"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
        ```javascript {style=abap}
        // ドキュメントページにこのテンプレートを挿入:
        // マネージャーのパフォーマンス指標
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // テンプレートパスを指定
        const template = "Bulleted List Template.docx";

        // 出力ファイルパスを設定
        const result = "Result Report.docx"

        // JSONソースからマネージャーのデータを取得
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // 埋め込まれたデータでレポートを生成
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
        ```javascript {style=abap} 
        // プレゼンテーションにチャートタイトルテンプレートを追加:
        // 顧客の収益 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // チャートデータテンプレートも含める:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // チャートテンプレートパスを指定
        const template = "Pie Chart Template.pptx";

        // 出力ファイルパスを設定
        const result = "Result Report.pptx"

        // XMLソースから顧客データを取得
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // チャートを生成して結果を保存
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---