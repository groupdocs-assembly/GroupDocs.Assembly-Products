



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: id
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Sisipkan barcode dalam file PDF dengan Java"
head_description: "API GroupDocs.Assembly for Java memudahkan pembuatan dan penyisipan gambar barcode ke dalam dokumen dan email Anda secara real-time."

############################# Header ############################
title: "Hasilkan barcode untuk file PDF dengan API Java kami" 
description: "GroupDocs.Assembly for Java menyediakan alat yang komprehensif untuk membuat, menyesuaikan, dan menyisipkan barcode secara dinamis ke dalam file PDF."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Sekarang"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) membantu Anda menghasilkan dan menyesuaikan dokumen dengan menambahkan data dari berbagai sumber. Sisipkan teks, angka, grafik, tabel, daftar, gambar, dan barcode. Gunakan template canggih untuk memastikan data muncul persis di tempat yang Anda inginkan. Mendukung lebih dari 50 format, termasuk PDF, file Office, dan email.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menyisipkan barcode dalam dokumen PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) memungkinkan Anda menyisipkan barcode ke dalam format populer seperti template PDF. Mendukung lebih dari 60 jenis, termasuk barcode 1D dan 2D.
      
      1. Siapkan template dengan placeholder untuk barcode (template PDF tidak didukung).
      2. Ambil data dari sumber yang didukung.
      3. Sesuaikan pengaturan barcode seperti ukuran dan resolusi.
      4. Simpan dokumen dengan barcode yang ditambahkan sebagai file PDF.
   
    code:
      platform: "java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Dokumen contoh"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Gunakan tag ini dalam template Anda untuk membuat barcode dalam dokumen keluaran
        // <<barcode [barcode_expression] -barcode_type>>

        // Tentukan jalur file untuk template
        // Template PDF saat ini tidak didukung.
        String template = "barcode_template.docx";

        // Ambil data dari sumber Anda
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Simpan dokumen dengan barcode yang ditambahkan sebagai file PDF.
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Bangun dokumen menggunakan template yang didorong data"
  description: "GroupDocs.Assembly for Java menyederhanakan pembuatan dokumen di berbagai jenis file populer. Gunakan template untuk menambahkan grafik, tabel, daftar, tautan, gambar, dan barcode tanpa kesulitan."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Fitur GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Hasilkan laporan menggunakan data bisnis"
      content: "API ini mengisi dokumen dengan data dari format seperti JSON, XML, dan CSV dengan efisien dan akurat."

    # feature loop
    - title: "Visualisasikan data dengan elemen bawaan"
      content: "GroupDocs.Assembly mendukung elemen asli seperti tabel, grafik, dan daftar, serta teks, tautan, gambar, dan pembuatan barcode secara real-time."

    # feature loop
    - title: "Sisipkan data di tempat yang Anda butuhkan"
      content: "Dengan template berbasis LINQ, Anda dapat menempatkan data dengan tepat, menggunakan loop untuk menambahkan array, dan menyesuaikan format seperti warna secara programatikal."

    # feature loop
    - title: "Kompatibilitas luas dengan jenis file"
      content: "Kelola file seperti dokumen MS Office, PDF, HTML, OpenOffice, dan email. Anda juga dapat menggabungkan satu dokumen ke dokumen lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara membuat barcode secara dinamis"
      content: |
        Contoh ini menunjukkan bagaimana cara menghasilkan dan menambahkan barcode ke dokumen PDF secara dinamis.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Siapkan template dengan placeholder barcode
          // <<barcode [barcode_expression] -barcode_type>>

          // Tetapkan jalur ke file template Anda
          // Template PDF saat ini tidak didukung.
          String template = "barcode_template.docx";

          // Muatan data dari sumber tertentu
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Bangun objek sumber data dengan data yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Buat instance dari DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Sesuaikan pengaturan barcode
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Simpan dokumen yang diperbarui dengan barcode
          asm.assembleDocument(template, "result.pdf", data);
          ```
        platform: "java"
        copy_title: "Salin"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Jelajahi fitur GroupDocs.Assembly secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduh dari Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Pelajari tentang lisensi"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Temukan fitur utama"
    exclude: "barcode"
    description: "Platform kami menyederhanakan penanganan dokumen bisnis dengan alat dan otomatisasi yang kuat."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/java/barcode/pdf/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/java/chart/pdf/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/java/document/pdf/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/java/list/pdf/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/java/table/pdf/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buat laporan dalam berbagai format"
    exclude: "PDF"
    description: "Java mendukung lebih dari 50 jenis file, memungkinkan penggabungan data dan pemrosesan template secara effortless untuk hasil profesional."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/assembly/java/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/assembly/java/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/assembly/java/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/assembly/java/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---