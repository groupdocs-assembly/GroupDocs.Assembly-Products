



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: ja
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# ファイルで PPTX のチャートを作成する"
head_description: "GroupDocs.Assembly for .NET API は、開発者がリアルタイムデータを使用して文書に動的にチャートやグラフを生成し挿入することを可能にします。"

############################# Header ############################
title: ".NET API を使用して PPTX ファイルにチャートを埋め込む" 
description: "GroupDocs.Assembly for .NET は、PPTX ファイルに動的データを追加し、チャートをシームレスに統合するための強力な方法を提供します。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で試す"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET とは？"
    link: "/assembly/net/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) は、さまざまなソースからのデータを統合することにより、文書やレポートの作成を効率化するために設計されたツールです。チャート、テーブル、リスト、バーコード、画像を動的に生成できます。高度なフォーマットオプションにより、コンテンツの正確な配置とカスタマイズが可能です。50 以上のファイル形式をサポートしており、PDF、MS Office ドキュメント、およびメールも含まれます。

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 文書にチャートを追加する方法"
    content: |
      [GroupDocs.Assembly](/assembly/net/) は、PPTX テンプレートにチャートを生成し埋め込む作業を簡単にします。棒グラフ、円グラフ、折れ線グラフなどのさまざまなチャートタイプをサポートしています。
      
      1. PPTX テンプレートを設計し、チャートのためのプレースホルダーを配置します。
      2. 互換性のあるソースからデータを取得します。
      3. タイプ、ラベル、カラー スキームなどのチャートオプションを定義します。
      4. チャートが埋め込まれた状態で更新されたファイルを保存します。
   
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
        // テンプレートにこのタグを追加してチャートを生成します。
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // テンプレートのファイルパスを指定します。
        string template = "chart_template.pptx";

        // 希望のソースからデータを読み込みます。
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // チャートを埋め込んだ文書を保存します。
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "動的なチャートをドキュメントに簡単に追加"
  description: "GroupDocs.Assembly for .NET は、広く使用されている形式でデータ主導の文書を作成する手順を簡素化します。テンプレートを使用して、チャート、テーブル、バーコード、リスト、ハイパーリンク、および画像を高度な動的データ統合で挿入します。"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly の主な機能"
  features:
    # feature loop
    - title: "データをプロフェッショナルなチャートに変換"
      content: "JSON、XML、CSV などのソースからデータを視覚的に魅力的なチャートに変換するのに、API で数ステップで実現可能です。"

    # feature loop
    - title: "視覚的に魅力的なコンテンツを作成"
      content: "GroupDocs.Assembly は、棒グラフ、円グラフ、折れ線グラフなど、複数のチャートタイプをサポートしています。これらとテーブル、バーコード、画像、その他の要素を組み合わせて、プロフェッショナルなレポートを作成できます。"

    # feature loop
    - title: "チャートを正確に配置しカスタマイズ"
      content: "LINQ 構文を使用することで、必要な場所にチャートを動的に生成し配置できます。スタイル、色、レイアウトを簡単にカスタマイズし、要件に合わせることが可能です。"

    # feature loop
    - title: "さまざまなファイル形式で機能"
      content: "MS Office、PDF、OpenOffice、HTML などの一般的な形式で文書を生成します。対応する形式でシームレスにチャートを埋め込むことができ、完全な互換性があります。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラムでチャートを作成"
      content: |
        この例では、PPTX 文書にチャートを動的に作成して埋め込む方法を示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // チャートのためのプレースホルダーを持つテンプレートを準備します。
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // テンプレートファイルのパスを提供します。
          string template = "table_template.pptx";

          // ソースからデータを取得します。
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 必要な情報を持つデータオブジェクトを構築します。
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // タイプや外観などのチャートプロパティを設定します。
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // DocumentAssembler を初期化します。
          DocumentAssembler asm = new DocumentAssembler();

          // チャートを含む文書をエクスポートします。
          asm.AssembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "主な機能を発見"
    exclude: "chart"
    description: "私たちのプラットフォームは、ニーズに合わせた魅力的でデータ主導の文書を作成するのに役立ちます。"
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
    title: "複数の形式で視覚的に豊かなレポートを作成"
    exclude: "PPTX"
    description: ".NET を使用すると、50 以上のサポート形式でチャートが統合された文書を生成でき、テンプレートをデータとシームレスに組み合わせることができます。"
    items: 
          
        # format loop 1
        - name: "PDFにチャートを挿入"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにチャートを挿入"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにチャートを挿入"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにチャートを挿入"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---