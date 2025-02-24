



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: id
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Sisipkan Grafik ke dalam Berkas DOCX dengan JavaScript"
head_description: "Dengan GroupDocs.Assembly for Node.js via Java, pengembang dapat dengan cepat membuat dan menyisipkan grafik dinamis ke dalam dokumen menggunakan sumber data langsung."

############################# Header ############################
title: "Tambahkan Grafik ke Berkas DOCX Menggunakan Node.js" 
description: "GroupDocs.Assembly for Node.js via Java menyederhanakan proses integrasi grafik ke dalam dokumen DOCX dengan input data secara real-time."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai Gratis Hari Ini"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Gambaran Umum GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) adalah solusi yang kuat untuk membuat dokumen dan laporan otomatis. Tambahkan grafik, tabel, gambar, kode batang, dan daftar ke dalam berkas dengan presisi. Platform serbaguna ini mendukung lebih dari 50 format, termasuk PDF, dokumen Office, dan email.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-Langkah untuk Menambahkan Grafik ke Dokumen DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) memudahkan menambahkan grafik ke berkas DOCX. Pilih dari jenis grafik seperti grafik batang, garis, atau lingkaran.
      
      1. Desain template DOCX dengan placeholder untuk grafik.
      2. Muat data dari sumber yang didukung.
      3. Konfigurasi opsi grafik, termasuk jenis, warna, dan label.
      4. Ekspor dokumen dengan grafik yang disisipkan.
   
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
        // Sisipkan tag ini di template Anda untuk menghasilkan grafik.
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan jalur berkas template.
        const template = "chart_template.docx";

        // Ambil data dari sistem sumber Anda.
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Simpan dokumen akhir dengan grafik yang disisipkan.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Sisipkan Grafik dengan Mudah di Dokumen Anda"
  description: "GroupDocs.Assembly for Node.js via Java memudahkan pembuatan dokumen kaya fitur dalam jenis berkas populer. Gunakan template untuk menambahkan grafik, tabel, kode batang, daftar, gambar, dan lebih banyak lagi dengan pembaruan data secara real-time."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Ubah Data Menjadi Grafik Profesional"
      content: "Konversi data dari sumber seperti JSON, XML, atau CSV menjadi grafik berkualitas tinggi yang dapat disisipkan langsung ke dalam dokumen."

    # feature loop
    - title: "Buat Visual Menakjubkan"
      content: "Hasilkan grafik batang, grafik lingkaran, dan grafik garis yang bekerja tanpa masalah dengan elemen dokumen lain seperti gambar, tabel, dan kode batang."

    # feature loop
    - title: "Penataan dan Penempatan Grafik yang Fleksibel"
      content: "Gunakan template LINQ untuk mengontrol penempatan dan penataan grafik, termasuk warna, tata letak, dan label, untuk presentasi yang rapi."

    # feature loop
    - title: "Mendukung Banyak Format Berkas"
      content: "Hasilkan dokumen dalam format seperti MS Office, PDF, OpenOffice, dan HTML, dengan grafik yang terintegrasi sempurna untuk hasil yang profesional."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Hasilkan dan Sisipkan Grafik Secara Dinamis"
      content: |
        Contoh ini menggambarkan cara membuat dan menyisipkan grafik ke dalam berkas DOCX secara programatik.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Siapkan template dengan placeholder untuk grafik.
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Tentukan jalur ke berkas template.
          const template = "table_template.docx";

          // Ambil data dari sumber yang dipilih.
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Siapkan objek data berisi informasi grafik.
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Pilih jenis grafik dan sesuaikan tampilannya.
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Inisialisasi DocumentAssembler.
          const asm = new assemblyLib.DocumentAssembler();

          // Simpan dokumen yang diperbarui dengan grafik yang disisipkan.
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "Temukan Fitur Lanjutan"
    exclude: "chart"
    description: "Platform ini menyederhanakan pembuatan dokumen dengan alat yang dirancang untuk visualisasi data dan integrasi yang mulus."
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
    title: "Hasilkan Laporan dalam Berbagai Format Berkas"
    exclude: "DOCX"
    description: "Node.js via Java mendukung lebih dari 50 format, memudahkan penggabungan template dengan data untuk memproduksi dokumen yang terpolish."
    items: 
          
        # format loop 1
        - name: "Diagram dalam PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Diagram dalam DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Diagram dalam PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Diagram dalam XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---