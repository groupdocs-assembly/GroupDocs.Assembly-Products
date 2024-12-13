



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: id
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buat daftar dalam dokumen PPTX menggunakan Java"
head_description: "Rancang dan sisipkan daftar dinamis ke dalam template PPTX Anda dengan API GroupDocs.Assembly for Java."

############################# Header ############################
title: "Tambahkan daftar dinamis ke file PPTX dengan API Java kami" 
description: "GroupDocs.Assembly for Java menyediakan alat yang fleksibel untuk menghasilkan dan menyisipkan daftar kaya data langsung ke dalam dokumen PPTX."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) memudahkan Anda merancang dokumen profesional dengan menarik data dari berbagai sumber. Gunakan untuk membuat daftar, tabel, grafik, atau teks, dan tempatkan elemen ini secara tepat di mana dibutuhkan dengan fitur template yang canggih. Dengan dukungan untuk lebih dari 50 format, termasuk PDF, file MS Office, dan dokumen email, ini membantu mengotomatiskan dan menyederhanakan alur kerja Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menambahkan daftar berbasis data ke dokumen PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) memungkinkan Anda dengan cepat menyisipkan daftar kaya data ke dalam template PPTX. Sesuaikan dan atur konten tanpa kesulitan.
      
      1. Buat template PPTX dan tandai tempat untuk daftar.
      2. Atur jalur file ke template.
      3. Ambil data dari format yang didukung seperti JSON atau XML.
      4. Simpan dokumen akhir dengan daftar yang ditambahkan.
   
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
        // Sisipkan tag ini di template Anda di mana daftar harus muncul
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Tentukan jalur file template
        String template = "list_template.pptx";

        // Ambil data dari sumber yang Anda pilih
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Simpan dokumen dengan daftar yang disisipkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Hasilkan dokumen dari template dengan integrasi data"
  description: "GroupDocs.Assembly for Java menyederhanakan penambahan daftar dinamis, tabel, grafik, dan komponen lainnya ke dalam template dokumen."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Bangun laporan dengan data dari berbagai sumber"
      content: "Gunakan data dari format seperti JSON, XML, dan CSV untuk mengisi daftar dan komponen lainnya secara efisien."

    # feature loop
    - title: "Tambahkan daftar dan elemen data lainnya dengan mulus"
      content: "GroupDocs.Assembly memungkinkan penyisipan daftar, grafik, tabel, dan lainnya, bersama teks, gambar, dan tautan untuk membuat dokumen yang rapi."

    # feature loop
    - title: "Kontrol tepat di mana data muncul"
      content: "Template berbasis LINQ memungkinkan Anda menentukan lokasi yang tepat untuk daftar dan data Anda. Gunakan loop untuk membuat daftar terperinci secara otomatis dan terapkan format kustom."

    # feature loop
    - title: "Mendukung berbagai format dokumen"
      content: "Buat atau edit file dalam format seperti MS Office, PDF, OpenOffice, HTML, dan email. Gabungkan konten dari beberapa dokumen sesuai kebutuhan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara membuat daftar secara programatis"
      content: |
        Contoh ini menunjukkan cara menambahkan daftar secara dinamis ke dalam file PPTX menggunakan GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Tambahkan tag placeholder di template Anda untuk daftar
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Berikan jalur file ke template Anda
          String template = "numlist_template.pptx";

          // Ambil data yang diperlukan untuk mengisi daftar
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Siapkan sumber data dengan rincian yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inisialisasi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Simpan dokumen output dengan daftar yang telah selesai
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "Temukan apa yang bisa dilakukan GroupDocs.Assembly"
    exclude: "list"
    description: "Rancang dan hasilkan dokumen kaya konten dengan alat integrasi data yang canggih."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Hasilkan dokumen dalam berbagai format"
    exclude: "PPTX"
    description: "Java mendukung lebih dari 50 format, memungkinkan Anda untuk membuat dokumen terstruktur dengan menggabungkan data dan template."
    items: 
          
        # format loop 1
        - name: "Buat daftar dalam PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Buat daftar dalam DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Buat daftar dalam PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Buat daftar dalam XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---