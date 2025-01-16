---
############################# Static ############################
layout: "landing"
date: 2025-01-16T13:04:06
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
head_title: "Node.jsを使用した文書の作成、オートメーション、カスタマイズのためのツールキット"
head_description: "Node.jsを使用して文書ワークフローを自動化するライブラリです。テンプレートからPDF、Word、Excel、PowerPoint、HTML、メールファイルを生成します。"

############################# Header ############################
title: "Node.js APIによる文書とレポートの自動化の簡素化"
description: "事前に構築されたテンプレートとデータを統合してJavaScriptレポート生成を効率化します。"
words:
  for: "のため"

actions:
  main: "NPMで無料トライアルを始める"
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
  title: "Node.jsを使用してWord文書にチャートを作成する"
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
  description: "データ処理が統合されたプログラム的に文書を作成するためのNode.jsライブラリです。"
  features:
    # feature loop
    - title: "JavaScriptを使用してビジネスデータをテンプレートに統合"
      content: "GroupDocs.Assembly for Node.js via Javaを使用してJSON、XML、または他のデータをテンプレートに埋め込むことで洗練されたレポートを生成します。"

    # feature loop
    - title: "埋め込まれたコンテンツの管理"
      content: "外部データを使って文書内のテーブル、チャート、その他のビジュアルを自動的に埋め込みます。"

    # feature loop
    - title: "カスタマイズ可能なオプション"
      content: "GroupDocs.Assembly for Node.js via Javaでは、バーコードの追加、URLからのデータ取得、さまざまな形式でのファイルのエクスポートなどの機能を追加できます。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Assembly for Node.js via Javaは主要なオペレーティングシステム、フレームワーク、およびパッケージマネージャーとスムーズに統合されます。"
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
    GroupDocs.Assembly for Node.js via Javaは多様な[文書フォーマット](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/)をサポートしています。
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
  title: "GroupDocs.Assemblyの主要機能"
  description: "強力なデータ管理ツールを使用して動的な文書とレポートを作成します。"

  items:
    # feature loop
    - icon: "preview"
      title: "リッチデータビジュアル"
      content: "完全にカスタマイズ可能なチャート、表、画像、リストを文書に挿入します。"

    # feature loop
    - icon: "manipulate"
      title: "データの変換"
      content: "情報を効果的に構造化および表示するために、数式やソートなどのツールを活用します。"

    # feature loop
    - icon: "two_pages"
      title: "広範な形式互換性"
      content: "テンプレートや出力のために人気のファイル形式をシームレスに使用します。"

    # feature loop
    - icon: "document_settings"
      title: "高度なテンプレートカスタマイズ"
      content: "数値、アルファベット、その他のスタイルオプションでテンプレートのフォーマットが可能です。"

    # feature loop
    - icon: "text"
      title: "動的なバーコードの生成"
      content: "必要に応じて、文書にバーコード画像を直接作成して埋め込みます。"

    # feature loop
    - icon: "add"
      title: "柔軟なテキストスタイリング"
      content: "テンプレート内で大文字化やタイトルケースなどのテキストスタイルを適用します。"

    # feature loop
    - icon: "manipulate"
      title: "動的なコンテンツ挿入"
      content: "文書生成中に外部ファイルからのコンテンツを動的に含めます。"

    # feature loop
    - icon: "convert"
      title: "さまざまな形式へのエクスポート"
      content: "指定した設定で複数の形式で文書を保存します。"

    # feature loop
    - icon: "update"
      title: "メディアを動的に埋め込む"
      content: "文書作成時にBase64データを使用して画像やその他の要素を挿入します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "GroupDocs.Assemblyを使用して一般的なタスクを実行するための実用的な例を見つけてください。"
  items:
    # code sample loop
    - title: "Word文書に箇条書きリストを追加する"
      content: |
        データを効果的に整理する方法として、Word文書での[箇条書きリスト](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/)の作成方法を確認してください。 この例では、GroupDocs.Assemblyを使用して箇条書きリストを生成する方法を示します。
        {{< landing/code title="Word文書に箇条書きリストを追加する">}}
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
    - title: "PowerPointに円グラフを挿入する"
      content: |
        テンプレートとXMLを使用してプレゼンテーションに[円グラフ](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/)を追加する方法を学びます。 データを視覚的かつ明確に提示するために、円グラフでレポートを強化します。
        {{< landing/code title="PowerPointに円グラフを挿入する">}}
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