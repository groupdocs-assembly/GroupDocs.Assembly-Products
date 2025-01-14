



---
############################# Static ############################
layout: "format"
date:  2025-01-14T15:37:18
draft: false
lang: id
format: Pdf
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
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {texts_pdf.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {texts_pdf.step_4}
   
    code:
      platform: "java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Dokumen contoh"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // {examples.comment_1}
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // {examples.comment_2}
        // {texts_pdf.comment_tmp}
        const template = "table_template.docx";

        // {examples.comment_3}
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // {examples.comment_4}
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_table.webp" # 500x500 px
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
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // {code_1.comment_2}
          // {texts_pdf.comment_tmp}
          const template = "table_template.docx";

          // {code_1.comment_3}
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // {code_1.comment_4}
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // {code_1.comment_5}
          const asm = new assemblyLib.DocumentAssembler();

          // {code_1.comment_6}
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "Salin"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "Unduh hasilnya"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.pdf"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Jelajahi fitur GroupDocs.Assembly secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduh dari NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Pelajari tentang lisensi"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "table"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "PDF"
    description: ""
    items: 
          
        # format loop 1
        - name: "Tambahkan tabel ke PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan tabel ke DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan tabel ke PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Tambahkan tabel ke XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---