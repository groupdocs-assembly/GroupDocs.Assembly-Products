



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: id
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Gabungkan Dokumen dalam PPTX dengan JavaScript"
head_description: "Gabungkan file PPTX dengan menggunakan JavaScript. GroupDocs.Assembly menyederhanakan penggabungan dokumen hanya dalam beberapa langkah sederhana."

############################# Header ############################
title: "Gabungkan Konten dalam File PPTX dengan Mudah" 
description: "Dengan GroupDocs.Assembly for Node.js via Java, mengintegrasikan satu file PPTX ke dalam yang lain berlangsung cepat dan tepat. Nikmati alat yang fleksibel dan andal untuk penggabungan yang mulus."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba Gratis"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Gambaran Umum GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) menawarkan cara yang kuat untuk mengelola dokumen. Gabungkan satu file ke dalam yang lain sambil mendukung lebih dari 50 format, seperti PDF dan MS Office. Sesuaikan tata letak, edit konten, dan atur dokumen persis seperti yang Anda butuhkan.

############################# Steps ############################
steps:
    enable: true
    title: "Cara Menggabungkan Dokumen ke dalam File PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) memudahkan untuk menyisipkan satu file PPTX ke dalam yang lain dengan opsi yang dapat disesuaikan.
      
      1. Rancang template PPTX dengan placeholder untuk konten.
      2. Tentukan jalur file untuk template.
      3. Berikan jalur file untuk dokumen yang akan digabung.
      4. Ekspor file akhir dengan konten yang digabung.
   
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
        // Masukkan tag ini ke dalam template Anda untuk mendefinisikan tempat di mana dokumen akan disisipkan
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan jalur file untuk template utama
        const template = "doc_template.pptx";

        // Berikan jalur untuk dokumen yang ingin Anda gabungkan
        const data 
            = new assemblyLib.DataSourceInfo("insert.pptx", "doc_expression");

        // Simpan output akhir dengan dokumen yang disisipkan
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Alat Kuat untuk Integrasi Dokumen"
  description: "GroupDocs.Assembly for Node.js via Java memudahkan penyisipan file di berbagai format yang sepenuhnya dapat disesuaikan. Berikan hasil yang konsisten dan profesional setiap saat."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Buat Laporan dengan Data Bisnis"
      content: "Ambil data dari sumber JSON, XML, atau CSV untuk membuat laporan dan dokumen yang komprehensif dengan cepat dan akurat."

    # feature loop
    - title: "Tambahkan Elemen Visual yang Kaya"
      content: "GroupDocs.Assembly memungkinkan Anda untuk menyertakan tabel, grafik, daftar, gambar, dan kode batang di samping teks dan hyperlink."

    # feature loop
    - title: "Penempatan Data yang Presisi"
      content: "Gunakan template LINQ untuk menempatkan data tepat di tempatnya, tangani item yang berulang seperti array, dan sesuaikan gaya tanpa kesulitan."

    # feature loop
    - title: "Bekerja dengan Berbagai Format"
      content: "Gabungkan konten secara mulus di berbagai format seperti PDF, file MS Office, HTML, dan OpenOffice, menawarkan fleksibilitas untuk semua proyek."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sisipkan Gambar ke dalam Dokumen Secara Pemrograman"
      content: |
        Contoh ini menunjukkan cara menyisipkan gambar ke dalam file PPTX menggunakan GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Tambahkan placeholder dalam template untuk gambar
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Tentukan jalur ke file template
          const template = "template.pptx";

          // Atur jalur ke gambar yang ingin Anda sisipkan
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Inisialisasi objek DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Simpan dokumen dengan gambar yang disertakan
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Fitur Utama dalam Sekilas"
    exclude: "document"
    description: "Jelajahi alat komprehensif yang ditawarkan GroupDocs.Assembly untuk penggabungan dokumen yang efisien dan mulus."
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
    title: "Gabungkan Dokumen dalam Berbagai Format"
    exclude: "PPTX"
    description: "Gunakan Node.js via Java untuk menggabungkan konten di lebih dari 50 format file, memastikan hasil yang profesional dan rapi."
    items: 
          
        # format loop 1
        - name: "Sisipkan dokumen dalam PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Sisipkan dokumen dalam DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Sisipkan dokumen dalam PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Sisipkan dokumen dalam XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---