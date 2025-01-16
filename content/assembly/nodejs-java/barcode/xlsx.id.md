



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:03:58
draft: false
lang: id
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tambahkan Barcode ke Berkas XLSX Menggunakan JavaScript"
head_description: "Hasilkan dan sematkan barcode dalam dokumen dan email Anda dengan API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Buat Barcode untuk Berkas XLSX Menggunakan Node.js" 
description: "Dengan GroupDocs.Assembly for Node.js via Java, Anda dapat secara dinamis menghasilkan, menyesuaikan, dan menyematkan barcode ke dalam dokumen XLSX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai Sekarang"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Pendahuluan ke GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) memungkinkan Anda untuk membuat dokumen profesional dengan menggabungkan data dari berbagai sumber. Tambahkan grafik, tabel, daftar, gambar, dan barcode ke berkas Anda dengan baik. Gunakan template untuk mengatur konten tepat di tempatnya. Bekerja dengan lebih dari 50 format, termasuk PDF, dokumen Office, dan email.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk Menambahkan Barcode dalam Berkas XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) memudahkan untuk menyematkan barcode dalam dokumen XLSX. Ini mendukung lebih dari 60 tipe barcode, termasuk format 1D dan 2D.
      
      1. Buat template XLSX dengan placeholder untuk barcode.
      2. Ambil data dari sumber yang kompatibel.
      3. Atur opsi barcode seperti ukuran dan resolusi.
      4. Simpan dokumen akhir dengan barcode yang disematkan.
   
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
        // Gunakan tag ini dalam template untuk menyertakan barcode dalam dokumen keluaran.
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan jalur ke berkas template.
        const template = "barcode_template.xlsx";

        // Muat data yang diperlukan dari sumber Anda.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Simpan dokumen dengan barcode yang diterapkan.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Hasilkan Dokumen dengan Template Berbasis Data"
  description: "Dengan GroupDocs.Assembly for Node.js via Java, Anda dapat membuat berkas profesional dalam format populer dengan menyematkan grafik, tabel, daftar, tautan, gambar, dan barcode secara mulus."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Fitur Inti dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Buat Laporan dengan Data Bisnis"
      content: "Gunakan API untuk mengisi template dengan data dari format seperti JSON, XML, dan CSV dengan cepat dan akurat."

    # feature loop
    - title: "Tambahkan Elemen Visual"
      content: "GroupDocs.Assembly mendukung penyisipan elemen seperti grafik, tabel, daftar, teks, tautan, gambar, dan barcode secara real time."

    # feature loop
    - title: "Kontrol Penempatan Data"
      content: "Dengan template berbasis LINQ, Anda dapat secara tepat memposisikan data, mengulang melalui array, dan menerapkan format kustom secara programatik."

    # feature loop
    - title: "Kompatibel dengan Banyak Format"
      content: "Bekerja dengan berkas seperti dokumen MS Office, PDF, HTML, berkas OpenOffice, dan email. Gabungkan beberapa dokumen saat diperlukan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Contoh: Hasilkan Barcode Secara Programatik"
      content: |
        Contoh ini menunjukkan cara menghasilkan dan menyisipkan barcode ke dalam dokumen XLSX secara programatik.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Rancang template dengan placeholder barcode.
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Tentukan jalur berkas template.
          const template = "barcode_template.xlsx";

          // Ambil data dari sumber Anda.
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Buat objek sumber data dengan detail yang diperlukan.
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Inisialisasi sebuah instance DocumentAssembler.
          const asm = new assemblyLib.DocumentAssembler();

          // Atur konfigurasi barcode.
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Simpan dokumen dengan barcode yang disertakan.
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: "Jelajahi Fitur Utama"
    exclude: "barcode"
    description: "Sederhanakan pemrosesan dokumen dengan alat canggih dan kemampuan otomatisasi."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Format Berkas yang Didukung untuk Pembuatan Laporan"
    exclude: "XLSX"
    description: "Node.js via Java menangani lebih dari 50 tipe berkas, memudahkan penggabungan data dan pemrosesan template untuk hasil yang berkualitas tinggi."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---