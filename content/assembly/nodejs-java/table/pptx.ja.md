



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:05
draft: false
lang: ja
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptを使ってPPTXドキュメントにテーブルを挿入"
head_description: "GroupDocs.Assembly for Node.js via Javaを使用して、さまざまなソースからデータを取得し、ドキュメントやメールにテーブルを素早く埋め込むことができます。"

############################# Header ############################
title: "Node.jsでPPTXファイルにテーブルを容易に追加" 
description: "GroupDocs.Assembly for Node.js via Javaを使用すると、複数のソースからデータを使用してPPTXドキュメントのテーブルを埋めることがシンプルです。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアルを開始"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Javaの紹介"
    link: "/assembly/nodejs-java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)は、ドキュメント作成の自動化を実現する強力なツールです。テーブル、チャート、リスト、画像をテンプレートに挿入し、正確なコンテンツ配置を可能にします。PDF、Word、メールなど、50以上のファイル形式をサポートし、レポート生成やその他のタスクを効率化します。

############################# Steps ############################
steps:
    enable: true
    title: "PPTXにテーブルにデータを追加する方法"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)を使用すると、動的データソースを使用してPPTXファイルのテーブルテンプレートを素早く埋め込むことができます。
      
      1. PPTXテンプレートを作成し、テーブルの行と列のプレースホルダーを追加します。
      2. JSONやCSVなどのサポートされるソースからデータをロードします。
      3. 必要に応じてデータを整理し、フォーマットします。
      4. 完成したテーブルを持つドキュメントを生成します。
   
    code:
      platform: "java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "例の文書"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "コピーするにはクリック"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "他の例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // テーブル行のプレースホルダーにこれらのタグを含めます
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // テンプレートファイルパスを指定します
        const template = "table_template.pptx";

        // 選択したソースからデータをロードします
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // 完成したテーブルを持つ最終ドキュメントを保存します
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "データ駆動型テーブルをドキュメントに追加"
  description: "GroupDocs.Assembly for Node.js via Javaを使用すると、ユーザーはテンプレートベースのワークフローを用いて、チャート、画像、リストを埋め込むとともに、テーブルを自動的に作成できます。"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な機能"
  features:
    # feature loop
    - title: "構造化データからテーブルを生成"
      content: "JSON、XML、CSVなどの形式からデータを取得し、ドキュメントテーブルを自動的に入力します。"

    # feature loop
    - title: "洗練されたビジュアルコンテンツを作成"
      content: "GroupDocs.Assemblyを使用して、プロフェッショナルなテーブル、チャート、リストを設計し、リンク、画像、テキストを追加して洗練されたドキュメントの外観を実現します。"

    # feature loop
    - title: "動的なテーブルコンテンツ配置"
      content: "LINQベースのテンプレートを使用して、プログラム的に行と列を追加し、フォント、色、配置などのスタイルをカスタマイズします。"

    # feature loop
    - title: "フォーマットを超えてシームレスに動作"
      content: "MS Office、OpenOffice、PDF、HTMLなどのフォーマットで簡単にテーブルを作成または編集し、必要に応じてファイルに統合します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラムによりテーブルを埋める方法"
      content: |
        この例では、外部ソースからデータを取得してPPTXドキュメントのテーブルを埋める方法を示します。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // テーブルのプレースホルダーを持つテンプレートを設計します
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // テンプレートのファイルパスを指定します
          const template = "table_template.pptx";

          // 必要なデータをソースからロードします
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // データを必要な構造に整理します
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // DocumentAssemblerを初期化します
          const asm = new assemblyLib.DocumentAssembler();

          // 完成したテーブルを持つ出力ドキュメントを保存します
          asm.assembleDocument(template, "result.pptx", data);
          ```
        platform: "java"
        copy_title: "コピー"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Assemblyの機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "NPMからダウンロード"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "ライセンスについて学ぶ"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主要機能の概要"
    exclude: "table"
    description: "当社のAPIはテーブルの作成を自動化し、多様なツールやテンプレートを使用してドキュメント生成を強化します。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな形式でテーブルを生成"
    exclude: "PPTX"
    description: "Node.js via Javaを使用して、テンプレートを埋め込み、50以上のサポートされるファイルタイプにわたる包括的なテーブルを作成します。"
    items: 
          
        # format loop 1
        - name: "PDFに表を追加"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXに表を追加"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXに表を追加"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXに表を追加"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---