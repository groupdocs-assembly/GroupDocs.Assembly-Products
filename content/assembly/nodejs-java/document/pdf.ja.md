



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:02
draft: false
lang: ja
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptでPDFのドキュメントをマージする"
head_description: "JavaScriptを使用してPDFファイルを結合します。GroupDocs.Assemblyはドキュメントのマージを数ステップでスムーズに行います。"

############################# Header ############################
title: "PDFファイル内のコンテンツを簡単に結合" 
description: "GroupDocs.Assembly for Node.js via Javaを使用すると、1つのPDFファイルを別のファイルに迅速かつ正確に統合できます。シームレスなマージのための柔軟で信頼性のあるツールをお楽しみください。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で試す"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Javaの概要"
    link: "/assembly/nodejs-java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)は、ドキュメントを管理するための強力な方法を提供します。PDFやMS Officeなど、50を超えるフォーマットをサポートし、他のファイルに1つのファイルを結合します。レイアウトをカスタマイズし、コンテンツを編集し、必要なようにドキュメントを整理できます。

############################# Steps ############################
steps:
    enable: true
    title: "PDFファイルにドキュメントをマージする方法"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)を使用すると、カスタマイズ可能なオプションで1つのPDFファイルを別のファイルに挿入できます。
      
      1. 埋め込むコンテンツのためのプレースホルダーを含むテンプレートを設計します（PDFテンプレートはサポートされていません）。
      2. テンプレートのファイルパスを設定します。
      3. マージするドキュメントのファイルパスを提供します。
      4. マージされたコンテンツを含む最終ドキュメントをPDFファイルとして保存します。
   
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
        // このタグをテンプレートに挿入して、ドキュメントが埋め込まれる場所を定義します
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // メインテンプレートのファイルパスを設定します
        // 現時点ではPDFテンプレートはサポートされていません。
        const template = "doc_template.docx";

        // マージしたいドキュメントのパスを提供します
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // 埋め込まれたドキュメントとともに最終出力を保存します
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ドキュメント統合のための強力なツール"
  description: "GroupDocs.Assembly for Node.js via Javaは、さまざまなフォーマット間でのファイル埋め込みを簡単かつ完全にカスタマイズ可能にします。毎回一貫性のあるプロフェッショナルな結果を提供します。"
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な機能"
  features:
    # feature loop
    - title: "ビジネスデータでレポートを生成"
      content: "JSON、XML、またはCSVソースからデータを取得し、包括的なレポートやドキュメントを迅速かつ正確に作成します。"

    # feature loop
    - title: "リッチな視覚要素を追加"
      content: "GroupDocs.Assemblyを使用すると、テキストやハイパーリンクとともにテーブル、チャート、リスト、画像、バーコードを含めることができます。"

    # feature loop
    - title: "精密なデータ配置"
      content: "LINQテンプレートを使用して、データを正確に配置し、配列などの繰り返しアイテムを処理し、スタイルを簡単にカスタマイズできます。"

    # feature loop
    - title: "さまざまなフォーマットに対応"
      content: "PDF、MS Officeファイル、HTML、OpenOfficeなど、フォーマット間でコンテンツをシームレスにマージし、すべてのプロジェクトに柔軟性を提供します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラム的にドキュメントに画像を埋め込む"
      content: |
        この例では、GroupDocs.Assemblyを使用してPDFファイルに画像を挿入する方法を示します。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 画像のためのプレースホルダーをテンプレートに追加します
          // <<image [expression]>>

          // テンプレートファイルへのパスを指定します
          // 現時点ではPDFテンプレートはサポートされていません。
          String template = "template.docx";
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 埋め込む画像へのパスを設定します
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // DocumentAssemblerオブジェクトを初期化します
          const asm = new assemblyLib.DocumentAssembler();

          // 画像を含むドキュメントを保存します
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "一目でわかるコア機能"
    exclude: "document"
    description: "GroupDocs.Assemblyが提供する効率的でシームレスなドキュメントマージのための包括的なツールを探ります。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "多様なフォーマットでのドキュメントの結合"
    exclude: "PDF"
    description: "Node.js via Javaを使用して、50を超えるファイルフォーマット間でコンテンツを結合し、プロフェッショナルで洗練された結果を保証します。"
    items: 
          
        # format loop 1
        - name: "PDFに文書を埋め込む"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXに文書を埋め込む"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXに文書を埋め込む"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXに文書を埋め込む"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---