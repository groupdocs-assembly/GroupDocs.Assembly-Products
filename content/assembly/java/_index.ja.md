---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: ja
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
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "ドキュメント作成、自動化、レポーティング用のJavaライブラリ"
head_description: "ドキュメント作成とレポート生成を自動化するためのJavaライブラリ。カスタムテンプレートを使用してPDF、Word、Excel、PPTX、HTML、およびメール文書を作成します。"

############################# Header ############################
title: "レポートとドキュメントを自動化するためのJava API"
description: "データをテンプレートとマージすることによって、Javaでのレポート生成を簡素化。"
words:
  for: "のため"

actions:
  main: "Mavenからトライアルを入手"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "始める準備はできましたか？"
  description: "GroupDocs.Assemblyの機能を無料で試すか、ライセンスをリクエストしてください。"

release:
  title: "バージョン{0}リリース"
  notes: "新機能を確認する"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "JavaでDOCXにチャートを生成"
  more: "詳細な例"
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
    // メインテンプレートへのパス
    String template = "chart_template.docx";

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
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assemblyの概要"
  description: "自動化されたドキュメント作成とシームレスなデータ統合のために設計されたJavaライブラリ。"
  features:
    # feature loop
    - title: "Javaでテンプレートにビジネスデータをマージ"
      content: "GroupDocs.Assembly for Javaを使用して、JSON、XML、またはその他のソースからのデータを事前に設計されたテンプレートに簡単に埋め込むことができます。"

    # feature loop
    - title: "埋め込みオブジェクトと作業"
      content: "外部ソースからのデータを用いて、ドキュメント内のテーブル、チャート、および図を自動的に埋め込みます。"

    # feature loop
    - title: "高度なカスタマイズ"
      content: "GroupDocs.Assembly for Javaは、バーコードの生成、URLを介したオンラインデータの取得、さまざまな形式での出力のエクスポートなど、柔軟な機能を提供します。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Assembly for Javaは人気のオペレーティングシステム、開発フレームワーク、およびパッケージマネージャーとシームレスに連携します。"
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
    GroupDocs.Assembly for Javaは幅広い[ドキュメント形式](https://docs.groupdocs.com/assembly/java/supported-document-formats/)をサポートしています。
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
  title: "GroupDocs.Assemblyの主な機能"
  description: "高度なデータ処理を伴ったプロフェッショナルなドキュメントとレポートを作成。"

  items:
    # feature loop
    - icon: "preview"
      title: "視覚データ要素"
      content: "ドキュメント内にチャート、テーブル、画像、リストなどの要素を追加し、フォーマット。"

    # feature loop
    - icon: "manipulate"
      title: "データ変換"
      content: "データを効果的に整理し表示するために、数式やソート、その他のツールを使用。"

    # feature loop
    - icon: "two_pages"
      title: "マルチフォーマットサポート"
      content: "テンプレートと出力ファイルの一般的なファイルタイプで簡単に作業。"

    # feature loop
    - icon: "document_settings"
      title: "強化されたテンプレートフォーマット"
      content: "数値、アルファベットなどの高度なフォーマットオプションでテンプレートをカスタマイズ。"

    # feature loop
    - icon: "text"
      title: "動的なバーコード生成"
      content: "必要に応じてバーコード画像を迅速に作成しドキュメントに挿入。"

    # feature loop
    - icon: "add"
      title: "柔軟なテキストスタイリング"
      content: "テンプレート内で大文字、小文字、タイトルケースなどのテキスト変換を適用。"

    # feature loop
    - icon: "manipulate"
      title: "外部コンテンツのインポート"
      content: "ドキュメントを生成する際に、外部ファイルからのコンテンツを動的に埋め込みます。"

    # feature loop
    - icon: "convert"
      title: "複数フォーマットでのエクスポート"
      content: "指定された拡張子や設定を使用して、最終的なドキュメントをさまざまなファイル形式で保存。"

    # feature loop
    - icon: "update"
      title: "動的メディアの埋め込み"
      content: "ドキュメント作成中にBase64エンコードデータを使用して画像やその他のコンテンツを挿入。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "GroupDocs.Assemblyの一般的なタスク向けのサンプルコードを探求します。"
  items:
    # code sample loop
    - title: "Wordで箇条書きリストを作成"
      content: |
        Word文書に整理されたデータ表現のために[箇条書きリスト](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/)の追加方法を学びます。 この例では、GroupDocs.Assemblyを使用してWordにリストを生成します。
        {{< landing/code title="Wordで箇条書きリストを作成">}}
        ```java {style=abap}
        // ドキュメントページにこのテンプレートを挿入:
        // マネージャーのパフォーマンス指標
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // テンプレートパスを指定
        String template = "Bulleted List Template.docx";

        // 出力ファイルパスを設定
        String result = "Result Report.docx"

        // JSONソースからマネージャーのデータを取得
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // 埋め込まれたデータでレポートを生成
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "PPTXで円グラフを作成"
      content: |
        テンプレートとXMLを使用してプレゼンテーションに[円グラフ](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/)を追加します。 データを視覚化するために円グラフを含めることで、レポートをより魅力的にします。
        {{< landing/code title="PPTXで円グラフを作成">}}
        ```java {style=abap}   
        // プレゼンテーションにチャートタイトルテンプレートを追加:
        // 顧客の収益 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // チャートデータテンプレートも含める:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // チャートテンプレートパスを指定
        String template = "Pie Chart Template.pptx";

        // 出力ファイルパスを設定
        String result = "Result Report.pptx"

        // XMLソースから顧客データを取得
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // チャートを生成して結果を保存
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---