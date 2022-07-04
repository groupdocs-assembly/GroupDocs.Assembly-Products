---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/assembly/java/hyperlink/docm/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "JavaAPIを介してOfficeDOCM ドキュメントとレポートにハイパーリンクを追加する"
head_description: "GroupDocs.Assembl for Javaは、Javaアプリ内でのPDF DOCX、RTF、XLSX、PPTX、EML、MSGなどのオフィスおよび電子メールドキュメントへのハイパーリンクの動的挿入をサポートします。"

############################# Header ############################
title: "JavaAPIを介してOfficeドキュメントと電子メールにハイパーリンクを追加する"
description: "GroupDocs.Assembly Java APIを使用すると、ソフトウェアの専門家は、PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、MSGなどの電子メールメッセージやOfficeドキュメントにハイパーリンクをプログラムで追加できます。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java APIを使用してOfficeおよびEmailsドキュメントにハイパーリンクを追加する方法は？"
    content: |
       ハイパーリンクは、クリックして新しいドキュメントまたは現在のドキュメント内の新しいセクションにジャンプできる単語、フレーズ、または画像です。 ハイパーリンクはワールドワイドWebのバックボーンであり、WorldWideWebで必要な多くの機能に使用されます。 GroupDocs.Assembly for Javaは、ドキュメントの自動化およびレポート生成APIであり、ソフトウェア開発者がドキュメントまたはレポート内にハイパーリンクを動的に挿入するのに役立ちます。 APIは非常に安定しており、ドキュメントページへのハイパーリンクの追加、プレゼンテーションスライドへのリンクの追加、スプレッドシートセルへのハイパーリンクの追加、ハイパーリンクコンテンツの変更、ブックマークからのリンクの動的挿入、不要な削除など、ハイパーリンク管理に関連するいくつかの高度な機能を完全にサポートします。 リンク、ハイパーリンクの代わりにテキストを表示するなど。 PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシート、PowerPointプレゼンテーションなど、非常に一般的なドキュメントタイプの一部が完全にサポートされています。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Javaを介してWord処理ドキュメントへのハイパーリンクを挿入する"
      content_left: |
       GroupDocs.Assembly Java APIは、一般的に使用されるさまざまなドキュメント形式内でのハイパーリンクの挿入と編集を完全にサポートしています。 以下のJavaコード例は、MicrosoftWordドキュメント内にハイパーリンクを挿入する方法を示しています。

      title_right: "Java経由でDOCMドキュメントにハイパーリンクを挿入する"
      content_right: |
        * ソースドキュメントと宛先ドキュメントの設定
        * Uri式を設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) に電話してください ドキュメントをアセンブルするメソッド。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "Javaを介してスプレッドシートにハイパーリンクを追加する"
      content_left: |
       GroupDocs.Assembly Java APIを使用すると、コンピュータープログラマーは、Spreadsheetドキュメント内にハイパーリンクを簡単に挿入および変更できます。 彼らは簡単にアクセスしたり、その場所を編集したり、新しい場所に置き換えたりすることができます。 次のJavaコードは、プログラマーがスプレッドシート内にハイパーリンクを簡単に追加できることを示しています。

      title_right: "DOCMファイルへのハイパーリンクを挿入する方法"
      content_right: |
        * ソースと宛先のスプレッドシートファイルの設定
        * Uri式を設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) に電話してください ドキュメントをアセンブルするメソッド。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "Javaを介してPowerPointプレゼンテーションへのハイパーリンクを挿入する"
      content_left: |
       GroupDocs.Assembly Java APIを使用すると、プログラマーはドキュメント管理関連のタスクを簡単に処理できます。 これは、ソフトウェアプログラマーがPowerPointプレゼンテーションドキュメントに簡単にアクセスしてハイパーリンクを追加できることを示すJavaコードの例です。

      title_right: "プレゼンテーションにハイパーリンクを挿入する方法"
      content_right: |
        * ソースと宛先のプレゼンテーションファイルの設定
        * Uriを設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) に電話してください ドキュメントをアセンブルするメソッド。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "JavaAPIを使用して電子メールにハイパーリンクを追加する"
      content_left: |
       GroupDocs.Assembly for Javaを使用すると、ソフトウェア開発者は数行のJavaコードで電子メールメッセージにハイパーリンクを簡単に追加できます。 次の例は、開発者が自分の電子メールドキュメント内にハイパーリンクを挿入し、自分のJavaアプリ内で他のユーザーに送信する方法を示しています。

      title_right: "メールにハイパーリンクを追加する方法"
      content_right: |
        * ソースと宛先のスプレッドシートファイルの設定
        * Uriを設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) に電話してください ドキュメントをアセンブルするメソッド。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

    - title_left: "システム要求"
      content_left: |
        GroupDocs.Assembly Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 Microsoft Word、Excel、PowerPoint、Outlook、OpenOffice、その他50以上の形式でドキュメントを生成できます。 完全なシステム要件ガイドについては、[システム要件](https://docs.groupdocs.com/assembly/java/system-requirements/) にアクセスしてください。以下のコードを実行する前に、次の前提条件がインストールされていることを確認してください。 システム：
         * オペレーティングシステム：Microsoft Windows、Linux、MacOS
         * Javaバージョンのサポート：J2SE 7.0（1.7）、J2SE 8.0（1.8）以降
         * [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/) からGroupDocs.AssemblyJavaAPIの最新バージョンを入手してください
        
      title_right: "GroupDocs.Assemblyを使用する理由"
      content_right: |
        * テンプレートからカスタムドキュメントを作成します。
        * 電子メールの添付ファイルを動的に添付します。
        * ドキュメントを作成および自動化するために追加のソフトウェアは必要ありません。
        * データソースに基づいて出力ドキュメントを生成します。
        * レポートにドキュメントコンテンツを動的に挿入する
        * スプレッドシートの組み立て中に数式を適用します。
        * 複数のデータ形式のサポートを提供します
        * シーケンシャルデータ操作のサポート。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---