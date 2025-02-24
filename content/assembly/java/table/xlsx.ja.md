



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: ja
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java を使用して XLSX ドキュメントにテーブルを追加"
head_description: "GroupDocs.Assembly for Java を使えば、開発者は動的なソースからデータを引き出して、迅速にドキュメントやメールにテーブルを統合できます。"

############################# Header ############################
title: "Java API で XLSX ファイルに簡単にテーブルを埋め込む" 
description: "GroupDocs.Assembly for Java は、さまざまな入力からデータを読み込んで XLSX ドキュメントのテーブルに埋め込むプロセスを簡素化します。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアルを開始"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java とは？"
    link: "/assembly/java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) は、事前に設計されたテンプレートにデータを自動的に挿入することでドキュメントやレポートを生成するためのツールです。テーブル、リスト、チャート、画像を簡単に追加できます。高度な機能により、ドキュメント内でコンテンツを正確に配置することが可能です。PDF、MS Office、メール形式を含む50以上のファイルタイプに対応しています。

############################# Steps ############################
steps:
    enable: true
    title: "XLSX テーブルにデータを挿入する手順"
    content: |
      [GroupDocs.Assembly](/assembly/java/) は、XLSX および他の形式のテーブルテンプレートを埋めるのを支援します。動的データを利用してテーブルを生成します。
      
      1. XLSX テンプレートを設定し、テーブルの行と列のプレースホルダーを配置します。
      2. サポートされている任意の入力ソースからデータを引き出します。
      3. 必要に応じてデータをフィルタリングまたは前処理します。
      4. 完成したテーブルを持つ最終文書を生成します。
   
    code:
      platform: "java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "例の文書"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "コピーするにはクリック"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "他の例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // テーブル行プレースホルダー内でこれらのタグを使用します
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // テンプレートファイルへのパスを定義します
        String template = "table_template.xlsx";

        // 選択したソースからデータを読み込みます
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // 埋め込まれたテーブルを持つ出力ファイルを保存します
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "データが埋め込まれたテーブルを使ったドキュメント作成"
  description: "GroupDocs.Assembly for Java を利用すれば、ドキュメント内でのテーブル作成の自動化が容易になります。また、テンプレートを使用してチャートやリスト、画像などの要素を追加することもサポートしています。"
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly の主な機能"
  features:
    # feature loop
    - title: "複数のデータ形式からレポートを生成"
      content: "APIは、JSON、XML、CSVなどの形式とシームレスに連携し、整然としたデータでドキュメントのテーブルを埋め込むことができます。"

    # feature loop
    - title: "視覚的に情報を提示"
      content: "GroupDocs.Assembly は、プロフェッショナルなテーブル、リスト、チャートを構築し、リンク、テキスト、画像を挿入して洗練された外観を提供します。"

    # feature loop
    - title: "テーブルの内容を正確に配置"
      content: "柔軟なLINQベースの構文を使用して、行と列を動的に追加できます。フォントスタイルや色などの見た目もプログラム的にカスタマイズできます。"

    # feature loop
    - title: "複数の形式に対応"
      content: "MS Office、OpenOffice、PDF、HTML などと連携して、サポートされている任意のファイル形式に対してテーブルを簡単に統合できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "動的にデータが埋め込まれたテーブルを作成"
      content: |
        この例では、動的な入力データを使用して XLSX ドキュメント内にテーブルを埋め込む方法を示します。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // テーブル用のプレースホルダーを持つテンプレートを設計します
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // テンプレートファイルの場所を設定します
          String template = "table_template.xlsx";

          // 希望するソースからデータを読み込みます
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 必要なフィールドを含むデータオブジェクトを準備します
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // DocumentAssembler のインスタンスを作成します
          DocumentAssembler asm = new DocumentAssembler();

          // テーブルが埋め込まれた文書を保存します
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "コピー"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "コピーするにはクリック"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.xlsx"
        links:
          #  loop
          - title: "他の例"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Assemblyの機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Mavenからダウンロード"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "ライセンスについて学ぶ"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主要機能の概要"
    exclude: "table"
    description: "私たちのAPIは、テーブルの自動埋め込みを含む他の強力なコンポーネントを活用して、プロフェッショナルなドキュメント作成を簡素化します。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな形式で詳細なテーブルを生成"
    exclude: "XLSX"
    description: "Java を使用すれば、データでテンプレートを埋め込み、50以上のファイルタイプで詳細なレポートを生成できます。"
    items: 
          
        # format loop 1
        - name: "PDFに表を追加"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXに表を追加"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXに表を追加"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXに表を追加"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---