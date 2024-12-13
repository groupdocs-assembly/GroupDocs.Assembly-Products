



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: id
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Sisipkan satu dokumen ke dalam dokumen XLSX menggunakan Java"
head_description: "Gabungkan file XLSX dengan Java. GroupDocs.Assembly menyederhanakan proses penggabungan dokumen hanya dalam beberapa baris kode."

############################# Header ############################
title: "Sisipkan konten ke dalam file XLSX dengan mudah" 
description: "Gunakan GroupDocs.Assembly for Java untuk menyisipkan satu dokumen XLSX ke dalam yang lain secara mulus. Dapatkan hasil yang tepat dengan alat yang fleksibel dan dapat diandalkan."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) adalah solusi serbaguna untuk menangani dokumen. Ini memungkinkan Anda untuk mengintegrasikan satu dokumen ke dalam dokumen lain, mendukung lebih dari 50 format seperti PDF dan file MS Office. Sesuaikan keluaran Anda dengan menggabungkan, mengedit, dan mengatur konten persis seperti yang Anda inginkan.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menyisipkan dokumen ke dalam file XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) memudahkan penyisipan satu dokumen XLSX ke dalam yang lain yang sederhana dan dapat disesuaikan.
      
      1. Siapkan templat XLSX dengan placeholder untuk konten yang disisipkan.
      2. Tentukan jalur file untuk templat.
      3. Berikan jalur file untuk dokumen yang ingin disisipkan.
      4. Simpan file keluaran dengan konten yang digabungkan.
   
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
        // Gunakan tag ini dalam templat Anda untuk menandai tempat untuk dokumen yang disisipkan
        // <<doc [doc_expression]>>

        // Tetapkan jalur file untuk templat utama
        String template = "doc_template.xlsx";

        // Berikan jalur ke dokumen yang ingin Anda sisipkan
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // Simpan file akhir dengan konten yang disisipkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Alat canggih untuk menyederhanakan integrasi dokumen"
  description: "Dengan GroupDocs.Assembly for Java, menyisipkan dokumen sangat mudah dan dapat disesuaikan, terlepas dari jenis file tersebut. Dapatkan hasil yang bersih dan konsisten di seluruh proyek Anda."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Sorotan GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Buat laporan menggunakan data bisnis"
      content: "Isi dokumen dengan data dari sumber seperti JSON, XML, atau CSV dengan cepat dan andal, menyederhanakan alur kerja Anda."

    # feature loop
    - title: "Tingkatkan dokumen dengan konten visual"
      content: "GroupDocs.Assembly memungkinkan Anda menyisipkan tabel, grafik, dan daftar bersama teks, tautan, gambar, dan bahkan kode batang dinamis."

    # feature loop
    - title: "Tempatkan data tepat di tempatnya"
      content: "Templat LINQ membantu menempatkan data Anda secara presisi, menangani elemen yang berulang seperti array, dan menerapkan gaya kustom dengan cepat."

    # feature loop
    - title: "Kompatibel dengan berbagai format file"
      content: "Gabungkan dokumen dari berbagai format, termasuk PDF, HTML, file MS Office, dan OpenOffice, memastikan fleksibilitas untuk proyek Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menyisipkan gambar ke dalam dokumen secara programatis"
      content: |
        Contoh ini menunjukkan cara menyisipkan gambar ke dalam file XLSX menggunakan GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Tambahkan tag placeholder dalam file templat
          // <<image [expression]>>

          // Tentukan jalur ke templat
          String template = "template.xlsx";

          // Tentukan jalur ke gambar
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inisialisasi instance DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan file dengan gambar yang disisipkan
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "Kemampuan utama dalam sekilas"
    exclude: "document"
    description: "Temukan fitur luas yang ditawarkan GroupDocs.Assembly untuk membuat penyisipan dan penggabungan dokumen menjadi efisien dan tanpa masalah."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Gabungkan berbagai jenis dokumen"
    exclude: "XLSX"
    description: "Dengan Java, Anda dapat menyisipkan dan menggabungkan konten di lebih dari 50 format file. Tambahkan file secara mulus untuk menghasilkan hasil profesional."
    items: 
          
        # format loop 1
        - name: "Sisipkan dokumen dalam PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Sisipkan dokumen dalam DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Sisipkan dokumen dalam PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Sisipkan dokumen dalam XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---