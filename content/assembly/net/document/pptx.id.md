



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: id
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Sisipkan satu dokumen ke dalam dokumen lain dalam PPTX menggunakan API C#"
head_description: "Gabungkan dokumen PPTX dengan menggunakan C#. Dengan GroupDocs.Assembly, gabungkan file tanpa kendala dalam beberapa langkah saja."

############################# Header ############################
title: "Gabungkan dokumen dalam format PPTX" 
description: "Dengan GroupDocs.Assembly for .NET, Anda dapat dengan cepat menyisipkan satu dokumen PPTX ke dalam dokumen lainnya. API ini menyediakan alat yang kuat untuk penggabungan dokumen yang tepat."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) adalah alat yang kuat untuk komposisi dan manipulasi dokumen. Ini memungkinkan pengguna untuk menyisipkan satu dokumen ke dalam dokumen lainnya, memungkinkan penggabungan konten yang mulus. Dengan dukungan untuk lebih dari 50 format—termasuk PDF, file MS Office, dan lainnya—Anda dapat mengatur, mengedit, dan menyesuaikan hasil akhir sesuai kebutuhan Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menggabungkan dokumen ke dalam file PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) memungkinkan Anda menyisipkan satu dokumen ke dalam file PPTX lain tanpa kesulitan. Gabungkan dan sesuaikan konten dengan tepat.
      
      1. Rancang template PPTX dengan placeholder untuk dokumen yang disisipkan.
      2. Tentukan jalur file untuk template.
      3. Tentukan jalur file dokumen yang akan disisipkan.
      4. Simpan file akhir dengan konten yang disisipkan.
   
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
        // Tambahkan tag ini ke template Anda untuk menandai titik penyisipan
        // <<doc [doc_expression]>>

        // Tentukan jalur file untuk template
        string template = "doc_template.pptx";

        // Sediakan jalur dokumen yang akan disisipkan
        DataSourceInfo data 
            = new DataSourceInfo("insert.pptx", "doc_expression");

        // Simpan dokumen yang digabungkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Permudah penggabungan dokumen dengan alat canggih"
  description: "Koleksi GroupDocs.Assembly for .NET menyederhanakan penyisipan satu dokumen ke dalam dokumen lain, mendukung berbagai format file dan menawarkan kustomisasi untuk integrasi yang mulus."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Hasilkan laporan dari data bisnis Anda"
      content: "Secara otomatis populasi dokumen dengan data dari JSON, XML, CSV, atau sumber lain, memastikan alur kerja yang akurat dan efektif."

    # feature loop
    - title: "Perkaya dokumen dengan elemen visual"
      content: "GroupDocs.Assembly memungkinkan Anda untuk menyertakan tabel, grafik, dan daftar, serta teks, tautan, gambar, dan kode batang yang dihasilkan secara dinamis."

    # feature loop
    - title: "Tempatkan dan format data dengan tepat"
      content: "Template berbasis LINQ memberi Anda kontrol atas penempatan data, memungkinkan Anda menangani loop untuk array, dan memungkinkan gaya seperti kustomisasi warna."

    # feature loop
    - title: "Bekerja dengan berbagai format file"
      content: "Dengan mudah sisipkan dokumen satu sama lain di berbagai format seperti MS Office, PDF, HTML, OpenOffice, dan lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menyisipkan gambar ke dalam dokumen secara programatis"
      content: |
        Contoh ini menunjukkan bagaimana cara menyisipkan gambar ke dalam dokumen PPTX menggunakan GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tambahkan tag placeholder di template Anda
          // <<image [expression]>>

          // Tentukan jalur file untuk template
          string template = "template.pptx";

          // Atur jalur ke file gambar
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inisialisasi instansi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan dokumen dengan gambar yang disisipkan
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Temukan alat kami yang kuat"
    exclude: "document"
    description: "Jelajahi fitur yang ditawarkan GroupDocs.Assembly untuk menyisipkan dan menggabungkan dokumen dengan akurasi."
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
    title: "Gabungkan dokumen dalam berbagai format"
    exclude: "PPTX"
    description: "Dengan API .NET, Anda dapat menggabungkan dokumen di lebih dari 50 format yang didukung. Dengan efisien sisipkan file atau bagian ke dalam dokumen akhir Anda."
    items: 
          
        # format loop 1
        - name: "Sisipkan dokumen dalam PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Sisipkan dokumen dalam DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Sisipkan dokumen dalam PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Sisipkan dokumen dalam XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---