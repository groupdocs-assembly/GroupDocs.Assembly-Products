---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: ja
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
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NETドキュメント自動化、アセンブリおよびレポート生成用API"
head_description: "C# .NET APIによるドキュメント自動化、アセンブリ、およびレポート生成。カスタムテンプレートからPDF、Word、Excel、PPTX、HTML、およびメール文書を作成します。"

############################# Header ############################
title: ".NETドキュメント自動化およびレポーティングAPI"
description: ".NETアプリケーションでテンプレートを定義し、データをマージしてレポートを生成。"
words:
  for: "のため"

actions:
  main: "Nugetからトライアルをダウンロード"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "始める準備はできましたか？"
  description: "GroupDocs.Assemblyの機能を無料で試すか、ライセンスをリクエストしてください。"

release:
  title: "バージョン{0}リリース"
  notes: "新機能を確認する"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "C#を使用してDOCXでチャートを埋める"
  more: "詳細な例"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // メインテンプレートへのパス
    string template = "chart_template.docx";

    // データソースからマネージャーの生産性データを取得
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // DataSourceInfoのインスタンスをデータで作成
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // 別のDataSourceInfoを使用してチャートの色を設定
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // テンプレートをデータで埋めて出力先に保存
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assemblyの概要"
  description: ".NETソリューションによる高度なデータ統合を使用したドキュメント作成の自動化。"
  features:
    # feature loop
    - title: "C#でドキュメントテンプレートにビジネスデータを追加"
      content: "GroupDocs.Assembly for .NETを使用すると、JSONやXMLなどのソースからデータを事前定義のテンプレートに簡単に挿入できます。"

    # feature loop
    - title: "ネイティブデータオブジェクトの処理"
      content: "サポートされているドキュメントタイプには、データで自動的にポピュレートできる図、チャート、テーブル、リストなどが含まれます。"

    # feature loop
    - title: "追加機能"
      content: "GroupDocs.Assembly for .NETは幅広いカスタマイズオプションを提供します。プログラムによるデータオブジェクトの設計、バーコードの生成、URL経由でのオンラインデータソースの利用、さまざまな形式での出力の保存が可能です。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Assembly for .NETは以下のオペレーティングシステム、フレームワーク、およびパッケージマネージャーに対応しています。"
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
  title: "サポートされているファイル形式"
  description: |
    GroupDocs.Assembly for .NETは以下の[ファイル形式](https://docs.groupdocs.com/assembly/net/supported-document-formats/)を処理できます。
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
  title: "GroupDocs.Assemblyの機能"
  description: "高度なデータモデルを使用してドキュメントやレポートを作成。"

  items:
    # feature loop
    - icon: "preview"
      title: "高度なデータ表現"
      content: "チャート、リスト、テーブル、画像など幅広いデータオブジェクトをサポート。"

    # feature loop
    - icon: "manipulate"
      title: "データ操作"
      content: "データを効果的に表示するための数式や順序操作を適用。"

    # feature loop
    - icon: "two_pages"
      title: "広範なサポート形式"
      content: "テンプレートや出力ファイル用のすべての一般的なドキュメント形式でシームレスに動作。"

    # feature loop
    - icon: "document_settings"
      title: "リッチテンプレートマークアップ"
      content: "テンプレート内で順序、基数、およびアルファベットの数値形式を活用。"

    # feature loop
    - icon: "text"
      title: "バーコードの埋め込み"
      content: "動的にバーコード画像を生成し、ドキュメントに挿入。"

    # feature loop
    - icon: "add"
      title: "データのフォーマット"
      content: "テンプレート内の文字列を大文字、小文字、頭文字大文字またはその他のスタイルでフォーマット。"

    # feature loop
    - icon: "manipulate"
      title: "ドキュメントコンテンツの操作"
      content: "外部ドキュメントからのコンテンツをダイナミックに挿入。"

    # feature loop
    - icon: "convert"
      title: "複数形式での保存"
      content: "ファイル拡張子または詳細設定を使用して出力ファイル形式を指定。"

    # feature loop
    - icon: "update"
      title: "柔軟なデータ処理"
      content: "Base64でエンコードされたバイトを使用して、動的に画像やドキュメントを挿入。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "GroupDocs.Assemblyの一般的な操作に関するコードスニペット。"
  items:
    # code sample loop
    - title: "Microsoft Word文書に箇条書きリストを作成"
      content: |
        [箇条書きリスト](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/)はビジネスデータを提示する一般的な方法です。 こちらはGroupDocs.Assemblyを使用してWord文書にリストを追加する例です。
        {{< landing/code title="ドキュメントにリストを埋め込む方法">}}
        ```csharp {style=abap}
        // ドキュメントページにこのテンプレートを挿入:
        // マネージャーのパフォーマンス指標
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // テンプレートパスを指定
        string template = "Bulleted List Template.docx";

        // 出力ファイルパスを設定
        string result = "Result Report.docx"

        // JSONソースからマネージャーのデータを取得
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // 埋め込まれたデータでレポートを生成
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "PPTXプレゼンテーションに円グラフを作成"
      content: |
        テンプレートとXMLデータを使用して[円グラフ](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/)を作成できます。 視覚的に魅力的なデータ表現でレポートを強化。
        {{< landing/code title="円グラフを表現する方法">}}
        ```csharp {style=abap}
        // プレゼンテーションにチャートタイトルテンプレートを追加:
        // 顧客の収益 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // チャートデータテンプレートも含める:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // チャートテンプレートパスを指定
        string template = "Pie Chart Template.pptx";

        // 出力ファイルパスを設定
        string result = "Result Report.pptx"

        // XMLソースから顧客データを取得
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // チャートを生成して結果を保存
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---