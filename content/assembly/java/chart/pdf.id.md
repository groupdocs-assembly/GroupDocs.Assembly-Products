



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: id
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buat diagram dalam dokumen PDF menggunakan Java"
head_description: "API GroupDocs.Assembly for Java memungkinkan pengembang untuk membuat dan menyisipkan grafik atau diagram dinamis ke dalam dokumen secara mulus, didukung oleh data waktu nyata."

############################# Header ############################
title: "Tambahkan grafik ke dokumen PDF dengan API Java" 
description: "GroupDocs.Assembly for Java menyederhanakan proses penyisipan grafik ke dalam dokumen PDF dengan memanfaatkan data waktu nyata."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Pengantar GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) adalah solusi serbaguna untuk mengotomatiskan pembuatan dokumen dan laporan. Ini memungkinkan Anda menambahkan grafik, tabel, daftar, barcode, dan gambar langsung ke dalam file Anda, dengan alat canggih untuk pemformatan dan integrasi data yang tepat. Platform ini mendukung lebih dari 50 format, termasuk PDF, file Microsoft Office, dan email.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah untuk memasukkan grafik ke dalam dokumen PDF"
    content: |
      [GroupDocs.Assembly](/assembly/java/) menyederhanakan proses penyisipan grafik ke dalam template PDF. Pilih dari berbagai gaya grafik, termasuk grafik batang, lingkaran, dan garis.
      
      1. Buat template dengan tempat untuk grafik (template PDF tidak didukung).
      2. Muat data Anda dari sumber yang kompatibel.
      3. Tentukan opsi grafik, seperti jenis, label, dan warna.
      4. Simpan dokumen yang berisi grafik sebagai file PDF.
   
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
        // Tambahkan tag ini ke template Anda untuk menyertakan grafik
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Berikan jalur file ke template Anda
        // Template PDF tidak didukung saat ini.
        String template = "chart_template.docx";

        // Ambil data yang diperlukan dari sumber Anda
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Simpan dokumen akhir dengan grafik yang disisipkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Menyisipkan grafik dinamis ke dalam dokumen Anda dengan mudah"
  description: "GroupDocs.Assembly for Java menyediakan cara yang efektif untuk membangun dokumen kaya data dalam format populer. Gunakan template untuk menyisipkan grafik, tabel, barcode, daftar, tautan, dan gambar dengan pembaruan dinamis dari data Anda."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Fitur kunci dari GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Ubah data menjadi grafik"
      content: "Gunakan API untuk mengubah data dari JSON, XML, CSV, atau sumber lainnya menjadi grafik profesional yang bersih untuk dokumen Anda."

    # feature loop
    - title: "Buat konten yang berdampak visual"
      content: "GroupDocs.Assembly mendukung berbagai format visual, termasuk grafik batang, diagram lingkaran, dan grafik garis, yang dapat dikombinasikan dengan tabel, barcode, gambar, dan lainnya untuk laporan yang lebih baik."

    # feature loop
    - title: "Tempatkan dan sesuaikan grafik dengan fleksibilitas"
      content: "Dengan sintaks berbasis LINQ, Anda dapat secara dinamis menghasilkan dan memposisikan grafik dalam dokumen, sambil dengan mudah menyesuaikan gaya, warna, dan tata letak untuk memenuhi kebutuhan desain Anda."

    # feature loop
    - title: "Mendukung berbagai format dokumen"
      content: "Hasilkan dokumen dalam format seperti MS Office, PDF, OpenOffice, dan HTML. Grafik terintegrasi dengan mulus ke dalam format mana pun yang didukung untuk hasil yang profesional."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Secara programatis menghasilkan dan menyisipkan grafik"
      content: |
        Contoh ini menunjukkan cara membuat dan menyisipkan grafik ke dalam dokumen PDF secara programatis.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Siapkan template dengan tempat untuk grafik
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Tentukan jalur file ke template
          // Template PDF tidak didukung saat ini.
          String template = "table_template.docx";

          // Muat data dari sumber pilihan Anda
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Buat objek data dengan informasi yang relevan
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Konfigurasi jenis dan penampilan grafik
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inisialisasi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan dokumen yang telah selesai dengan grafik yang disisipkan
          asm.assembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "Jelajahi kemampuan yang kuat"
    exclude: "chart"
    description: "Platform ini menyederhanakan proses perancangan dokumen yang fokus pada data dan menarik secara visual sesuai kebutuhan Anda."
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
    title: "Hasilkan laporan komprehensif dalam berbagai format"
    exclude: "PDF"
    description: "Java memungkinkan Anda membuat dokumen dengan grafik yang terintegrasi di lebih dari 50 format file, memastikan penggabungan template dan data yang mulus."
    items: 
          
        # format loop 1
        - name: "Diagram dalam PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Diagram dalam DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Diagram dalam PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Diagram dalam XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---