



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: id
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Menghasilkan daftar dalam dokumen PPTX dengan C#"
head_description: "API GroupDocs.Assembly for .NET memungkinkan pengembang untuk secara dinamis membuat dan menyisipkan daftar yang diisi data ke dalam dokumen dan templat."

############################# Header ############################
title: "Tambahkan daftar berbasis data ke dokumen PPTX menggunakan API .NET kami" 
description: "GroupDocs.Assembly for .NET menawarkan alat yang kuat untuk secara dinamis menghasilkan dan menyisipkan daftar dalam dokumen PPTX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Versi Percobaan Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Ikhtisar GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) dirancang untuk mempercepat pembuatan dokumen dan laporan dengan mengintegrasikan data dari berbagai sumber. Isi templat dengan daftar, grafik, tabel, barcode, atau teks, dan tempatkan konten secara tepat menggunakan tanda markup lanjutan. Dengan dukungan lebih dari 50 format—termasuk PDF, file MS Office, dan email—ini sangat ideal untuk mengotomatiskan alur kerja dokumen.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menambahkan daftar yang diisi data ke dokumen PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) memudahkan menyisipkan daftar berbasis data ke dalam templat PPTX. Buat dan sesuaikan daftar dengan lancar.
      
      1. Siapkan templat PPTX dengan placeholder untuk daftar.
      2. Atur jalur ke templat.
      3. Ambil data dari sumber yang didukung seperti JSON atau XML.
      4. Simpan dokumen akhir dengan daftar yang disisipkan.
   
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
        // Tambahkan tag ini ke templat Anda untuk menandai tempat di mana daftar akan muncul
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Tentukan jalur ke file templat
        string template = "list_template.pptx";

        // Ambil data dari sumber pilihan Anda
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Simpan dokumen dengan daftar yang dihasilkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Buat dokumen dengan mengisi templat menggunakan data terstruktur"
  description: "GroupDocs.Assembly for .NET menyederhanakan pembangunan dokumen berbasis data. Tambahkan daftar, tabel, barcode, grafik, gambar, dan elemen lainnya secara dinamis menggunakan templat lanjutan."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Fitur GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Hasilkan laporan dari data bisnis"
      content: "API ini mengisi dokumen dalam format populer menggunakan data dari sumber seperti JSON, XML, CSV, dll. dengan akurasi dan efisiensi."

    # feature loop
    - title: "Gunakan daftar dan elemen lainnya untuk menyajikan data"
      content: "GroupDocs.Assembly memungkinkan Anda untuk menyisipkan daftar, tabel, dan grafik bersamaan dengan teks, barcode, hyperlink, dan gambar untuk menciptakan dokumen yang terstruktur dengan baik."

    # feature loop
    - title: "Sisipkan data dengan tepat di tempat yang diinginkan"
      content: "Manfaatkan sintaksis berbasis LINQ untuk memposisikan daftar dan elemen data lainnya dengan presisi. Gunakan loop untuk mengisi daftar secara dinamis dan terapkan format khusus secara programatik."

    # feature loop
    - title: "Mendukung berbagai format dokumen"
      content: "Hasilkan dan kelola dokumen dalam berbagai format seperti MS Office, OpenOffice, PDF, HTML, dan file email. Mudah mengintegrasikan beberapa dokumen menjadi satu."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menghasilkan daftar secara dinamis"
      content: |
        Contoh ini menunjukkan cara menyematkan daftar yang dihasilkan secara dinamis ke dalam dokumen PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tambahkan tag placeholder ke templat Anda untuk daftar
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Tentukan jalur ke file templat
          string template = "numlist_template.pptx";

          // Ambil data untuk mengisi daftar
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Buat objek sumber data dengan informasi yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inisialisasi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan dokumen akhir dengan daftar yang dihasilkan
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "Jelajahi kemampuan kunci"
    exclude: "list"
    description: "Platform kami dibangun untuk menyederhanakan pembuatan dan integrasi konten dokumen berbasis data."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buat dokumen terstruktur dalam format populer"
    exclude: "PPTX"
    description: ".NET mendukung lebih dari 50 format, memungkinkan Anda untuk dengan mudah menggabungkan data dan templat untuk menghasilkan hasil yang rapi dan terstruktur."
    items: 
          
        # format loop 1
        - name: "Buat daftar dalam PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Buat daftar dalam DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Buat daftar dalam PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Buat daftar dalam XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---