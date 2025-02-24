



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: ja
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Javaを使用してDOCXドキュメントにチャートを生成"
head_description: "GroupDocs.Assembly for Java APIは、開発者がドキュメントに動的なチャートやグラフをシームレスに作成および挿入できるようにし、リアルタイムデータで強化されます。"

############################# Header ############################
title: "Java APIを使ってDOCXドキュメントにチャートを追加" 
description: "GroupDocs.Assembly for Javaは、リアルタイムデータを活用してDOCXドキュメントにチャートを埋め込むプロセスを簡素化します。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で始める"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Javaの概要"
    link: "/assembly/java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)は、ドキュメントやレポートの作成を自動化するための多用途なソリューションです。チャート、テーブル、リスト、バーコード、画像を直接ファイルに追加でき、精密なフォーマットやデータ統合のための高度なツールを提供します。このプラットフォームは、PDF、Microsoft Officeファイル、メールなど、50以上のフォーマットをサポートしています。

############################# Steps ############################
steps:
    enable: true
    title: "DOCXドキュメントにチャートを埋め込む手順"
    content: |
      [GroupDocs.Assembly](/assembly/java/)は、DOCXテンプレートにチャートを挿入するプロセスを簡素化します。棒グラフ、円グラフ、折れ線グラフなど、さまざまなチャートスタイルから選択できます。
      
      1. DOCXテンプレートを作成し、チャートのためのプレースホルダーを設けます。
      2. 互換性のあるソースからデータをロードします。
      3. チャートのオプション（タイプ、ラベル、色など）を設定します。
      4. チャートを含むドキュメントを保存します。
   
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
        // チャートを含めるためにテンプレートにこのタグを追加します
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // テンプレートへのファイルパスを指定します
        String template = "chart_template.docx";

        // ソースから必要なデータを抽出します
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // 埋め込まれたチャートを含む最終的なドキュメントを保存します
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "文書に動的チャートを簡単に埋め込む"
  description: "GroupDocs.Assembly for Javaは、人気のフォーマットでデータに富んだ文書を構築するための簡単な方法を提供します。テンプレートを使用して、データからの動的更新を持つチャート、テーブル、バーコード、リスト、リンク、画像を挿入します。"
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な機能"
  features:
    # feature loop
    - title: "データを簡単にチャートに変換"
      content: "APIを使って、JSON、XML、CSVなどのソースからデータをクリーンでプロフェッショナルなチャートに変換できます。"

    # feature loop
    - title: "視覚的にインパクトのあるコンテンツを作成"
      content: "GroupDocs.Assemblyは、棒グラフ、円グラフ、折れ線グラフなど、さまざまな視覚フォーマットをサポートしており、テーブルやバーコード、画像などと組み合わせることで、より充実したレポートを作成できます。"

    # feature loop
    - title: "カスタマイズ可能なチャート配置とスタイル"
      content: "LINQベースの構文を使用することで、ドキュメント内にチャートを動的に生成し配置でき、スタイル、色、レイアウトを容易に調整してデザインニーズに応えられます。"

    # feature loop
    - title: "複数のドキュメントフォーマットをサポート"
      content: "MS Office、PDF、OpenOffice、HTMLなどのフォーマットでドキュメントを生成できます。チャートはサポートされているどのフォーマットにもスムーズに統合され、プロフェッショナルな結果を得られます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラムでチャートを生成・埋め込む"
      content: |
        この例は、DOCXドキュメントにチャートをプログラムで作成し、埋め込む方法を示しています。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // チャート用のプレースホルダーがあるテンプレートを準備します
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // テンプレートへのファイルパスを指定します
          String template = "table_template.docx";

          // 選択したソースからデータをロードします
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 関連情報を持つデータオブジェクトを作成します
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // チャートのタイプと外観を設定します
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // DocumentAssemblerを初期化します
          DocumentAssembler asm = new DocumentAssembler();

          // チャートが埋め込まれた完了したドキュメントを保存します
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "強力な機能を探求"
    exclude: "chart"
    description: "このプラットフォームは、ニーズに合わせたデータ重視で視覚的に魅力的なドキュメントを設計するプロセスを簡素化します。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "多様なフォーマットで包括的なレポートを生成"
    exclude: "DOCX"
    description: "Javaを使って、50以上のファイルフォーマットで統合されたチャートを持つドキュメントを作成し、テンプレートとデータのシームレスなマージを確保します。"
    items: 
          
        # format loop 1
        - name: "PDFにチャートを挿入"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにチャートを挿入"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにチャートを挿入"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにチャートを挿入"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---