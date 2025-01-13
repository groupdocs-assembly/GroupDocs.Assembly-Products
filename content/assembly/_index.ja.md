---
############################# Static ############################
layout: "family"
date:  2025-01-13T15:11:22
draft: false

product: "Assembly"
product_tag: "assembly"

lang: ja

############################# Head ############################
head_title: "GroupDocsによる.NETおよびJavaのAPIとオンラインドキュメント生成アプリ"
head_description: ".NETおよびJavaアプリケーションのためのオールインワンドキュメント自動化・レポーティングソリューション。カスタムテンプレートとデータから一般的なドキュメントを生成します。"

############################# Header ############################
title: "ドキュメント自動化およびレポーティングソリューション"
description:  |
  クロスプラットフォームアプリおよびAPIを使用して、テンプレートとデータソースを利用した詳細なレポートを作成します。

  柔軟なマークアップを使用して、Word、Excel、プレゼンテーションなどの形式でレポートを生成します。

  JSON、XML、CSVなどのデータソースからデータを用いて、チャート、バーコード、表、およびその他の要素をポピュレートします。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "プラットフォームを選択してください"
  title: "プラットフォームの独立性"
  description: "GroupDocs.Assemblyは以下のオペレーティングシステムおよびフレームワークに対応しています:"
  details_link_title: "詳細を学ぶ"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> その他のテキストエディタ
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Assemblyの主な機能"
  description: "このソリューションは、ビジネスデータで自動的に埋め込まれた人気のあるドキュメント形式でレポートを作成するのに役立ちます。ドキュメント生成タスクを自動化します。"

  items:
    # items loop
    - icon: "additional"
      title: "データでテンプレートを埋める"
      content: "サポートされているソースからデータを使用してレポートを埋める。"

    # items loop
    - icon: "manipulate"
      title: "柔軟なマークアップ"
      content: "カスタマイズ可能な方法でドキュメントにデータを追加。"

    # items loop
    - icon: "structure"
      title: "ネイティブドキュメント機能"
      content: "テーブル、チャート、バーコードを使用してデータを表示。"

    # items loop
    - icon: "merge"
      title: "すべての一般的な形式"
      content: "すべての一般的に使用されるドキュメント形式をサポート。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "カスタマイズされたレポートを生成"
  description: "GroupDocs.Assemblyのコード例"
  items:
    # code sample loop
    - title: "生成されたバーコードを使用"
      content: |
       GroupDocs.Assemblyはレポートテンプレートにバーコードのマークアップを許可します。レポートを作成する際に、マークアップと提供されたデータに基づいてバーコードが生成されます。テキスト、データオブジェクト、およびマークアップを含むテンプレートへのパスを指定します。また、バーコードにコンテンツを埋め込むデータソースを指定します。
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // DocumentAssemblerクラスのインスタンスを作成
            DocumentAssembler assembler = new DocumentAssembler();

            //テンプレートへのパスを指定
            var tmp_path = "barcode_template.docx";

            //結果ドキュメントへのパスを指定
            var res_path = "result.docx";

            //データソースのインスタンスを作成
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //AssembleDocumentを呼び出してレポートを生成
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // DocumentAssemblerクラスのインスタンスを作成
            DocumentAssembler assembler = new DocumentAssembler();
            
            //テンプレートへのパスを指定
            String tmp_path = "barcode_template.docx";

            //結果ドキュメントへのパスを指定
            String res_path = "result.docx";

            //データソースのインスタンスを作成
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // AssembleDocumentを呼び出してレポートを生成
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // DocumentAssemblerクラスのインスタンスを作成
            const assembler = new assemblyLib.DocumentAssembler();
            
            //テンプレートへのパスを指定
            const tmp_path = "barcode_template.docx";

            //結果ドキュメントへのパスを指定
            const res_path = "result.docx";

            //データソースのインスタンスを作成
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // AssembleDocumentを呼び出してレポートを生成
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "50以上のファイル形式をサポート"
  description: "GroupDocs.Assemblyはほぼすべての人気ファイル形式で動作します。"

############################# Metrics ###############################
metrics:
  enable: true
  title: "製品の統計"
  description: "製品のメトリクスを探求し、進捗、影響、成長についての洞察を得ましょう。"

  items:
    # items loop
    - number: "50+"
      title: "サポートされている形式"
      content: "最も広く使用されている50以上のドキュメント形式をサポートしています。"

    # items loop
    - number: "650k"
      title: "NuGetダウンロード数"
      content: "GroupDocs.Assembly for .NETは、NuGetで65万回以上ダウンロードされた人気のライブラリです。"

    # items loop
    - number: "18k"
      title: "Mavenダウンロード数"
      content: "Java開発者は、MavenでGroupDocs.Assemblyを18000回以上ダウンロードしています。"

    # items loop
    - number: "150+"
      title: "満足している顧客"
      content: "私たちの製品は、世界中の個々の開発者や大手企業に信頼され、革新的なソリューションを作成するために使用されています。"


############################# Customers ###############################
customers:
  enable: true
  title: "私たちの満足した顧客"
  description: "GroupDocsのライブラリは、世界中の著名なブランドの一部によって使用されています。"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "お使いのプラットフォームでGroupDocs.Assemblyの機能を無料でお試しください。"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "よくある質問"
  description: "よくある質問を参照してください。"

  items:
    # items loop
    - question: "GroupDocs.Assemblyはドキュメント作成のために外部ライブラリを必要としますか？"
      answer: "いいえ、GroupDocs.Assemblyは独立して動作し、Adobe AcrobatやMicrosoft Officeなどのサードパーティライブラリは必要ありません。"

    # items loop
    - question: "GroupDocs.Assemblyの機能を購入前に試すことはできますか？"
      answer: "はい、できます！GroupDocs.Assemblyは無料体験を提供しています。それをインストールして機能を探索してください。トライアルバージョンは、ドキュメントに「トライアルバッジ」を追加し、最初の3ページのみを処理します。完全な体験をするために、すべての機能にアクセスできる30日間の一時ライセンスを取得してください。詳細は[一時ライセンス](https://purchase.groupdocs.com/temporary-license/)をご覧ください。"

    # items loop
    - question: "どのようなライセンスが利用可能ですか？"
      answer: "GroupDocs.Assemblyライセンスをお探しですか？お客様のニーズに応じたさまざまなオプションを提供しています。チームのサイズ、展開場所（単一オフィスまたはリモート）、お客様がクライアントにSDK/APIを配布するために共有する必要があるかどうかに応じて選択してください。もしくは、使用した分だけ支払うメーター制のプランがある月額使用ライセンスを選択できます。自分に最適なオプションを[価格設定](https://purchase.groupdocs.com/pricing/assembly/net/)で見つけてください。"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.AssemblyのローコードAPI"
  description: "クラウドベースのREST APIを介してアプリケーションを使用してドキュメントを生成します。"
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "cURL RESTful APIを使用して、Word、Excel、PowerPointなどのテンプレートにデータを追加します。"
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: ".NETアプリケーションを強化し、クラウドSDKを介してレポートを生成します。ビジネスデータをカスタム形式で表示。"
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDKは、Javaアプリケーション向けにさまざまな種類のドキュメントを生成するオプションを提供します。"
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.AssemblyのWebアプリ"
  description: "GroupDocs.Assemblyは、ドキュメントを生成するための無料Webアプリケーションを提供します。ブラウザ上で50を超える人気ファイル形式を直接処理できます、無料で。"

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Excel、Word、PowerPointなどのファイルタイプでレポートを生成し、ブラウザから直接それを行います。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "テンプレートとデータソースからMicrosoft Wordドキュメントを作成。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "テンプレートとデータソースをアップロードして、Excelレポートを無料で生成。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---