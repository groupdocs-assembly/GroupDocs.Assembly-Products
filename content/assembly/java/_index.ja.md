---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

head_title: "Java Document Automation Assembly＆Dynamic Reports Generator API"
head_description: "ドキュメントの自動化、組み立て、レポート作成のためのJavaAPI。カスタムテンプレートからレポートを作成します。 DB、JSON、OData、およびXMLデータソースからPDF Word ExcelPPTXHTMLをアセンブルします."

title: "ドキュメントとレポートを自動化するJavaAPI"
description: "データを取得するためのドキュメント自動化アプリケーションを構築します。カスタマイズ可能なテンプレートに入れて、JavaAPIを介して動的レポートを生成します."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
        product: "GroupDocs.Assembly"
        platform: "Java"

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

            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java APIは、Javaでドキュメント自動化およびレポート作成アプリケーションを迅速に開発し、外部ソフトウェアをインストールせずにテンプレートからカスタムレポートを生成するのに役立ちます。レポート生成エンジンは、テンプレートドキュメントからデータをフェッチしてアセンブルし、定義された構文に従って指定された出力形式でレポートを生成します。テンプレート要素のフォーマットプロパティを動的に構成および挿入でき、データを取得するためのさまざまなデータソース（JSON、XML、OData、データベース、CSV、データテーブルとしてのスプレッドシート、データテーブルおよびデータベースとしてのワード処理テーブル）をサポートします。  

      ドキュメントアセンブリライブラリは複数のドキュメント形式を認識し、PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシート、PowerPointプレゼンテーション、テキストなど、サポートされているすべてのファイル形式でテンプレートを作成できます。 LINQベースのテンプレート構文をサポートし、ユーザーはテンプレート要素の書式設定プロパティを動的に構成および挿入することもできます。  

      GroupDocs.Assembly for Javaは、新規または既存のJavaアプリケーションと簡単に統合できます。すべてのJavaバージョンとの互換性が高く、Javaランタイムを実行できる一般的なオペレーティングシステム（Windows、Linux、MacOS）をサポートしています。
    tabs:
      enable: true     
      
      tab_one:
        description: |
          以下は、Java用のGroupDocs.Assemblyの概要です。

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
          Javaドキュメント生成APIでサポートされている[ドキュメントファイル形式]（https://docs.groupdocs.com/assembly/java/supported-document-formats/）を以下に示します。

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
          GroupDocs.Assembly for Javaは、次のオペレーティングシステム、フレームワーク、およびパッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *MicrosoftWindowsデスクトップ
                * Microsoft Windows Server
                * Linux
                * マックOS

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * Java 7（1.7）以降

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "開発環境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                *Eclipse
            - icon: "fas fa-tools"
              title: "ビルド自動化ツール"
              content: |
                * Maven

features:
    enable: true
    title: "GroupDocs.Assembly for Java Features"

    feature:
      - icon: "fas fa-copy"
        content: "画像の比率を維持しながら、Word、Excel、プレゼンテーション、電子メールのテキストボックスで画像を調整する"

      - icon: "fas fa-eye"
        content: "数式を使用してシーケンシャルデータ操作を実行する-スプレッドシートの組み立て中に数式を適用する"

      - icon: "fas fa-bolt"
        content: "テンプレート構文の文字列にUpper、Lower、Capital、FirstCapフォーマットを適用する"
      
      - icon: "fas fa-file-powerpoint"
        content: "テンプレート構文のサポート序数、基数、アルファベットの数値の性質のフォーマット"

      - icon: "fas fa-code"
        content: "テンプレート構文タグ内のカスタム変数とテキストコメントを使用してテンプレートドキュメントをサポートする"

      - icon: "fas fa-cloud"
        content: "レポートにドキュメントコンテンツを動的に挿入する"

      - icon: "fas fa-remove-format"
        content: "HTMLドキュメントの背景色を動的に構成し、レポートでバーコードを生成する"

      - icon: "fas fa-comment-slash"
        content: "レポートにハイパーリンクを動的に挿入し、電子メールメッセージ本文に属性を適用する"

      - icon: "fas fa-location-arrow"
        content: "ワープロ文書の組み立て中に電子メールの添付ファイルと更新フィールドを動的に添付する"

      - icon: "fas fa-border-all"
        content: "MicrosoftWordのNEXTフィールドアナログのサポート"

      - icon: "fas fa-wrench"
        content: "リンクとブックマークをドキュメント形式に動的に追加し、Excelスプレッドシートのセル範囲に名前を付けます"

      - icon: "fas fa-columns"
        content: "組み立てられたPOTおよびOTPプレゼンテーションドキュメント形式のロードと保存"

      - icon: "fas fa-file-word"
        content: "数値、テキスト、画像、日時、チャート要素のテンプレートフォーマット"

      - icon: "fas fa-envelope"
        content: "Base64でエンコードされたバイトから画像とドキュメントを動的に挿入します"

      - icon: "fas fa-print"
        content: "LINQベースのテンプレート構文"

      - icon: "fas fa-file-archive"
        content: "明示的な仕様またはファイル拡張子を使用して、アセンブルされたファイルの形式を変更する"

      - icon: "fas fa-lock"
        content: "マークダウンでサポートされている順序付きリスト-新しく組み立てられた電子メールとWord文書をマークダウンに保存"

      - icon: "fas fa-file-code"
        content: "チャート、画像、表、リストなど、さまざまなレポートタイプを生成します"
      
      - icon: "fas fa-fill-drip"
        content: "例外スローではなく、生成されたドキュメントのインラインテンプレート構文エラー"

      - icon: "fas fa-file-excel"
        content: "Word文書およびHTMLとRTF本文を含む電子メールの番号付きリストを動的に再起動します"

      - icon: "fas fa-heading"
        content: "組み立てられたマークダウンドキュメントのテーブル、自動リンク、インラインリンク、および画像のサポート"

      - icon: "fas fa-project-diagram"
        content: "バーコードを動的に生成する（GS1-128 AI 8102クーポン拡張およびUPCA＆GS1データバークーポン"

      - icon: "fas fa-cube"
        content: "リソースを使用してHTMLからテンプレートドキュメントをロードし、アセンブルされたWord、Excel、PowerPoint、および電子メールをリソースを使用してHTMLに保存します"

    more_feature:
      - title: "テンプレート要素を操作する"
        content: |
          GroupDocs.Assembly forJavaAPIを使用して多数のテンプレート要素を操作します。使用できるテンプレート要素には、テキストブロック、画像、ハイパーリンク、HTMLブロック、バーコード（バーコードフォント経由）、およびグラフが含まれます。リストアイテムとテーブル行に繰り返しブロックと条件付きブロックを適用することもできます。ドキュメント、プレゼンテーション、スプレッドシート、およびHTMLとRTF本文を含む電子メールのテンプレート式に基づいて、同じテキストを保持するテーブルセルを動的にマージします。
      
      - title: "リストレポートを操作する"
        content: |
          GroupDocs.Assembly for Java APIを使用して、次のタイプのリストレポートをサポートします。  

          *箇条書き
          *番号付きリスト
          *色付きの番号付きリスト

      - title: "チャートレポートの操作"
        content: |
          GroupDocs.Assembly for Javaは、次のタイプのチャートレポートをサポートしています。

          *データの3つの次元を表示するバブルチャート
          *縦棒グラフ
          * 円グラフ
          *散布図
          *シリーズチャート（カラー）

      - title: "テーブルレポートを操作する"
        content: |
          GroupDocs.Assembly for Javaは、次のタイプのテーブルレポートをサポートします。  

          *マスター-詳細テーブル
          *強調表示された行のあるテーブル
          *代替コンテンツを含むテーブル
          *フィルタリング、グループ化、および順序付けを含むテーブル  

          テーブル行でデータバンドを使用することもできます。

      - title: "チャートレポートの操作"
        content: |
          GroupDocs.Assembly for Java APIとJavaアプリケーションの統合は、とても簡単です。以下は、Javaを使用してOpenDocument形式でレポートを生成するコードのブロック例です。  

          ```java
          //DocumentAssemblerクラスをインスタンス化します
          DocumentAssembler assembler = new DocumentAssembler();
          //AssembleDocumentを呼び出してレポートを生成します
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          //（https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Javaで新しいDataStorage（）メソッドの詳細を参照してください）
          ```

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Assemblyは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

back_to_top:
  enable: true
---
