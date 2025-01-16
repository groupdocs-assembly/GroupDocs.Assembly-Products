



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:04
draft: false
lang: id
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Sisipkan Tabel ke Dalam Dokumen PPTX dengan JavaScript"
head_description: "Gunakan GroupDocs.Assembly for Node.js via Java untuk dengan cepat menyisipkan tabel dalam dokumen atau email, menarik data dari berbagai sumber."

############################# Header ############################
title: "Tambah Tabel ke Berkas PPTX dengan Mudah Menggunakan Node.js" 
description: "Dengan GroupDocs.Assembly for Node.js via Java, mengisi tabel dalam dokumen PPTX menjadi lebih sederhana, menggunakan data dari berbagai sumber."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai Uji Coba Gratis Anda"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Pendahuluan ke GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) adalah alat yang kuat untuk mengotomasi pembuatan dokumen. Alat ini memungkinkan Anda untuk menyisipkan tabel, grafik, daftar, dan gambar ke dalam templat, dengan penempatan konten yang tepat. Mendukung lebih dari 50 format file, termasuk PDF, Word, dan email, alat ini mempermudah pembuatan laporan dan tugas lainnya.

############################# Steps ############################
steps:
    enable: true
    title: "Cara Menambahkan Data ke Tabel di PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) memungkinkan Anda untuk dengan cepat mengisi templat tabel untuk file PPTX menggunakan sumber data dinamis.
      
      1. Buat templat PPTX dengan placeholder untuk baris dan kolom tabel.
      2. Muat data dari sumber yang didukung seperti JSON atau CSV.
      3. Atur dan format data sesuai kebutuhan.
      4. Hasilkan dokumen dengan tabel yang telah diisi.
   
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
        // Sertakan tag ini di placeholder baris tabel dari templat Anda
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan jalur file templat
        const template = "table_template.pptx";

        // Muat data Anda dari sumber yang dipilih
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Simpan dokumen akhir dengan tabel yang diisi
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Tambahkan Tabel Berbasis Data ke Dokumen"
  description: "GroupDocs.Assembly for Node.js via Java memungkinkan pengguna untuk secara otomatis membuat tabel, dan juga menyisipkan grafik, gambar, dan daftar menggunakan alur kerja berbasis templat."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Hasilkan Tabel dari Data Terstruktur"
      content: "Ambil data dari JSON, XML, CSV, dan format lainnya untuk secara otomatis mengisi tabel dokumen."

    # feature loop
    - title: "Buat Konten Visual yang Menarik"
      content: "Gunakan GroupDocs.Assembly untuk merancang tabel, grafik, dan daftar yang profesional, serta menambahkan tautan, gambar, dan teks untuk tampilan dokumen yang lebih halus."

    # feature loop
    - title: "Penempatan Konten Tabel Dinamis"
      content: "Tambah baris dan kolom secara programatis menggunakan templat berbasis LINQ, dan sesuaikan gaya seperti font, warna, dan penempatan."

    # feature loop
    - title: "Bekerja Tanpa Hambatan di Berbagai Format"
      content: "Dengan mudah buat atau edit tabel di MS Office, OpenOffice, PDF, HTML, dan format lainnya, menggabungkannya ke dalam file sesuai kebutuhan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara Mengisi Tabel Secara Programatis"
      content: |
        Contoh ini menunjukkan cara mengisi tabel dalam dokumen PPTX dengan data dari sumber eksternal.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Rancang templat dengan placeholder untuk tabel
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Tentukan jalur file ke templat
          const template = "table_template.pptx";

          // Muat data yang diperlukan dari sumber Anda
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Atur data ke dalam struktur yang diperlukan
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Inisialisasi DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Simpan dokumen keluaran dengan tabel yang telah diisi
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "Fitur Inti dalam Genggaman"
    exclude: "table"
    description: "API kami mengotomasi pembuatan tabel dan meningkatkan pembuatan dokumen dengan alat dan templat yang serbaguna."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Hasilkan Tabel dalam Berbagai Format"
    exclude: "PPTX"
    description: "Dengan Node.js via Java, isi templat dan buat tabel komprehensif di lebih dari 50 jenis file yang didukung."
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