



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: id
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buat grafik dalam file XLSX dengan C#"
head_description: "API GroupDocs.Assembly for .NET memungkinkan pengembang untuk menghasilkan dan menyisipkan grafik ke dalam dokumen secara dinamis menggunakan data waktu nyata."

############################# Header ############################
title: "Sisipkan grafik dalam file XLSX dengan API .NET" 
description: "GroupDocs.Assembly for .NET memberikan cara yang ampuh untuk mengisi file XLSX dengan data dinamis dan mengintegrasikan grafik dengan lancar."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) adalah alat yang dirancang untuk menyederhanakan pembuatan dokumen dan laporan dengan mengintegrasikan data dari berbagai sumber. Hasilkan grafik, tabel, daftar, kode batang, dan gambar secara dinamis. Opsi format yang canggih memungkinkan penempatan dan kustomisasi konten Anda dengan tepat. Mendukung lebih dari 50 format file, termasuk PDF, dokumen MS Office, dan email.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menambahkan grafik ke dokumen XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) memudahkan untuk menghasilkan dan menyisipkan grafik ke dalam templat XLSX Anda. Mendukung berbagai jenis grafik, seperti grafik batang, lingkaran, dan garis.
      
      1. Rancang templat XLSX dengan placeholder untuk grafik.
      2. Ambil data Anda dari sumber yang kompatibel.
      3. Tentukan opsi grafik seperti tipe, label, dan skema warna.
      4. Simpan file yang diperbarui dengan grafik disisipkan.
   
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
        // Sertakan tag ini dalam templat Anda untuk menghasilkan grafik
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Tentukan jalur file untuk templat Anda
        string template = "chart_template.xlsx";

        // Ambil data dari sumber pilihan Anda
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Simpan dokumen dengan grafik yang disisipkan
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tambahkan grafik dinamis ke dokumen Anda tanpa kesulitan"
  description: "GroupDocs.Assembly for .NET menyederhanakan pembuatan dokumen berbasis data dalam format yang banyak digunakan. Gunakan templat untuk menyisipkan grafik, tabel, kode batang, daftar, superlink, dan gambar dengan integrasi data dinamis yang canggih."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Ubah data menjadi grafik profesional"
      content: "Ubah data dari JSON, XML, CSV, dan sumber lainnya menjadi grafik yang menarik secara visual hanya dengan beberapa langkah menggunakan API kami."

    # feature loop
    - title: "Buat konten yang menarik secara visual"
      content: "GroupDocs.Assembly mendukung berbagai jenis grafik seperti grafik batang, grafik lingkaran, dan grafik garis. Gabungkan ini dengan tabel, kode batang, gambar, dan elemen lain untuk membuat laporan profesional."

    # feature loop
    - title: "Posisikan dan kustomisasi grafik dengan tepat"
      content: "Dengan sintaks LINQ, Anda dapat menghasilkan dan menempatkan grafik secara dinamis tepat di tempat yang diperlukan. Kustomisasi gaya, warna, dan tata letak untuk memenuhi kebutuhan Anda."

    # feature loop
    - title: "Bekerja dengan berbagai format file"
      content: "Hasilkan dokumen dalam format populer seperti MS Office, PDF, OpenOffice, dan HTML. Sisipkan grafik secara mulus ke dalam format apa pun yang didukung dengan kompatibilitas penuh."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Buat grafik secara programatis"
      content: |
        Contoh ini menunjukkan cara membuat dan menyisipkan grafik secara dinamis ke dalam dokumen XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Siapkan templat dengan placeholder untuk grafik
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Berikan jalur ke file templat
          string template = "table_template.xlsx";

          // Ambil data dari sumber Anda
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Bangun objek data dengan informasi yang diperlukan
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Atur properti grafik seperti tipe dan tampilan
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inisialisasi DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Ekspor dokumen dengan grafik yang disertakan
          asm.AssembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Temukan kemampuan kunci"
    exclude: "chart"
    description: "Platform kami membantu Anda membuat dokumen yang menarik dan berbasis data yang disesuaikan dengan kebutuhan Anda."
    items: 
          
        # operation loop 1
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "Buat dan tambahkan barcode secara dinamis ke dokumen"

        # operation loop 2
        - name: "Visualisasikan data dengan diagram"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "Isi berbagai jenis diagram dengan data"

        # operation loop 3
        - name: "Gabungkan dokumen"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "Kombinasikan konten satu dokumen ke dokumen lain"

        # operation loop 4
        - name: "Tampilkan data dengan daftar"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "Hasilkan daftar dalam dokumen menggunakan data tertentu"

        # operation loop 5
        - name: "Atur data dalam tabel"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "Ambil data dari sumber mana pun dan isi tabel"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buat laporan yang kaya secara visual dalam berbagai format"
    exclude: "XLSX"
    description: ".NET memungkinkan Anda menghasilkan dokumen dengan grafik terintegrasi di lebih dari 50 format yang didukung, menggabungkan templat dengan data Anda dengan mulus."
    items: 
          
        # format loop 1
        - name: "Diagram dalam PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Diagram dalam DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Diagram dalam PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Diagram dalam XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---