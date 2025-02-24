



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: ja
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#を使用してPPTX文書にテーブルを作成"
head_description: "GroupDocs.Assembly for .NET APIは、開発者が動的ソースからデータを使って文書やメールにテーブルを簡単に追加・入力できるようにします。"

############################# Header ############################
title: "私たちの.NET APIを使用してPPTX文書にデータテーブルを生成" 
description: "GroupDocs.Assembly for .NETは、さまざまなソースからのデータを使用して、PPTX文書内のテーブルを動的に埋めることを可能にします。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアルをダウンロード"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET 概要"
    link: "/assembly/net/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)は、複数のソースからのデータを使ってテンプレートを埋めることで、文書やレポートを作成するために設計されています。構造化データをテーブル、リスト、チャートにシームレスに挿入したり、画像を動的に埋め込んだりできます。高度な構文により、正確なデータ配置が実現されます。PDF、MS Office文書、メールファイルなど50以上のフォーマットをサポートしています。

############################# Steps ############################
steps:
    enable: true
    title: "PPTX文書のテーブルを埋める方法"
    content: |
      [GroupDocs.Assembly](/assembly/net/)を使用すると、PPTXのようなフォーマットでテンプレート内のテーブルを動的に埋め込むことができます。さまざまなソースからデータを挿入します。
      
      1. PPTXテンプレートを作成し、テーブルのプレースホルダーを追加します。
      2. 任意のサポートされているソースからデータを取得します。
      3. 必要な情報のみを含むようにデータをフィルタリングします。
      4. 埋め込まれたテーブルを持つ文書を保存します。
   
    code:
      platform: "net"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "例の文書"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "コピーするにはクリック"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "他の例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // テンプレートテーブル行にこれらのタグを追加
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // テンプレートのファイルパスを設定
        string template = "table_template.pptx";

        // サポートされているソースからデータを取得
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // データで埋められたテーブルを持つ文書を保存
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "動的なテーブルを持つ文書を生成"
  description: "GroupDocs.Assembly for .NETは、テンプレートと高度なマークアップを通じてテーブルの自動入力を加速し、チャート、リスト、画像などの追加要素をサポートすることで文書作成を効率化します。"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な特徴"
  features:
    # feature loop
    - title: "構造化データからレポートを作成"
      content: "APIは、JSON、XML、CSVなどのソースからのデータを処理し、オフィス文書にテーブルを効率的かつ正確に埋め込みます。"

    # feature loop
    - title: "データを視覚的に表示"
      content: "GroupDocs.Assemblyは、プロフェッショナルな文書デザインのために、テーブル、リスト、チャートを作成し、テキスト、リンク、画像を埋め込むことを可能にします。"

    # feature loop
    - title: "テーブルデータを精確に配置"
      content: "LINQベースの構文を使用して、動的にテーブルの行や列を追加します。色やフォーマットなどのスタイルをプログラム的にカスタマイズします。"

    # feature loop
    - title: "幅広いフォーマットをサポート"
      content: "MS Office、OpenOffice、PDF、HTMLなどの人気のファイルフォーマットを簡単に扱えます。サポートされている文書タイプに埋め込まれたテーブルをシームレスに挿入します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "データテーブルを動的に埋め込む方法"
      content: |
        この例では、動的データを使用してPPTX文書内のテーブルを埋める方法を示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // テーブル用のプレースホルダーを持つテンプレートを準備
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // テンプレートへのファイルパスを指定
          string template = "table_template.pptx";

          // 選択したソースからデータを取得
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 必要なデータを持つデータソースオブジェクトを作成
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // DocumentAssemblerを初期化
          DocumentAssembler asm = new DocumentAssembler();

          // 埋め込まれたテーブルを持つ完成文書を保存
          asm.AssembleDocument(template, "result.pptx", data);
          ```
        platform: "net"
        copy_title: "コピー"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "コピーするにはクリック"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.pptx"
        links:
          #  loop
          - title: "他の例"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Assemblyの機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Nugetからダウンロード"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "ライセンスについて学ぶ"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主な機能を探る"
    exclude: "table"
    description: "私たちのソリューションは、動的に埋め込まれたテーブルと追加要素を持つプロフェッショナルな文書の作成を簡素化します。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "詳細なテーブルを持つレポートを作成"
    exclude: "PPTX"
    description: ".NETは、50以上のサポートフォーマットでテンプレートにテーブルやその他のデータ要素を埋め込むことで、包括的なレポートを作成できます。"
    items: 
          
        # format loop 1
        - name: "PDFに表を追加"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXに表を追加"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXに表を追加"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXに表を追加"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---