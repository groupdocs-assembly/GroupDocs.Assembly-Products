---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

head_title: ".ドキュメント自動化、アセンブリ、レポート生成のためのNET API"
head_description: "C＃.NETドキュメントの自動化、アセンブリ、レポート生成API。カスタムテンプレートからPDFWordExcelPPTXHTMLおよび電子メールドキュメントを作成する."

title: ".NET Document Automation＆Reporting API"
description: "テンプレートを定義し、データをマージして、.NETアプリケーションでレポートを生成する."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
        product: "GroupDocs.Assembly"
        platform: ".NET"

    middle:
        button:
            - link: "#overview"
              text: "概要"

            - link: "#features"
              text: "特徴"

            - link: "#support"
              text: "サポート"

            - link: "https://products.groupdocs.app/assembly"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Assembly for .NET APIは、C＃、ASP.NET、およびその他の.NET関連アプリケーションでカスタマイズされたテンプレートからレポートを生成する機能を備えた強力なドキュメント自動化およびレポート生成アプリケーションを構築するのに役立ちます。わずか数行のコードで、.NETレポートライブラリは、定義されたドキュメントテンプレートから指定されたデータをインテリジェントにアセンブルし、さまざまなデータソース（データベース、XML、JSON、ODATA、CSV、カスタム.NETオブジェクト）。  

      LINQベースのテンプレート構文をサポートしており、ユーザーは、PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシート、PowerPointプレゼンテーション、スライドなど、一般的に使用されるすべてのビジネスファイル形式で出力ドキュメントを簡単に生成できます。テンプレート要素のフォーマットプロパティは、テキスト、HTMLおよび条件付きブロック、画像、チャート、バーコード、ハイパーリンク、ピボットテーブルなどを操作することによっても構成できます。  

      GroupDocs.Assembly for .NETを使用して、.NETプラットフォームを対象とする任意の開発環境でアプリケーションを開発できます。すべての.NETベースの言語と互換性があり、Monoまたは.NETフレームワーク（.NET Coreを含む）をインストールできる一般的なオペレーティングシステム（Windows、Linux、MacOS）をサポートします。
    tabs:
      enable: true
      
      tab_one:
        description: |
          以下は、GroupDocs.Assemblyfor.NETの概要です。
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "概要"
          content: |
            *データの定式化
            *データフォーマット
            *データの自動化
            *テンプレートを作成
            *テンプレート要素のフォーマット
            *レポートの生成
      
      tab_two:
        description: |
          .NETドキュメント生成APIでサポートされている[ドキュメントファイル形式]（https://docs.groupdocs.com/assembly/net/supported-document-formats/）を以下に示します。

        left:
          enable: true
          table:
            - title: "MicrosoftOfficeの形式"
              content: |
                * ** Word **：DOC、DOCX、DOT、DOTX、DOTM、DOCM、RTF、WordprocessingML（XML）
                * ** Excel **：XLS、XLSX、XLSM、XLSB、XLT、XLTM、XLTX、SpreadsheetML（XML）
                * ** PowerPoint **：PPT、PPTX、PPTM、PPS、PPSX、PPSM、POTX、POTM
                * ** Outlook **：EML、EMLX、MSG、MHT

            - title: "サポートされているデータソース"
              content: |
                *データベース
                * XML
                * OData
                * JSON
                * CSV
                *カスタム.NETオブジェクト
                *データの表としてのスプレッドシート
                *データのテーブルとしてのワードプロセッシングテーブル

        right:
          enable: true
          table:
            - title: "その他のフォーマット"
              content: |
                * ** OpenOfficeドキュメント形式**：ODT、OTT、ODS、ODP
                * **メール**：MHT、MHTML
                * ** Web **：HTML
                * ** Markdownドキュメントファイル**：MD
                * **その他**：TXT

            - title: "フォーマット間アセンブリのサポート"
              content: |
                *ワードプロセッシング**TO**ワードプロセッシング、HTML、PDF、XPS、TIFF、MHTML、Markdown、TXT、XAML、OpenXPS、EPUB、SVG、PS、PCL
                *スプレッドシート**TO**スプレッドシート、HTML、PDF、XPS、TIFF、MHTML
                *プレゼンテーション**TO**プレゼンテーション、HTML、PDF、XPS、TIFF
                *メール**TO**ワードプロセッシング、メール、HTML、PDF、XPS、TIFF、MHTML、マークダウン、TXT、XAML、OpenXPS、EPUB、SVG、PS、PCL
                * HTML＆TXT ** TO **ワードプロセッシング、HTML、PDF、XPS、TIFF、MHTML、Markdown、TXT、XAML、OpenXPS、EPUB、SVG、PS、PCL

      tab_three:
        description: |
          GroupDocs.Assembly for .NETは、次のオペレーティングシステム、フレームワーク、およびパッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *Windowsデスクトップ
                * WindowsServer
                * Windows Azure
                * Linux

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * .NETFramework2.0以降
                * MonoFramework1.2以降

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "パッケージマネージャー"
              content: |
                * NuGet

            - icon: "fas fa-tools"
              title: "開発環境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

features:
    enable: true
    title: "GroupDocs.Assemblyfor.NET機能"

    feature:
      - icon: "fas fa-copy"
        content: "複数のデータ形式で動作します"

      - icon: "fas fa-eye"
        content: "数式とシーケンシャルデータ操作を使用してデータを操作できる"

      - icon: "fas fa-bolt"
        content: "テンプレート構文の文字列をUpper、Lower、Capital、FirstCapにフォーマットします"
      
      - icon: "fas fa-file-powerpoint"
        content: "テンプレート構文で序数、基数、アルファベットの数値フォーマットを実行する"

      - icon: "fas fa-code"
        content: "テンプレートドキュメントで変数を定義し、テンプレート構文タグ内でテキストコメントをサポートする"

      - icon: "fas fa-cloud"
        content: "外部ドキュメントのコンテンツをレポートに動的に挿入する"

      - icon: "fas fa-remove-format"
        content: "レポートでバーコード画像を動的に生成し、HTMLドキュメントの背景色を設定します"

      - icon: "fas fa-comment-slash"
        content: "電子メールメッセージ本文に属性を動的に割り当て、レポートにハイパーリンクを挿入する"

      - icon: "fas fa-location-arrow"
        content: "電子メールメッセージの添付ファイルを動的に作成する"

      - icon: "fas fa-border-all"
        content: "MicrosoftWordNEXTフィールドのアナログのサポート"

      - icon: "fas fa-wrench"
        content: "ワードプロセッシングドキュメントのアセンブル中にフィールドを更新する"

      - icon: "fas fa-columns"
        content: "スプレッドシートドキュメントを組み立てながら数式を計算する"

      - icon: "fas fa-file-word"
        content: "テンプレートの数値、テキスト、画像、チャート、日時要素をフォーマットします"

      - icon: "fas fa-envelope"
        content: "組み立てられたPOTおよびOTPプレゼンテーションドキュメント形式のロードと保存"

      - icon: "fas fa-print"
        content: "テンプレートにLINQベースの構文を使用し、テンプレート要素の条件付きテキストフォーマットを実行する"

      - icon: "fas fa-file-archive"
        content: "ファイル拡張子または明示的な仕様を使用して、アセンブルされたドキュメントのファイル形式を変更する"

      - icon: "fas fa-lock"
        content: "マークダウンでサポートされている順序付きリスト-新しく組み立てられた電子メールとWord文書をマークダウンに保存"

      - icon: "fas fa-file-code"
        content: "チャート、リスト、表、画像など、さまざまなタイプのレポートをサポートします"
      
      - icon: "fas fa-fill-drip"
        content: "例外スローではなく、生成されたドキュメントのインラインテンプレート構文エラー"

      - icon: "fas fa-file-excel"
        content: "リソースを使用してHTMLからテンプレートドキュメントをロードし、アセンブルされたWord、Excel、PowerPoint、および電子メールをリソースを使用してHTMLに保存します"

      - icon: "fas fa-heading"
        content: "再起動リストの番号付けをWord文書形式で動的に追加し、HTMLおよびRTF本文を使用して電子メールを送信"

      - icon: "fas fa-project-diagram"
        content: "Base64でエンコードされたバイトから画像とドキュメントを動的に挿入し、Wordドキュメントのチェックボックス値の設定を調整します"

      - icon: "fas fa-cube"
        content: "画像の比率を維持しながら、Word、Excel、プレゼンテーション、電子メールのテキストボックスで画像を拡大"

      - icon: "fab fa-uncharted"
        content: "リンクとブックマークをドキュメント形式に動的に追加し、Excelスプレッドシートのセル範囲に名前を付けます"

    more_feature:
      - title: "テンプレート要素のサポート"
        content: |
          GroupDocs.Assembly for .NET APIを使用すると、多数のテンプレート要素を操作するための制御が可能になります。フォーマットされたテキストブロック、HTMLブロック、画像、チャート、ハイパーリンク、およびバーコード（バーコードフォントを使用）を操作できます。リスト項目やテーブル行など、繰り返しブロックと条件付きブロックもサポートされています。スプレッドシート、プレゼンテーション、ドキュメント、および電子メールのテンプレート式に基づいて、同じテキストを含むテーブルセルをHTMLおよびRTF本文で動的にマージすることもできます。

      - title: "リストレポートの操作"
        content: |
          GroupDocs.Assembly for .NET APIを使用すると、次の3つのタイプのリストレポートを操作できます。  

          *箇条書き
          *番号付きリスト
          *色付きの番号付きリスト

      - title: "チャートレポートの操作"
        content: |
          GroupDocs.Assembly for .NETは、次のタイプのグラフレポートをサポートしています。  

          *データの3つの次元を表示するバブルチャート
          *縦棒グラフ
          * 円グラフ
          *散布図
          *シリーズチャート（カラー）

      - title: "テーブルレポートの操作"
        content: |
          GroupDocs.Assembly for .NETは、次のタイプのテーブルレポートをサポートします。  

          *マスター-詳細テーブル
          *強調表示された行のあるテーブル
          *代替コンテンツを含むテーブル
          *フィルタリング、グループ化、および順序付けを含むテーブル  
          
          テーブル行でデータバンドを使用することもできます。

      - title: "簡単な統合"
        content: |
          ほんの数行のコードを使用して、GroupDocs.Assembly for.NETAPIを.NETアプリケーションと簡単に統合できます。以下は、オープンドキュメント形式でレポートを生成するためのサンプルコードです。

          ```cs
          //DocumentAssemblerクラスをインスタンス化します
          DocumentAssembler assembler = new DocumentAssembler();
          //AssembleDocumentを呼び出してレポートを生成します
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
          //（https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NETでDataLayer.GetCustomerData（）メソッドの詳細を参照してください）
          ```

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Assemblyは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Assembly for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

back_to_top:
  enable: true
---
