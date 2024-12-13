



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:57
draft: false
lang: id
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tambahkan tabel ke dokumen PDF menggunakan Java"
head_description: "Dengan GroupDocs.Assembly for Java, pengembang dapat dengan cepat mengintegrasikan tabel ke dalam dokumen dan email, mengambil data dari sumber dinamis."

############################# Header ############################
title: "Isi tabel dalam file PDF dengan API Java kami" 
description: "GroupDocs.Assembly for Java menyederhanakan proses pengisian tabel dalam dokumen PDF dengan data dari berbagai sumber."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan Percobaan Gratis Anda"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) adalah alat untuk menghasilkan dokumen dan laporan dengan secara otomatis memasukkan data ke dalam template yang telah dirancang sebelumnya. Anda dapat menambahkan tabel, daftar, grafik, dan gambar dengan mudah. Fitur-fitur canggihnya memungkinkan Anda untuk menempatkan konten dengan presisi dalam dokumen Anda. Kompatibel dengan lebih dari 50 jenis file, termasuk PDF, MS Office, dan format email.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk memasukkan data ke dalam tabel PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) membantu Anda mengisi template tabel untuk PDF dan format lainnya. Gunakan data dinamis dari sumber Anda untuk membuat tabel.
      
      1. Desain template dengan placeholder untuk tabel (template PDF saat ini tidak didukung).
      2. Ambil data dari sumber input yang didukung.
      3. Filter atau praproses data agar sesuai dengan kebutuhan Anda.
      4. Simpan dokumen dengan tabel terisi sebagai file PDF.
   
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
        // Gunakan tag ini dalam tempat placeholder baris tabel dalam template Anda
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Tentukan jalur ke file template
        // Template PDF tidak didukung saat ini.
        String template = "table_template.docx";

        // Muat data dari sumber yang Anda pilih
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Simpan file keluaran dengan tabel terisi
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Buat dokumen dengan tabel yang terisi data"
  description: "GroupDocs.Assembly for Java mempermudah otomatisasi pembuatan tabel dalam dokumen Anda. Ini juga mendukung penambahan elemen seperti grafik, daftar, dan gambar menggunakan template."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Hasilkan laporan dari berbagai format data"
      content: "API bekerja secara mulus dengan JSON, XML, CSV, dan format lainnya untuk mengisi tabel dalam dokumen Anda dengan data yang terorganisir."

    # feature loop
    - title: "Sajikan informasi secara visual"
      content: "GroupDocs.Assembly membantu Anda membuat tabel, daftar, dan grafik yang profesional, serta menyisipkan tautan, teks, dan gambar, untuk tampilan yang rapi."

    # feature loop
    - title: "Tempatkan konten tabel dengan presisi"
      content: "Gunakan sintaks fleksibel berbasis LINQ untuk menambahkan baris dan kolom secara dinamis. Sesuaikan penampilan, seperti gaya dan warna font, secara programatik."

    # feature loop
    - title: "Kompatibel dengan berbagai format"
      content: "Bekerja dengan MS Office, OpenOffice, PDF, HTML, dan lainnya. Gabungkan tabel ke dalam format file yang didukung dengan mudah."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Buat tabel terisi data secara dinamis"
      content: |
        Contoh ini menunjukkan cara mengisi tabel dalam dokumen PDF menggunakan data input dinamis.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Desain template dengan placeholder untuk tabel
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Tetapkan lokasi file template
          // Template PDF tidak didukung saat ini.
          String template = "table_template.docx";

          // Muat data dari sumber yang Anda pilih
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Siapkan objek data yang berisi bidang yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Buat instance dari DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan dokumen dengan tabel yang terisi
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
            link: "/examples/assembly/formats/assembly_table.pdf"
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
    title: "Fitur kunci dalam sekilas"
    exclude: "table"
    description: "API kami menyederhanakan pembuatan dokumen profesional dengan mengotomatisasi pengisian tabel di samping komponen kuat lainnya."
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
    title: "Hasilkan tabel terperinci dalam berbagai format"
    exclude: "PDF"
    description: "Dengan Java, Anda dapat mengisi template dengan data dan menghasilkan laporan terperinci dalam lebih dari 50 jenis file."
    items: 
          
        # format loop 1
        - name: "Tambahkan tabel ke PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan tabel ke DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan tabel ke PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Tambahkan tabel ke XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---