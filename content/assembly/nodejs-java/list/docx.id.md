



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: id
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Buat Daftar Dinamis dalam DOCX dengan JavaScript"
head_description: "Desain dan masukkan daftar ke dalam template DOCX menggunakan API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Sisipkan Daftar Berbasis Data ke dalam Berkas DOCX dengan Node.js" 
description: "GroupDocs.Assembly for Node.js via Java menawarkan alat yang kuat untuk menambahkan daftar fleksibel yang didorong oleh data ke dalam dokumen DOCX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai Gratis"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) menyederhanakan pembuatan dokumen dengan menarik data dari berbagai sumber dan menyematkannya ke dalam template. Gunakan untuk membangun daftar, tabel, grafik, dan elemen lainnya, dengan opsi penempatan dan format yang tepat. Mendukung lebih dari 50 format, termasuk PDF, MS Office, dan email, ini membantu mengotomatiskan proses pembuatan dokumen Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah untuk Menyisipkan Daftar ke dalam Berkas DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) memudahkan penambahan daftar rinci yang didorong oleh data ke dalam template DOCX Anda.
      
      1. Buat template DOCX dan tentukan placeholder untuk daftar.
      2. Sediakan jalur file untuk template.
      3. Muat data dari sumber yang didukung seperti JSON atau XML.
      4. Simpan dokumen dengan daftar yang dihasilkan.
   
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
        // Tempatkan tag ini dalam template Anda untuk menandai di mana daftar akan ditempatkan
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan jalur file untuk template Anda
        const template = "list_template.docx";

        // Ambil data dari sumber yang ingin Anda gunakan
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Simpan file dengan daftar yang disematkan
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Hasilkan Dokumen dengan Data yang Terintegrasi"
  description: "Dengan GroupDocs.Assembly for Node.js via Java, Anda dapat menyematkan daftar, tabel, grafik, dan elemen lainnya ke dalam template, menghemat waktu dan usaha."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Sorotan dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Hasilkan Laporan dari Berbagai Sumber Data"
      content: "Impor data dari JSON, XML, CSV, atau format lain untuk mengisi daftar dan komponen lainnya dengan efisien."

    # feature loop
    - title: "Tambahkan Daftar dan Elemen Visual Lainnya"
      content: "GroupDocs.Assembly memungkinkan Anda untuk menyisipkan daftar, tabel, grafik, dan lainnya dengan lancar di samping teks, gambar, dan tautan untuk hasil yang rapi."

    # feature loop
    - title: "Tepat Menempatkan dan Mengatur Gaya Data"
      content: "Template berbasis LINQ memungkinkan Anda mengontrol dengan tepat di mana daftar dan data lainnya muncul, menggunakan loop untuk item yang berulang, dan menyesuaikan gaya agar sesuai dengan kebutuhan Anda."

    # feature loop
    - title: "Bekerja di Berbagai Format"
      content: "Buat dokumen dalam format seperti MS Office, PDF, OpenOffice, HTML, dan email. Gabungkan konten dari berbagai sumber ke dalam satu file."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Buat Daftar Secara Programatis dalam Dokumen"
      content: |
        Contoh ini menunjukkan cara menambahkan daftar secara dinamis ke dalam dokumen DOCX menggunakan GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Tambahkan placeholder dalam template Anda untuk daftar
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Tentukan jalur file template
          const template = "numlist_template.docx";

          // Muat data untuk mengisi daftar
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Siapkan sumber data dengan detail yang diperlukan
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Inisialisasi DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Simpan dokumen akhir dengan daftar yang disertakan
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "Jelajahi Fitur GroupDocs.Assembly"
    exclude: "list"
    description: "Desain dan hasilkan dokumen kaya data dengan tanpa usaha menggunakan alat integrasi yang kuat."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buat Dokumen dalam Berbagai Format"
    exclude: "DOCX"
    description: "Node.js via Java mendukung lebih dari 50 format file, memudahkan penggabungan template dan data menjadi hasil yang profesional."
    items: 
          
        # format loop 1
        - name: "Buat daftar dalam PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Buat daftar dalam DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Buat daftar dalam PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Buat daftar dalam XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---