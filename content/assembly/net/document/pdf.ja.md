



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: ja
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "PDFファイルにC# APIを使ってドキュメントを組み込む"
head_description: "C#を使用してPDFドキュメントをマージします。GroupDocs.Assemblyを使用して、数ステップでファイルをシームレスに結合できます。"

############################# Header ############################
title: "PDF形式のドキュメントを組み合わせる" 
description: "GroupDocs.Assembly for .NETを使用すれば、1つのPDFドキュメントに別のドキュメントを迅速に組み込むことができます。このAPIは、正確なドキュメント結合のための強力なツールを提供します。"
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NETとは？"
    link: "/assembly/net/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)は、ドキュメントの構成と操作のための強力なツールです。1つのドキュメントを別のドキュメントに組み込むことが可能で、コンテンツをシームレスに結合できます。PDFやMS Officeファイルなど、50以上のフォーマットをサポートしており、要件に応じて最終的な出力を整理・編集・カスタマイズできます。

############################# Steps ############################
steps:
    enable: true
    title: "PDFファイルにドキュメントをマージする方法"
    content: |
      [GroupDocs.Assembly](/assembly/net/)では、1つのPDFファイルに別のドキュメントを簡単に組み込むことができます。コンテンツをマージしてカスタマイズできます。
      
      1. 埋め込むコンテンツのための特定のプレースホルダーを持つテンプレートを設計します（PDFテンプレートはサポートされていません）。
      2. テンプレートのファイルパスを定義します。
      3. 組み込みたいドキュメントのファイルパスを指定します。
      4. 統合されたコンテンツを含む完成ファイルをPDFドキュメントとしてエクスポートします。
   
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
        // 挿入ポイントを示すためにテンプレートにこのタグを追加します
        // <<doc [doc_expression]>>

        // テンプレートのファイルパスを指定します
        // 現在、PDFテンプレートは使用できません。
        string template = "doc_template.docx";

        // 組み込み対象のドキュメントのパスを提供します
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // マージされたドキュメントを保存します
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度なツールでドキュメントの結合を効率化"
  description: "GroupDocs.Assembly for .NETライブラリは、さまざまなファイル形式をサポートし、シームレスな統合のためにカスタマイズを提供します。"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な機能"
  features:
    # feature loop
    - title: "ビジネスデータからレポートを生成"
      content: "JSON、XML、CSVなどのデータソースからドキュメントに自動的にデータを populatesし、正確で効率的なワークフローを保証します。"

    # feature loop
    - title: "視覚要素を用いてドキュメントを豊かに"
      content: "GroupDocs.Assemblyを使用すれば、テーブル、チャート、リスト、テキスト、リンク、画像、動的に生成されたバーコードを含めることができます。"

    # feature loop
    - title: "データを正確に配置・フォーマット"
      content: "LINQベースのテンプレートを通じてデータの配置をコントロールし、配列に対するループを処理し、色のカスタマイズなどのスタイリングを可能にします。"

    # feature loop
    - title: "複数のファイル形式で動作"
      content: "MS Office、PDF、HTML、OpenOfficeなど、さまざまな形式でドキュメントを相互に組み込むことができます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラムからドキュメントに画像を埋め込む方法"
      content: |
        この例では、GroupDocs.Assemblyを使用してPDFドキュメントに画像を挿入する方法を示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // テンプレートにプレースホルダータグを追加します
          // <<image [expression]>>

          // テンプレートのファイルパスを指定します
          // 現在、PDFテンプレートは使用できません。
          string template = "template.docx";

          // 画像ファイルのパスを設定します
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // DocumentAssemblerのインスタンスを初期化します
          DocumentAssembler asm = new DocumentAssembler();

          // 埋め込まれた画像と共にドキュメントを保存します
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "強力なツールを発見"
    exclude: "document"
    description: "GroupDocs.Assemblyが提供する正確なドキュメントの組み込みと結合の機能を探ってみましょう。"
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
    title: "様々なフォーマットのドキュメントをマージ"
    exclude: "PDF"
    description: ".NET APIを使用すれば、50以上のサポートされているフォーマット間でドキュメントを結合可能です。ファイルやセクションを最終ドキュメントに簡単に組み込むことができます。"
    items: 
          
        # format loop 1
        - name: "PDFに文書を埋め込む"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXに文書を埋め込む"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXに文書を埋め込む"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXに文書を埋め込む"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---