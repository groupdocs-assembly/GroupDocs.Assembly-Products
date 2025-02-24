



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: id
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buat tabel dalam dokumen DOCX dengan C#"
head_description: "API GroupDocs.Assembly for .NET memungkinkan pengembang untuk menambahkan dan mengisi tabel dalam dokumen dan email dengan data dari sumber dinamis."

############################# Header ############################
title: "Hasilkan tabel data dalam dokumen DOCX menggunakan API .NET kami" 
description: "GroupDocs.Assembly for .NET memungkinkan pengisian tabel dalam dokumen DOCX secara dinamis dengan data dari berbagai sumber."
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
       [GroupDocs.Assembly for .NET](/assembly/net/) dirancang untuk membuat dokumen dan laporan dengan mengisi template menggunakan data dari berbagai sumber. Masukkan data terstruktur ke dalam tabel, daftar, dan grafik dengan mudah, atau sematkan gambar secara dinamis. Sintaks canggih memastikan penempatan data yang akurat. Mendukung lebih dari 50 format, termasuk PDF, dokumen MS Office, dan file email.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mengisi tabel dalam dokumen DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) memungkinkan Anda mengisi tabel dalam template untuk format seperti DOCX. Masukkan data dari berbagai sumber ke dalam tabel Anda.
      
      1. Buat template DOCX dengan placeholder tabel.
      2. Ambil data dari sumber yang didukung.
      3. Filter data untuk menyertakan hanya informasi yang diperlukan.
      4. Simpan dokumen dengan tabel yang terisi.
   
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
        // Tambahkan tag ini ke dalam baris tabel template
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Tetapkan jalur file untuk template
        string template = "table_template.docx";

        // Ambil data dari sumber yang didukung
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Simpan dokumen dengan tabel yang terisi data.
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Hasilkan dokumen dengan tabel dinamis"
  description: "GroupDocs.Assembly for .NET mempercepat pembuatan dokumen dengan mengotomatiskan pengisian tabel dan mendukung elemen tambahan seperti grafik, daftar, dan gambar melalui template dan markup canggih."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Buat laporan dari data terstruktur"
      content: "API ini memproses data dari sumber seperti JSON, XML, dan CSV untuk mengisi tabel dalam dokumen kantor secara efisien dan akurat."

    # feature loop
    - title: "Tampilkan data secara visual"
      content: "GroupDocs.Assembly memungkinkan pembuatan tabel, daftar, dan grafik, bersama dengan penambahan teks, tautan, dan gambar untuk desain dokumen yang profesional."

    # feature loop
    - title: "Posisikan data tabel dengan tepat"
      content: "Gunakan sintaks berbasis LINQ untuk menambahkan baris dan kolom tabel secara dinamis. Kustomisasi gaya, termasuk warna dan format, secara programatik."

    # feature loop
    - title: "Mendukung berbagai format"
      content: "Tangani format file populer seperti MS Office, OpenOffice, PDF, dan HTML dengan mudah. Sisipkan tabel yang telah diisi ke dalam jenis dokumen yang didukung tanpa kesalahan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara mengisi tabel data secara dinamis"
      content: |
        Contoh ini menunjukkan cara mengisi tabel dalam dokumen DOCX menggunakan data dinamis.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Siapkan template dengan placeholder untuk tabel
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Tentukan jalur file ke template
          string template = "table_template.docx";

          // Ambil data dari sumber pilihan Anda
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Buat objek sumber data dengan data yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Inisialisasi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan dokumen lengkap dengan tabel yang terisi.
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    exclude: "table"
    description: "Solusi kami menyederhanakan pembuatan dokumen profesional dengan tabel yang terisi secara dinamis dan elemen tambahan."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buat laporan dengan tabel terperinci"
    exclude: "DOCX"
    description: ".NET memungkinkan pembuatan laporan yang komprehensif dengan mengisi template menggunakan tabel dan elemen data lainnya dalam lebih dari 50 format yang didukung."
    items: 
          
        # format loop 1
        - name: "Tambahkan tabel ke PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan tabel ke DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan tabel ke PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Tambahkan tabel ke XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---