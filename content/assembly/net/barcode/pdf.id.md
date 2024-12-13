



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:52
draft: false
lang: id
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Hasilkan barcode dalam dokumen PDF dengan C#"
head_description: "API GroupDocs.Assembly for .NET memungkinkan pengembang untuk secara dinamis menghasilkan dan menyematkan gambar barcode ke dalam dokumen dan email."

############################# Header ############################
title: "Tambahkan barcode ke dokumen PDF menggunakan API .NET kami" 
description: "GroupDocs.Assembly for .NET menawarkan dukungan penuh untuk pembuatan dan penyematan barcode secara dinamis dalam dokumen PDF."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Uji Coba Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Ikhtisar GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) dirancang untuk membantu Anda menghasilkan dokumen dan laporan dengan mengintegrasikan data dari berbagai sumber. Isi dokumen dengan teks atau data numerik, buat grafik, tabel, dan daftar, atau masukkan gambar dan barcode secara langsung. Gunakan markup yang canggih untuk menempatkan data dengan tepat di tempat yang diperlukan. Mendukung lebih dari 50 format, termasuk PDF, file MS Office, dan email.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menambahkan barcode yang dihasilkan ke dokumen PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) memudahkan penyisipan barcode ke dalam template dalam format seperti PDF. Mendukung lebih dari 60 jenis barcode, termasuk format satu dimensi dan dua dimensi.
      
      1. Buat template dengan tag spesifik untuk penempatan barcode (catatan: template PDF tidak kompatibel).
      2. Ambil data dari sumber data yang didukung.
      3. Konfigurasi properti tambahan seperti ukuran atau resolusi barcode.
      4. Simpan dokumen akhir dengan barcode yang disisipkan sebagai PDF.
   
    code:
      platform: "net"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Dokumen contoh"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Sisipkan tag ini ke dalam template Anda untuk menghasilkan barcode dalam dokumen akhir
        // <<barcode [barcode_expression] -barcode_type>>

        // Tentukan jalur file template
        // Dukungan untuk template PDF saat ini tidak tersedia.
        string template = "barcode_template.docx";

        // Ambil data dari sumber Anda
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Simpan dokumen dengan barcode yang dihasilkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Hasilkan dokumen dengan mengisi template dengan data"
  description: "GroupDocs.Assembly for .NET dirancang untuk menyederhanakan pembuatan dokumen dalam format populer. Tambahkan grafik, daftar, tabel, hyperlink, gambar, dan barcode menggunakan template dan markup yang canggih."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Fitur GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Buat laporan dari data bisnis"
      content: "API kami secara efisien mengisi dokumen dalam format kantor yang populer menggunakan data dari sumber seperti JSON, XML, dan CSV."

    # feature loop
    - title: "Gunakan elemen visual untuk menampilkan data"
      content: "GroupDocs.Assembly mendukung penyematan elemen asli seperti daftar, tabel, dan grafik, bersama dengan teks, hyperlink, gambar, dan barcode yang dihasilkan secara dinamis."

    # feature loop
    - title: "Masukkan data di mana saja dalam dokumen"
      content: "Gunakan sintaks berbasis LINQ untuk menempatkan data tepat di tempat yang dibutuhkan. Array dapat disisipkan menggunakan loop for-each, dan format (contoh: warna) dapat disesuaikan secara programatik."

    # feature loop
    - title: "Mendukung berbagai format"
      content: "Proses format file populer seperti MS Office, OpenOffice, PDF, HTML, dan berbagai format email. Sematkan satu dokumen ke dalam dokumen lain sesuai kebutuhan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menghasilkan barcode secara dinamis"
      content: |
        Contoh ini menunjukkan cara menyematkan barcode yang dihasilkan secara dinamis ke dalam dokumen PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Gunakan template ini untuk menyisipkan barcode ke dalam dokumen
          // <<barcode [barcode_expression] -barcode_type>>

          // Tentukan jalur ke file template
          // Dukungan untuk template PDF saat ini tidak tersedia.
          string template = "barcode_template.docx";

          // Ambil data dari sumber yang Anda pilih
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Buat objek sumber data dengan hanya data yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Inisialisasi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Atur properti barcode tambahan
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // Simpan dokumen akhir dengan barcode yang disematkan
          asm.AssembleDocument(template, "result.pdf", data);
          ```
        platform: "net"
        copy_title: "Salin"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "Unduh hasilnya"
            icon: "download"
            link: "/examples/assembly/formats/assembly_barcode.pdf"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Jelajahi fitur GroupDocs.Assembly secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduh dari Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Pelajari tentang lisensi"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Jelajahi fitur utama"
    exclude: "barcode"
    description: "Solusi kami dirancang untuk mempercepat proses dokumen bisnis Anda."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buat laporan dalam format populer"
    exclude: "PDF"
    description: ".NET mendukung pembuatan laporan dalam lebih dari 50 format, memungkinkan Anda untuk menggabungkan data dan template dengan lancar untuk hasil yang luar biasa."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---