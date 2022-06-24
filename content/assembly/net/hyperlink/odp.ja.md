---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/assembly/net/text/odp/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM EML EMLX MSG 

############################# Head ############################
head_title: "ODP ドキュメントにハイパーリンクを動的に挿入する.NETAPI"
head_description: "GroupDocs.Assembly .NET APIを使用すると、開発者は、PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、EML、MSGなどの電子メール、レポート、またはドキュメントへのハイパーリンクを動的に挿入できます。"

############################# Header ############################
title: ".NETAPIを介してODPドキュメントとレポートへのハイパーリンクを動的に挿入する"
description: "GroupDocs.Assembly .NET APIを使用すると、プログラマーは、レポート、電子メール、およびPDF DOC、DOCX、RTF、XLSX、CSV、PPT、PPTX、EML、HTML、MSGなどのOfficeドキュメントへのハイパーリンクを動的に挿入できます。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "レポート、電子メール、さまざまなドキュメントにハイパーリンクを動的に挿入するにはどうすればよいですか？"
    content: |
       このWebページでは、ユーザーが自分の.NETアプリケーション内に、レポート、電子メールメッセージ、およびさまざまな種類のドキュメントへのハイパーリンクを動的に挿入する方法について説明します。 ハイパーリンクはWorldWideWebのバックボーンであり、さまざまなページやドキュメントをリンクしたり、クリックして現在のドキュメント内の新しいセクションにジャンプしたりするために使用できます。 GroupDocs.Assembly .NETは非常に強力なAPIであり、ソフトウェア開発者が数行のコードでドキュメントまたはレポート内にハイパーリンクを動的に追加するのに役立ちます。 PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシート、PowerPointプレゼンテーションなど、非常に人気のあるドキュメントタイプのサポートが含まれています。 ドキュメントページへのリンクの挿入、セルへのリンクの挿入、ハイパーリンクの編集、ハイパーリンクの代わりにテキストを表示する、ブックマークからリンクを動的に挿入する、プレゼンテーションスライドにハイパーリンクを挿入するなど、いくつかの高度な機能をサポートしていました。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NETを介したワード処理ドキュメントへのハイパーリンクの挿入"
      content_left: |
       GroupDocs.Assembly .NET APIは、さまざまなタイプのドキュメント内にハイパーリンクを挿入および編集するための完全なサポートを提供します。 次のC＃.NETコード例は、Wordドキュメント内にハイパーリンクを簡単に追加する方法を示しています。 

      title_right: "Wordファイルにハイパーリンクを追加する方法"
      content_right: |
        * ソースドキュメントと宛先ドキュメントの設定
        * ウリ式を設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) メソッドを呼び出して、ドキュメントをアセンブルします。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "f4a8031406d44941d400088b718f7730"
      gistfile: "insert_hyperlinks_to_word_document.cs"

    - title_left: ".NETを介してスプレッドシートにハイパーリンクを動的に挿入する"
      content_left: |
       GroupDocs.Assembly .NET APIは、Spreadsheetファイル内のハイパーリンクの追加と処理を完全にサポートします。 その場所を簡単に編集したり、新しい場所に置き換えたりすることができます。 次のC＃コードは、ユーザーが自分の.NETアプリ内のスプレッドシートファイルにハイパーリンクを簡単に挿入できることを示しています。

      title_right: "スプレッドシートドキュメントにハイパーリンクを追加する"
      content_right: |
        * ソースドキュメントと宛先ドキュメントの設定
        * ウリ式を設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) メソッドを呼び出して、ドキュメントをアセンブルします。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "c2f9cd8bb06f9a7a2c444621ebf82696"
      gistfile: "insert_hyperlinks_in_spreadsheet_documents.cs"

    - title_left: ".NETAPIを介してPowerPointプレゼンテーションにハイパーリンクを追加する"
      content_left: |
       GroupDocs.Assembly for .NETは、ソフトウェアの専門家がさまざまな種類のドキュメントを管理するためのアプリケーションを構築するのに役立ちます。 次のコード例は、ソフトウェア開発者がPowerPointプレゼンテーションドキュメント内にハイパーリンクを追加する方法を示しています。 

      title_right: "プレゼンテーションにハイパーリンクを追加する方法"
      content_right: |
        * ソースと宛先のプレゼンテーションファイルの設定
        * Uriを設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) メソッドを呼び出して、ドキュメントをアセンブルします。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "49e1ca9eccc41942372c23c14f98ecef"
      gistfile: "insert_hyperlinks_in_presentation_documents.cs"

    - title_left: "電子メールにハイパーリンクを挿入するための.NETAPI"
      content_left: |
       GroupDocs.Assembly .NET APIを使用すると、ソフトウェアの専門家は電子メールドキュメント内にハイパーリンクを挿入できます。 次の.NETコードは、プログラマーが自分の電子メールメッセージにハイパーリンクを追加し、自分の.NETアプリ内から他のユーザーに送信する方法を示しています。 

      title_right: "電子メールドキュメントにハイパーリンクを追加する"
      content_right: |
        * ソースと宛先のスプレッドシートファイルの設定
        * Uriを設定し、テキスト式を表示します
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) クラスのインスタンスを作成します
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) メソッドを呼び出して、ドキュメントをアセンブルします。 それはサポートします
          * テンプレートドキュメントを読むためにストリーミングします。
          * 結果のドキュメントを書き込むためのストリーム。
          * ドキュメントの読み込みと保存のための追加オプション。
          * データソースオブジェクトに関する情報。

      gisthash: "8c119b4faa0334179854e164d87d3e7b"
      gistfile: "insert_hyperlinks_in_email_documents.cs"  

    - title_left: "システム要求"
      content_left: |
        GroupDocs.Assembly .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 完全なシステム要件ガイドについては、[システム要件](https://docs.groupdocs.com/assembly/net/system-requirements/) にアクセスしてください。以下のコードを実行する前に、次の前提条件がインストールされていることを確認してください。 システム：
         * オペレーティングシステム：Microsoft Windows、Linux、MacOS
         * 開発環境：Visual Studio、Xamarin、MonoDevelopなど
         * フレームワーク：.NETフレームワーク、.NET標準、.NETコア、モノラル
         * [NuGet](https://www.nuget.org/packages/GroupDocs.Assembly/) から最新バージョンのGroupDocs.Assembly.NETAPIを入手します。
        
      title_right: "GroupDocs.Assemblyを使用する理由"
      content_right: |
        * ユーザーがテンプレートからカスタムドキュメントを作成できるようにします。
        * ドキュメントの作成と自動化に追加のソフトウェアは必要ありません
        * データソースに基づいて出力ドキュメントを生成する機能
        * レポートにドキュメントコンテンツを動的に挿入する
        * 電子メールの添付ファイルを動的に添付し、レポートにハイパーリンクを挿入します
        * 空の段落の自動削除
        * 複数のデータ形式の完全サポート
        * 動的な電子メールの添付ファイルのサポート

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---