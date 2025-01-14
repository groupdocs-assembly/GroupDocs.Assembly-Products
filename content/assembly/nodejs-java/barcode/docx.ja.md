



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:12
draft: false
lang: ja
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: ""
head_description: ""

############################# Header ############################
title: "" 
description: ""
subtitle: "" 

header_actions:
  enable: true
  items:
    #  loop
    - title: ""
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: ""
    link: "/assembly/nodejs-java/"
    link_title: "詳細を見る"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {steps.content.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {steps.content.step_4}
   
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
        // {examples.comment_1}
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        const template = "barcode_template.docx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "{more_features.image_description}"
  features:
    # feature loop
    - title: "{more_features.feature_1.title}"
      content: "{more_features.feature_1.content}"

    # feature loop
    - title: "{more_features.feature_2.title}"
      content: "{more_features.feature_2.content}"

    # feature loop
    - title: "{more_features.feature_3.title}"
      content: "{more_features.feature_3.content}"

    # feature loop
    - title: "{more_features.feature_4.title}"
      content: "{more_features.feature_4.content}"
      
  code_samples_ext:
    # code sample ext loop
    - title: "{code_1.title}"
      content: |
        {code_1.content}
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // {code_1.comment_1}
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          const template = "barcode_template.docx";

          // {code_1.comment_3}
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // {code_1.comment_4}
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // {code_1.comment_5}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_6}
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // {code_1.comment_7}
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    title: ""
    exclude: "barcode"
    description: ""
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
    title: ""
    exclude: "DOCX"
    description: ""
    items: 
          
        # format loop 1
        - name: "PDFにバーコードを追加"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Adobeポータブルドキュメントフォーマット"
          
        # format loop 2
        - name: "DOCXにバーコードを追加"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Microsoft WordオープンXMLドキュメント"
          
        # format loop 3
        - name: "PPTXにバーコードを追加"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"
          
        # format loop 4
        - name: "XLSXにバーコードを追加"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"


          

---