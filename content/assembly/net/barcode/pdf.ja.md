



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:52
draft: false
lang: ja
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "PDFドキュメントにC#でバーコードを生成"
head_description: "GroupDocs.Assembly for .NET APIは、開発者がドキュメントやメールにバーコード画像を動的に生成して埋め込むことを可能にします。"

############################# Header ############################
title: "当社の.NET APIを使用してPDFドキュメントにバーコードを追加" 
description: "GroupDocs.Assembly for .NETは、PDFドキュメント内でバーコードを動的に作成および埋め込むための完全なサポートを提供します。"
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
    title: "GroupDocs.Assembly for .NETの概要"
    link: "/assembly/net/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)は、多様なソースからデータを統合して文書やレポートを生成するために設計されています。テキストや数値データで文書を埋め込んだり、チャート、テーブル、リストを作成したり、画像やバーコードをリアルタイムで挿入したりします。高度なマークアップを使用して、データを必要な場所に正確に配置します。PDF、MS Officeファイル、メールを含む50以上のフォーマットをサポートしています。

############################# Steps ############################
steps:
    enable: true
    title: "PDFドキュメントに生成されたバーコードを追加する手順"
    content: |
      [GroupDocs.Assembly](/assembly/net/)は、PDFのようなフォーマットのテンプレートにバーコードを挿入するプロセスを簡素化します。60以上のバーコードタイプをサポートし、1次元および2次元フォーマットが含まれます。
      
      1. バーコード配置用の特定のタグを持つテンプレートを作成します（注意：PDFテンプレートは非互換です）。
      2. サポートされている任意のデータソースからデータを取得します。
      3. バーコードのサイズや解像度などの追加プロパティを設定します。
      4. 挿入されたバーコードを持つ最終文書をPDFとして保存します。
   
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
        // 最終文書にバーコードを生成するために、このタグをテンプレートに挿入します。
        // <<barcode [barcode_expression] -barcode_type>>

        // テンプレートファイルパスを指定します。
        // PDFテンプレートのサポートは、現時点ではありません。
        string template = "barcode_template.docx";

        // ソースからデータを取得します。
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 生成されたバーコードを持つ文書を保存します。
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "データでテンプレートを埋めて文書を生成"
  description: "GroupDocs.Assembly for .NETは、人気のフォーマットで文書を作成するプロセスを簡素化するように設計されています。高度なテンプレートとマークアップを使用して、チャート、リスト、テーブル、ハイパーリンク、画像、バーコードを追加します。"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの機能"
  features:
    # feature loop
    - title: "ビジネスデータからレポートを作成"
      content: "当社のAPIは、JSON、XML、CSVなどのソースからデータを使用して、人気のオフィスフォーマットで文書を効率的に埋め込みます。"

    # feature loop
    - title: "データを表示するためのビジュアル要素の使用"
      content: "GroupDocs.Assemblyは、テキスト、ハイパーリンク、画像、および動的に生成されたバーコードとともに、リスト、テーブル、チャートなどのネイティブ要素を埋め込むことをサポートします。"

    # feature loop
    - title: "文書内の任意の場所にデータを挿入"
      content: "LINQベースの構文を使用して、データを正確に必要な場所に配置します。配列はfor-eachループを使用して挿入でき、フォーマット（例：色）はプログラム的にカスタマイズ可能です。"

    # feature loop
    - title: "幅広いフォーマットをサポート"
      content: "MS Office、OpenOffice、PDF、HTML、さまざまなメールフォーマットなどの人気のファイルフォーマットを処理します。必要に応じて、文書を他の文書に埋め込むことができます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "バーコードを動的に生成する方法"
      content: |
        この例では、PDFドキュメントに動的に生成されたバーコードを埋め込む方法を示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 文書にバーコードを挿入するためにこのテンプレートを使用します。
          // <<barcode [barcode_expression] -barcode_type>>

          // テンプレートファイルへのパスを指定します。
          // PDFテンプレートのサポートは、現時点ではありません。
          string template = "barcode_template.docx";

          // 選択したソースからデータを取得します。
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // 必要なデータのみを持つデータソースオブジェクトを作成します。
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // DocumentAssemblerを初期化します。
          DocumentAssembler asm = new DocumentAssembler();

          // 追加のバーコードプロパティを設定します。
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // 埋め込まれたバーコードを持つ最終文書を保存します。
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "主要機能を探る"
    exclude: "barcode"
    description: "当社のソリューションは、ビジネス文書処理のニーズを効率化するように設計されています。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "人気のフォーマットでレポートを作成"
    exclude: "PDF"
    description: ".NETは、50以上のフォーマットでレポートを生成でき、データとテンプレートをシームレスに結合して優れた結果を得ることができます。"
    items: 
          
        # format loop 1
        - name: "PDFにバーコードを追加"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにバーコードを追加"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにバーコードを追加"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにバーコードを追加"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---