---
############################# Static ############################
layout: "landing"
date: 2025-01-16T13:04:06
draft: false

lang: id
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Toolkit Node.js untuk Membangun, Mengotomatiskan, dan Menyesuaikan Dokumen"
head_description: "Library Node.js untuk mengotomatiskan alur kerja dokumen. Hasilkan file PDF, Word, Excel, PowerPoint, HTML, dan email dari template Anda."

############################# Header ############################
title: "API Node.js untuk Otomasi Dokumen dan Laporan yang Disederhanakan"
description: "Percepat proses pembuatan laporan JavaScript dengan menggabungkan data Anda dengan template yang sudah ada."
words:
  for: "untuk"

actions:
  main: "Mulai Uji Coba Anda di NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Lisensi"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Siap untuk Memulai?"
  description: "Coba fitur GroupDocs.Assembly secara gratis atau minta lisensi."

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Buat Grafik dalam Dokumen Word Menggunakan Node.js"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Path ke template utama
    const template = "chart_template.docx";

    // Ambil data produktivitas manajer dari sumber
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Buat instance DataSourceInfo dengan data
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Atur warna grafik menggunakan DataSourceInfo lain
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Isi template dengan data dan simpan ke output
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Ikhtisar GroupDocs.Assembly"
  description: "Library Node.js yang dirancang untuk membuat dokumen secara programatik dengan penanganan data yang terintegrasi."
  features:
    # feature loop
    - title: "Integrasikan Data Bisnis ke dalam Template dengan JavaScript"
      content: "Hasilkan laporan yang menarik dengan menyematkan JSON, XML, atau data lainnya ke dalam template dengan GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Kelola Konten yang Disematkan"
      content: "Secara otomatis mengisi tabel, grafik, dan visual lainnya dalam dokumen Anda menggunakan data eksternal."

    # feature loop
    - title: "Opsi Kustomisasi"
      content: "GroupDocs.Assembly for Node.js via Java memungkinkan Anda menambahkan fitur seperti kode batang, mengambil data dari URL, dan mengekspor file dalam berbagai format."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Assembly for Node.js via Java terintegrasi dengan lancar dengan sistem operasi, kerangka kerja, dan manajer paket terkemuka."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Assembly for Node.js via Java mendukung berbagai macam [format dokumen](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Format Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Gambar & Format Lainnya
        * **Portabel:** PDF
        * **Gambar:** SVG, TIFF
        * **Format kantor lainnya:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Format Lainnya
        * **Web:** HTML, MHTML
        * **Email:** EML, MSG, EMLX
        * **Lainnya:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Fitur Utama GroupDocs.Assembly"
  description: "Buat dokumen dan laporan dinamis dengan alat manajemen data yang kuat."

  items:
    # feature loop
    - icon: "preview"
      title: "Visual Data Kaya"
      content: "Sisipkan grafik, tabel, gambar, dan daftar ke dalam dokumen Anda dengan kustomisasi penuh."

    # feature loop
    - icon: "manipulate"
      title: "Transformasi Data Anda"
      content: "Manfaatkan alat seperti rumus dan pengurutan untuk menyusun dan menampilkan informasi secara efektif."

    # feature loop
    - icon: "two_pages"
      title: "Kompatibilitas Format yang Luas"
      content: "Bekerja secara mulus dengan format file populer untuk template dan keluaran."

    # feature loop
    - icon: "document_settings"
      title: "Kustomisasi Template Lanjutan"
      content: "Format template dengan opsi gaya numerik, alfabet, dan lainnya."

    # feature loop
    - icon: "text"
      title: "Hasilkan Kode Batang Secara Dinamis"
      content: "Buat dan sematkan gambar kode batang langsung ke dalam dokumen Anda sesuai permintaan."

    # feature loop
    - icon: "add"
      title: "Gaya Teks Fleksibel"
      content: "Terapkan gaya teks seperti kapitalisasi atau huruf besar kecil judul di dalam template Anda."

    # feature loop
    - icon: "manipulate"
      title: "Penyisipan Konten Dinamis"
      content: "Sertakan konten dari file eksternal secara dinamis saat pembuatan dokumen."

    # feature loop
    - icon: "convert"
      title: "Ekspor ke Berbagai Format"
      content: "Simpan dokumen dalam berbagai format dengan konfigurasi yang Anda tentukan."

    # feature loop
    - icon: "update"
      title: "Sematkan Media Secara Dinamis"
      content: "Sisipkan gambar atau elemen lainnya menggunakan data Base64 saat membuat dokumen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Temukan contoh praktis tentang cara menggunakan GroupDocs.Assembly untuk tugas umum."
  items:
    # code sample loop
    - title: "Tambahkan Daftar Ber nomor dalam Dokumen Word"
      content: |
        Lihat cara membuat [daftar ber nomor](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) dalam dokumen Word untuk mengatur data secara efektif. Contoh ini menunjukkan cara menghasilkan daftar ber nomor menggunakan GroupDocs.Assembly.
        {{< landing/code title="Tambahkan Daftar Ber nomor dalam Dokumen Word">}}
        ```javascript {style=abap}
        // Sisipkan template ini di halaman dokumen:
        // Indikator kinerja manajer
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan path template
        const template = "Bulleted List Template.docx";

        // Atur path file output
        const result = "Result Report.docx"

        // Ambil data manajer dari sumber JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Hasilkan laporan dengan data yang diisi
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Sisipkan Grafik Lingkaran ke dalam PowerPoint"
      content: |
        Pelajari cara menggunakan template dan XML untuk menambahkan [grafik lingkaran](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) dalam presentasi Anda. Tingkatkan laporan Anda dengan grafik lingkaran untuk menyajikan data secara visual dan jelas.
        {{< landing/code title="Sisipkan Grafik Lingkaran ke dalam PowerPoint">}}
        ```javascript {style=abap} 
        // Tambahkan template judul grafik ke presentasi:
        // Pendapatan pelanggan <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Sertakan juga template data grafik:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Tentukan path template grafik
        const template = "Pie Chart Template.pptx";

        // Atur path file output
        const result = "Result Report.pptx"

        // Ambil data pelanggan dari sumber XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Hasilkan grafik dan simpan hasilnya
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---