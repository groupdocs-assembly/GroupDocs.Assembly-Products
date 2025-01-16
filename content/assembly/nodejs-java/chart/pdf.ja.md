



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:00
draft: false
lang: ja
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptを使用してPDFファイルにチャートを挿入"
head_description: "GroupDocs.Assembly for Node.js via Javaを使用することで、開発者はライブデータソースを利用してドキュメントに動的なチャートを迅速に作成し、埋め込むことができます。"

############################# Header ############################
title: "Node.jsを使用してPDFファイルにチャートを追加" 
description: "GroupDocs.Assembly for Node.js via Javaは、リアルタイムデータ入力を用いてPDFドキュメントにチャートを統合するプロセスを簡素化します。"
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "今すぐ無料で始める"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Javaの概要"
    link: "/assembly/nodejs-java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)は、自動化されたドキュメントとレポートを作成するための強力なソリューションです。チャート、表、画像、バーコード、リストを高精度でファイルに追加できます。この多目的プラットフォームは、PDF、Officeドキュメント、メールなど、50以上のフォーマットをサポートしています。

############################# Steps ############################
steps:
    enable: true
    title: "PDFドキュメントにチャートを追加する手順"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)は、PDFファイルにチャートを追加することを簡単にします。バー、折れ線、円形グラフなどのチャートタイプから選択します。
      
      1. チャート用のプレースホルダーを持つテンプレートを作成します（PDFテンプレートはサポートされていません）。
      2. サポートされているソースからデータをロードします。
      3. チャートオプション（タイプ、色、ラベルなど）を設定します。
      4. チャートをPDFファイルとして保存します。
   
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
        // このタグをテンプレートに含めてチャートを生成します
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // テンプレートファイルのパスを指定します
        // 注意：現在、PDFテンプレートはサポートされていません。
        const template = "chart_template.docx";

        // ソースシステムからデータを抽出します
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // 埋め込まれたチャートを持つ最終ドキュメントを保存します
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "ドキュメントにチャートを簡単に埋め込む"
  description: "GroupDocs.Assembly for Node.js via Javaは、一般的なファイルタイプで機能豊かなドキュメントを生成することを簡単にします。テンプレートを使用してリアルタイムデータ更新と共にチャート、表、バーコード、リスト、画像などを追加します。"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な機能"
  features:
    # feature loop
    - title: "データをプロフェッショナルなチャートに変換"
      content: "JSON、XML、CSVなどのソースからデータを変換し、高品質のチャートを作成してドキュメントに直接埋め込むことができます。"

    # feature loop
    - title: "魅力的なビジュアルを作成"
      content: "バーグラフ、円グラフ、折れ線グラフを生成し、他のドキュメント要素（画像、表、バーコードなど）とシームレスに統合します。"

    # feature loop
    - title: "柔軟なチャートスタイリングと配置"
      content: "LINQテンプレートを使用してチャートの位置とスタイルを制御します。色、レイアウト、ラベルを整えて、洗練されたプレゼンテーションを実現します。"

    # feature loop
    - title: "多くのファイルフォーマットに対応"
      content: "MS Office、PDF、OpenOffice、HTMLなどのフォーマットでドキュメントを生成できます。チャートは完璧に統合され、プロフェッショナルな仕上がりになります。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "チャートを動的に生成し挿入する"
      content: |
        この例では、PDFファイルにチャートをプログラムで作成し埋め込む方法を示しています。
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // チャートのプレースホルダーを含むテンプレートを設定します
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // テンプレートファイルへのパスを定義します
          // 注意：現在、PDFテンプレートはサポートされていません。
          const template = "table_template.docx";

          // 選択したソースからデータを取得します
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // チャート情報を含むデータオブジェクトを準備します
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // チャートタイプを選択し、その外観をカスタマイズします
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // DocumentAssemblerを初期化します
          const asm = new assemblyLib.DocumentAssembler();

          // チャートを埋め込んだ更新済みドキュメントを保存します
          asm.assembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "高度な機能を発見"
    exclude: "chart"
    description: "このプラットフォームは、データビジュアライゼーションとシームレスな統合のためのツールを備え、ドキュメント作成を簡素化します。"
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
    title: "複数のファイルフォーマットでレポートを生成"
    exclude: "PDF"
    description: "Node.js via Javaは50以上のフォーマットをサポートしているため、テンプレートとデータを組み合わせて、洗練されたドキュメントを簡単に作成できます。"
    items: 
          
        # format loop 1
        - name: "PDFにチャートを挿入"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにチャートを挿入"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにチャートを挿入"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにチャートを挿入"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---