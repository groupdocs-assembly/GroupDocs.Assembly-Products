



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: ja
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Javaを使用してPDFドキュメントにリストを作成"
head_description: "GroupDocs.Assembly for Java APIを使用して、動的なリストをPDFテンプレートに設計して埋め込むことが可能です。"

############################# Header ############################
title: "当社のJava APIを使用してPDFファイルに動的リストを追加" 
description: "GroupDocs.Assembly for Javaは、PDFドキュメントにデータ豊富なリストを生成し挿入するための柔軟なツールを提供します。"
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で試す"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Javaとは?"
    link: "/assembly/java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)は、複数のソースからデータを取得してプロフェッショナルなドキュメントを設計することを可能にします。これを使用して、リスト、表、チャート、またはテキストを作成し、高度なテンプレート機能を使ってこれらの要素を必要な場所に配置できます。PDFやMS Officeファイル、メールドキュメントなど、50以上のフォーマットをサポートし、ワークフローの自動化と効率化を手助けします。

############################# Steps ############################
steps:
    enable: true
    title: "PDFドキュメントにデータ駆動型リストを追加する方法"
    content: |
      [GroupDocs.Assembly](/assembly/java/)を使用すると、PDFテンプレートにデータリッチなリストを迅速に挿入できます。コンテンツをカスタマイズして整理することができます。
      
      1. テンプレートを設計し、リスト用のプレースホルダーを指定します（PDFテンプレートはサポートされていません）。
      2. テンプレートへのファイルパスを設定します。
      3. JSONやXMLなどのサポートされているフォーマットからデータを取得します。
      4. リストを含む最終ドキュメントをPDFとして保存します。
   
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
        // リストが表示されるべきテンプレートにこのタグを含めます
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // テンプレートのファイルパスを定義します
        // 現時点ではPDFテンプレートはサポートされていません。
        String template = "list_template.docx";

        // 選択したソースからデータを引き出します
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 埋め込まれたリストを持つドキュメントを保存します
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "データ統合からテンプレートを生成"
  description: "GroupDocs.Assembly for Javaは、動的なリスト、表、チャート、その他のコンポーネントをドキュメントテンプレートに簡単に追加することができます。"
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assemblyの主な機能"
  features:
    # feature loop
    - title: "さまざまなソースからのデータでレポートを構築"
      content: "JSON、XML、CSVなどのフォーマットからデータを使用して、リストやその他のコンポーネントを効率的に埋め込みます。"

    # feature loop
    - title: "シームレスにリストやその他のデータ要素を追加"
      content: "GroupDocs.Assemblyは、テキスト、画像、リンクとともにリスト、チャート、表などを埋め込むことを可能にし、洗練されたドキュメントを作成します。"

    # feature loop
    - title: "データが表示される場所を正確に制御"
      content: "LINQベースのテンプレートを使用すると、リストやデータの正確な位置を定義できます。ループを使用して詳細なリストを自動的に作成し、カスタムフォーマットを適用します。"

    # feature loop
    - title: "さまざまなドキュメントフォーマットをサポート"
      content: "MS Office、PDF、OpenOffice、HTML、メールなどのフォーマットでファイルを作成または編集します。必要に応じて、複数のドキュメントの内容を統合します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "プログラムでリストを作成する方法"
      content: |
        この例では、GroupDocs.Assemblyを使用してPDFファイルに動的にリストを追加する方法を示します。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // リスト用のプレースホルダータグをテンプレートに追加します
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // テンプレートへのファイルパスを指定します
          // 現時点ではPDFテンプレートはサポートされていません。
          String template = "numlist_template.docx";

          // リストを埋め込むために必要なデータを引き出します
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // 必要な詳細でデータソースを準備します
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // DocumentAssemblerを初期化します
          DocumentAssembler asm = new DocumentAssembler();

          // 完成したリストで出力ドキュメントを保存します
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "GroupDocs.Assemblyの機能を発見"
    exclude: "list"
    description: "高度なデータ統合ツールを使用して、コンテンツリッチなドキュメントを簡単に設計および生成します。"
    items: 
          
        # operation loop 1
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "文書にバーコードを動的に作成して追加"

        # operation loop 2
        - name: "図を用いてデータを視覚化"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "さまざまな図のタイプにデータを埋め込む"

        # operation loop 3
        - name: "文書を統合"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "1つの文書の内容を別の文書に組み合わせる"

        # operation loop 4
        - name: "リストを使ってデータを表示"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "特定のデータを使用して文書内にリストを生成"

        # operation loop 5
        - name: "表にデータを整理"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "任意のソースからデータを取得し、表を埋める"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまなフォーマットでドキュメントを生成"
    exclude: "PDF"
    description: "Javaは50以上のフォーマットをサポートしており、データとテンプレートを結合して構造化されたドキュメントを作成できます。"
    items: 
          
        # format loop 1
        - name: "PDFにリストを作成"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにリストを作成"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにリストを作成"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにリストを作成"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---