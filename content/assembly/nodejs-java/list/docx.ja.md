



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: ja
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptでDOCXの動的リストを作成"
head_description: "GroupDocs.Assembly for Node.js via Java APIを使用してDOCXテンプレートにリストをデザインし、挿入します。"

############################# Header ############################
title: "Node.jsを使ったDOCXファイルへのデータ駆動型リストの埋め込み" 
description: "GroupDocs.Assembly for Node.js via Javaは、DOCX文書に柔軟でデータ駆動のリストを追加するための強力なツールを提供します。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で始める"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Javaについて"
    link: "/assembly/nodejs-java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)は、さまざまなソースからデータを取得し、それをテンプレートに埋め込むことで文書作成を簡素化します。リスト、表、チャート、その他の要素を精密に配置し、フォーマットオプションを用いて構築することができます。PDFやMS Office、電子メールを含む50以上のフォーマットに対応し、文書生成プロセスを自動化します。

############################# Steps ############################
steps:
    enable: true
    title: "DOCXファイルにリストを挿入する手順"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)を使用すると、DOCXテンプレートに詳細なデータ駆動型リストを追加することができます。
      
      1. DOCXテンプレートを作成し、リストのプレースホルダーを定義します。
      2. テンプレートのファイルパスを提供します。
      3. JSONやXMLなどのサポートされているソースからデータを読み込みます。
      4. 生成されたリストを含む文書を保存します。
   
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
        // このタグをテンプレートに配置して、リストの挿入位置を指定します
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // テンプレートのファイルパスを設定します
        const template = "list_template.docx";

        // 使用するデータソースからデータを取得します
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // 埋め込まれたリストを含むファイルとして保存します
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "統合データを使った文書の生成"
  description: "GroupDocs.Assembly for Node.js via Javaを使用すると、リスト、表、チャート、その他の要素をテンプレートに埋め込むことができ、時間と労力を節約できます。"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyのハイライト"
  features:
    # feature loop
    - title: "複数のデータソースからのレポート生成"
      content: "JSON、XML、CSVなどのフォーマットからデータをインポートし、リストやその他のコンポーネントを効率的にポピュレートします。"

    # feature loop
    - title: "リストやその他の視覚要素の追加"
      content: "GroupDocs.Assemblyを使用すると、テキスト、画像、リンクと並べてリスト、表、チャートなどをシームレスに埋め込むことができ、洗練された結果を得られます。"

    # feature loop
    - title: "データの正確な配置とスタイル設定"
      content: "LINQベースのテンプレートを使用すると、リストやその他のデータが表示される正確な位置を制御し、繰り返し要素のためのループを使用して、ニーズに合わせたスタイルをカスタマイズできます。"

    # feature loop
    - title: "複数のフォーマットに対応"
      content: "MS Office、PDF、OpenOffice、HTML、電子メールなどのフォーマットで文書を作成します。さまざまなソースからコンテンツを統合して1つのファイルにまとめます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラムで文書にリストを作成する"
      content: |
        この例では、GroupDocs.Assemblyを使用してDOCX文書にリストを動的に追加する方法を示します。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // リスト用のプレースホルダーをテンプレートに追加します
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // テンプレートのファイルパスを指定します
          const template = "numlist_template.docx";

          // リストをポピュレートするためにデータを読み込みます
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // 必要な詳細を含むデータソースを準備します
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // DocumentAssemblerを初期化します
          const asm = new assemblyLib.DocumentAssembler();

          // リストを含む最終文書を保存します
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "GroupDocs.Assemblyの機能を探索"
    exclude: "list"
    description: "強力な統合ツールを使用して、データが豊富な文書を手間なくデザインおよび生成します。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "複数のフォーマットで文書を作成"
    exclude: "DOCX"
    description: "Node.js via Javaは50以上のファイルフォーマットをサポートし、テンプレートとデータを専門的な成果に統合することが簡単です。"
    items: 
          
        # format loop 1
        - name: "PDFにリストを作成"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにリストを作成"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにリストを作成"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにリストを作成"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---