



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: ja
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#を使用してPDF文書にリストを生成する"
head_description: "GroupDocs.Assembly for .NET APIは、開発者が動的にデータを埋め込んだリストを文書やテンプレートに作成することを可能にします。"

############################# Header ############################
title: "私たちの.NET APIを使用してPDF文書にデータ駆動型リストを追加する" 
description: "GroupDocs.Assembly for .NETは、PDF文書にリストを動的に生成および埋め込むための強力なツールを提供します。"
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
       [GroupDocs.Assembly for .NET](/assembly/net/)は、さまざまなソースからのデータをシームレスに統合することで、文書やレポートの作成を効率化するように設計されています。リスト、チャート、テーブル、バーコード、またはテキストでテンプレートを埋め、先進的なマークアップを使用してコンテンツを正確に配置します。50以上のフォーマット（PDF、MS Officeファイル、メールなど）に対応しているため、文書ワークフローの自動化に最適です。

############################# Steps ############################
steps:
    enable: true
    title: "PDF文書にデータ埋め込みリストを追加する手順"
    content: |
      [GroupDocs.Assembly](/assembly/net/)は、PDFテンプレートにデータ駆動型のリストを挿入するのを簡潔にします。リストを作成及びカスタマイズします。
      
      1. リストの指定されたスポットを持つテンプレートを作成します（現在、PDFテンプレートはサポートされていません）。
      2. テンプレートへのパスを設定します。
      3. JSONやXMLなどのサポートされているソースからデータを取得します。
      4. リストが含まれた完成文書をPDFファイルとしてエクスポートします。
   
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
        // リストが表示される位置を示すために、テンプレートにこのタグを追加します
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // テンプレートファイルへのパスを指定します
        // PDFテンプレートのサポートは現在ありません。
        string template = "list_template.docx";

        // 選択したソースからデータを取得します
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 生成されたリスト付きの文書を保存します
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "構造化データでテンプレートを埋め込んで文書を作成する"
  description: "GroupDocs.Assembly for .NETは、データ駆動型文書を構築するのを簡単にします。先進的なテンプレートを使用して、リスト、テーブル、バーコード、チャート、画像、その他の要素を動的に追加します。"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 機能"
  features:
    # feature loop
    - title: "ビジネスデータからレポートを生成"
      content: "このAPIは、JSON、XML、CSVなどのソースからのデータを使用して、一般的なフォーマットで文書を正確かつ効率的に埋め込みます。"

    # feature loop
    - title: "データを提示するためにリストや他の要素を使用"
      content: "GroupDocs.Assemblyを使用することで、テキスト、バーコード、ハイパーリンク、および画像とともにリスト、テーブル、チャートを埋め込んで、よく構造化された文書を作成できます。"

    # feature loop
    - title: "必要な場所にデータを正確に挿入"
      content: "LINQベースの構文を活用して、リストや他のデータ要素の位置を正確に指定します。ループを使用してリストを動的に埋め込み、プログラムでカスタムフォーマットを適用します。"

    # feature loop
    - title: "複数の文書フォーマットをサポート"
      content: "MS Office、OpenOffice、PDF、HTML、およびメールファイルなど、さまざまなフォーマットで文書を生成および管理します。複数の文書を一つに簡単に統合できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "リストを動的に生成する方法"
      content: |
        この例は、PDF文書に動的に生成されたリストを埋め込む方法を示しています。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // リスト用にテンプレートにプレースホルダータグを追加します
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // テンプレートファイルへのパスを指定します
          // PDFテンプレートのサポートは現在ありません。
          string template = "numlist_template.docx";

          // リストを埋め込むためのデータを取得します
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // 必要な情報を持つデータソースオブジェクトを作成します
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // DocumentAssemblerを初期化します
          DocumentAssembler asm = new DocumentAssembler();

          // 生成されたリスト付きの最終文書を保存します
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "主要な機能を探索"
    exclude: "list"
    description: "私たちのプラットフォームは、データ駆動型文書コンテンツの作成と統合を簡素化するために構築されています。"
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
    title: "人気のフォーマットで構造化文書を作成"
    exclude: "PDF"
    description: ".NETは50以上のフォーマットをサポートし、データとテンプレートをシームレスに統合して洗練された構造化結果を生成します。"
    items: 
          
        # format loop 1
        - name: "PDFにリストを作成"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにリストを作成"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにリストを作成"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにリストを作成"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---