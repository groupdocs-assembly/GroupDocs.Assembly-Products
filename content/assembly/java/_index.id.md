---
layout: "product"
date: 2022-07-07T12:44:18+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

head_title: "Perakitan Otomatisasi Dokumen Java & API Pembuat Laporan Dinamis"
head_description: "Java API untuk otomatisasi dokumen, perakitan & pelaporan. Buat laporan dari template khusus. Rakit PDF Word Excel PPTX HTML dari sumber data DB, JSON, OData & XML."

title: "Java API untuk Mengotomatiskan Dokumen & Laporan"
description: "Membangun Aplikasi Otomasi Dokumen untuk Mengambil Data; letakkan di Template yang Dapat Disesuaikan & Hasilkan Laporan Dinamis melalui Java API."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
        product: "GroupDocs.Assembly"
        platform: "Java"

    middle:
        button:
            - link: "#overview"
              text: "Ringkasan"

            - link: "#features"
              text: "Fitur"

            - link: "#support"
              text: "Mendukung"

            - link: "https://products.groupdocs.app/assembly"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java API membantu Anda dengan cepat mengembangkan otomatisasi dokumen dan aplikasi pelaporan di Java untuk menghasilkan laporan kustom dari template tanpa menginstal perangkat lunak eksternal apa pun. Mesin pembuat laporan mengambil data dari dokumen template, merakitnya dan menghasilkan laporan dalam format output yang ditentukan sesuai dengan sintaks yang ditentukan. Ini memungkinkan Anda untuk mengonfigurasi dan menyisipkan properti pemformatan elemen template secara dinamis dan mendukung berbagai sumber data (JSON, XML, OData, database, CSV, spreadsheet sebagai tabel data, tabel pengolah kata sebagai tabel data dan database) untuk mengambil data.  

      Pustaka rakitan dokumen mengenali beberapa format dokumen dan memungkinkan Anda membuat templat di semua jenis file yang didukung seperti PDF, HTML, email Outlook, Microsoft Office Word, lembar kerja Excel, presentasi PowerPoint, dan teks. Ini mendukung sintaks template berbasis LINQ dan pengguna juga dapat mengonfigurasi dan menyisipkan properti pemformatan elemen template secara dinamis.  

      GroupDocs.Assembly untuk Java mudah diintegrasikan dengan aplikasi java baru atau yang sudah ada. Ini sangat kompatibel dengan semua versi Java dan mendukung sistem operasi populer (Windows, Linux, MacOS) yang mampu menjalankan runtime Java.
    tabs:
      enable: true     
      
      tab_one:
        description: |
          Berikut ini adalah ikhtisar GroupDocs.Assembly untuk Java:

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Ringkasan"
          content: |
            * Formulasi Data
            * Pemformatan Data
            * Otomatisasi Data
            * Buat Template
            * Pemformatan Elemen Template
            * Pembuatan Laporan
      
      tab_two:
        description: |
          [Format file dokumen](https://docs.groupdocs.com/assembly/java/supported-document-formats/) yang didukung untuk API pembuatan dokumen Java tercantum di bawah ini.

        left:
          enable: true
          table:
            - title: "Format Microsoft Office"
              content: |
                * **Kata**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            - title: "Sumber Data yang Didukung"
              content: |
                * Basis Data
                * XML
                * OData
                * JSON
                * CSV
                * Objek .NET Kustom
                * Spreadsheet sebagai Tabel Data
                * Tabel Pengolah Kata sebagai Tabel Data

        right:
          enable: true
          table:
            - title: "Format lainnya"
              content: |
                * **Format Dokumen OpenOffice**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **File Dokumentasi Penurunan Harga**: MD
                * **Lainnya**: TXT

            - title: "Dukungan Perakitan Antar-Format"
              content: |
                * Pemrosesan Kata **TO** Pemrosesan Kata, HTML, PDF, XPS, TIFF, MHTML, Penurunan Harga, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Spreadsheet **TO** Spreadsheet, HTML, PDF, XPS, TIFF, MHTML
                * Presentasi **TO** Presentasi, HTML, PDF, XPS, TIFF
                * Email **TO** Pemrosesan Kata, Email, HTML, PDF, XPS, TIFF, MHTML, Penurunan Harga, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML & TXT **TO** Pemrosesan Kata, HTML, PDF, XPS, TIFF, MHTML, Penurunan Harga, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      tab_three:
        description: |
          GroupDocs.Assembly untuk Java mendukung Sistem Operasi, Kerangka Kerja & Manajer Paket berikut:
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "Sistem operasi"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            - icon: "fas fa-code"
              title: "Kerangka yang Didukung"
              content: |
                * Java 7 (1.7) ke atas

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "Lingkungan Pengembangan"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            - icon: "fas fa-tools"
              title: "Bangun Alat Otomatisasi"
              content: |
                * Maven

features:
    enable: true
    title: "GroupDocs.Assembly untuk Fitur Java"

    feature:
      - icon: "fas fa-copy"
        content: "Sesuaikan Gambar di Textbox Word, Excel, Presentasi & Email sambil Mempertahankan Rasio Gambar"

      - icon: "fas fa-eye"
        content: "Gunakan Rumus & Lakukan Operasi Data Berurutan - Terapkan Rumus selama Perakitan Spreadsheet"

      - icon: "fas fa-bolt"
        content: "Terapkan Pemformatan Atas, Bawah, Kapital, FirstCap ke String di Sintaks Template"
      
      - icon: "fas fa-file-powerpoint"
        content: "Dukungan Sintaks Templat Pemformatan Sifat Numerik Ordinal, Kardinal, Alfabetik"

      - icon: "fas fa-code"
        content: "Mendukung Dokumen Template dengan Variabel Khusus & Komentar Teks dalam Tag Sintaks Template"

      - icon: "fas fa-cloud"
        content: "Sisipkan Konten Dokumen Secara Dinamis dalam Laporan"

      - icon: "fas fa-remove-format"
        content: "Konfigurasi Secara Dinamis Warna Latar Belakang Dokumen HTML & Hasilkan Barcode di Laporan"

      - icon: "fas fa-comment-slash"
        content: "Sisipkan Hyperlink secara Dinamis di Laporan & Terapkan Atribut ke Badan Pesan Email"

      - icon: "fas fa-location-arrow"
        content: "Lampirkan Lampiran Email dan Perbarui Bidang Secara Dinamis selama Perakitan Dokumen Pemrosesan Kata"

      - icon: "fas fa-border-all"
        content: "Dukungan Analog Bidang BERIKUTNYA dari Microsoft Word"

      - icon: "fas fa-wrench"
        content: "Tambahkan Tautan dan Bookmark secara Dinamis ke Format Dokumen dan Beri Nama Rentang Sel Spreadsheet Excel"

      - icon: "fas fa-columns"
        content: "Memuat & Menyimpan Format Dokumen Presentasi POT & OTP Rakitan"

      - icon: "fas fa-file-word"
        content: "Pemformatan Template untuk Numerik, Teks, Gambar, Tanggal-Waktu, Elemen Bagan"

      - icon: "fas fa-envelope"
        content: "Sisipkan gambar & dokumen secara dinamis dari byte yang disandikan Base64"

      - icon: "fas fa-print"
        content: "Sintaks Template Berbasis LINQ"

      - icon: "fas fa-file-archive"
        content: "Ubah Format File Rakitan menggunakan Spesifikasi Eksplisit atau Ekstensi File"

      - icon: "fas fa-lock"
        content: "Daftar Pesanan Didukung untuk Penurunan Harga - Simpan Email & Dokumen Word yang Baru Dirakit ke Penurunan Harga"

      - icon: "fas fa-file-code"
        content: "Hasilkan Berbagai Jenis Laporan, mis., Bagan, Gambar, Tabel, Daftar, dan lainnya"
      
      - icon: "fas fa-fill-drip"
        content: "Kesalahan Sintaks Template Sebaris dalam Dokumen yang Dihasilkan alih-alih Melempar Pengecualian"

      - icon: "fas fa-file-excel"
        content: "Mulai Ulang Daftar Bernomor secara Dinamis di Dokumen Word serta Email dengan Badan HTML & RTF"

      - icon: "fas fa-heading"
        content: "Dukungan Tabel, Tautan Otomatis, Tautan Sebaris, dan Gambar untuk Dokumen Penurunan Harga Rakitan"

      - icon: "fas fa-project-diagram"
        content: "Menghasilkan Barcode Secara Dinamis (GS1-128 AI 8102 Kupon Diperpanjang dan Kupon UPCA & GS1 Databar"

      - icon: "fas fa-cube"
        content: "Muat Dokumen Template dari HTML dengan Sumber Daya dan Simpan Rakitan Word, Excel, PowerPoint & Email ke HTML dengan Sumber Daya"

    more_feature:
      - title: "Memanipulasi Elemen Template"
        content: |
          Manipulasi banyak elemen template dengan GroupDocs.Assembly untuk Java API. Elemen template yang dapat Anda gunakan termasuk, blok teks, Gambar, Hyperlink, blok HTML, Barcode (melalui font Barcode), dan Bagan. Anda juga dapat menerapkan blok berulang & blok bersyarat untuk item daftar dan baris tabel. Penggabungan dinamis sel tabel yang menyimpan teks yang sama, berdasarkan ekspresi template untuk dokumen, presentasi, spreadsheet, dan email dengan badan HTML dan RTF.
      
      - title: "Memanipulasi Daftar Laporan"
        content: |
          Menggunakan GroupDocs.Assembly untuk Java API, mendukung jenis Laporan Daftar berikut:  

          * Daftar Berpoin
          * Daftar Bernomor
          * Daftar Bernomor Berwarna

      - title: "Memanipulasi Laporan Bagan"
        content: |
          GroupDocs.Assembly untuk Java mendukung jenis Laporan Bagan berikut:

          * Bagan Gelembung, yang menampilkan tiga dimensi data
          * Bagan Kolom
          * Pie chart
          * Bagan Sebar
          * Bagan Seri (Berwarna)

      - title: "Memanipulasi Laporan Tabel"
        content: |
          GroupDocs.Assembly untuk Java mendukung jenis Laporan Tabel berikut:  

          * Tabel Master-Detail
          * Tabel dengan Baris yang Disorot
          * Tabel dengan Konten Alternatif
          * Tabel dengan Filtering, Grouping, dan Ordering  

          Anda juga dapat menggunakan Pita Data di baris tabel.

      - title: "Memanipulasi Laporan Bagan"
        content: |
          Integrasi GroupDocs.Assembly untuk Java API dengan aplikasi Java Anda sangat mudah. Berikut ini adalah contoh blok kode yang menghasilkan laporan dalam format OpenDocument menggunakan Java:  

          ```java
          // Membuat instance kelas DocumentAssembler
          DocumentAssembler assembler = new DocumentAssembler();
          //Panggil AssembleDocument untuk menghasilkan laporan
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          //(Lihat detail metode DataStorage() baru di https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java)
          ```

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Assembly menawarkan API tampilan dokumen untuk lingkungan pengembangan populer lainnya"

    solution:
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

back_to_top:
  enable: true
---
