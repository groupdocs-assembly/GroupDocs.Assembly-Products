---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: id
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

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
head_title: "API .NET untuk Otomasi Dokumen, Penyusunan & Generasi Laporan"
head_description: "API C# .NET untuk otomasi dokumen, penyusunan, dan generasi laporan. Buat dokumen PDF, Word, Excel, PPTX, HTML, dan email dari template kustom."

############################# Header ############################
title: "API Otomasi & Pelaporan Dokumen .NET"
description: "Hasilkan laporan dalam aplikasi .NET dengan mendefinisikan template dan menggabungkan data."
words:
  for: "untuk"

actions:
  main: "Unduh Uji Coba melalui Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Lisensi"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Siap untuk Memulai?"
  description: "Coba fitur GroupDocs.Assembly secara gratis atau minta lisensi."

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Mengisi Grafik di DOCX Menggunakan C#"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Path ke template utama
    string template = "chart_template.docx";

    // Ambil data produktivitas manajer dari sumber
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Buat instance DataSourceInfo dengan data
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Atur warna grafik menggunakan DataSourceInfo lain
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Isi template dengan data dan simpan ke output
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Ikhtisar GroupDocs.Assembly"
  description: "Solusi .NET untuk mengotomatisasi pembuatan dokumen dengan integrasi data yang canggih."
  features:
    # feature loop
    - title: "Tambahkan Data Bisnis ke Template Dokumen dengan C#"
      content: "Generasi laporan yang mudah: Dengan GroupDocs.Assembly for .NET, Anda dapat dengan mudah menyisipkan data dari sumber seperti JSON atau XML ke dalam template yang telah ditentukan."

    # feature loop
    - title: "Proses Objek Data Bawaan"
      content: "Jenis dokumen yang didukung termasuk objek tertanam seperti diagram, grafik, tabel, dan daftar yang dapat diisi secara otomatis dengan data."

    # feature loop
    - title: "Fitur Tambahan"
      content: "GroupDocs.Assembly for .NET menyediakan opsi kustomisasi yang luas. Rancang objek data secara programatis, hasilkan barcode, gunakan sumber data online melalui URL, dan simpan output dalam berbagai format."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Assembly for .NET kompatibel dengan sistem operasi, framework, dan pengelola paket berikut."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Assembly for .NET dapat memproses [format file berikut](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "Fitur GroupDocs.Assembly"
  description: "Buat dokumen dan laporan menggunakan model data yang canggih."

  items:
    # feature loop
    - icon: "preview"
      title: "Representasi Data yang Canggih"
      content: "Mendukung berbagai objek data seperti grafik, daftar, tabel, gambar, dan lainnya."

    # feature loop
    - icon: "manipulate"
      title: "Manipulasi Data"
      content: "Terapkan formula dan operasi berurutan untuk memformat dan menampilkan data secara efektif."

    # feature loop
    - icon: "two_pages"
      title: "Berbagai Format yang Didukung"
      content: "Bekerja dengan lancar dengan semua format dokumen umum untuk template atau file output."

    # feature loop
    - icon: "document_settings"
      title: "Markup Template yang Kaya"
      content: "Manfaatkan format numerik, kardinal, dan alfabetik dalam template."

    # feature loop
    - icon: "text"
      title: "Sisipkan Barcode"
      content: "Hasilkan gambar barcode secara dinamis dan sisipkan ke dalam dokumen Anda."

    # feature loop
    - icon: "add"
      title: "Format Data"
      content: "Format string dalam template sebagai huruf besar, huruf kecil, gaya diberi huruf kapital, atau kapitalisasi huruf pertama."

    # feature loop
    - icon: "manipulate"
      title: "Manipulasi Konten Dokumen"
      content: "Sisipkan konten dari dokumen eksternal secara dinamis ke dalam laporan Anda."

    # feature loop
    - icon: "convert"
      title: "Simpan dalam Beberapa Format"
      content: "Tentukan format file output menggunakan ekstensi file atau konfigurasi terperinci."

    # feature loop
    - icon: "update"
      title: "Proses Data yang Fleksibel"
      content: "Sisipkan gambar dan dokumen secara dinamis menggunakan byte yang terenkode Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Potongan kode untuk operasi GroupDocs.Assembly yang khas."
  items:
    # code sample loop
    - title: "Daftar Bertitik dalam Dokumen Microsoft Word"
      content: |
        [Daftar bertitik](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) adalah cara umum untuk menyajikan data bisnis. Berikut adalah contoh menambahkan daftar ke dokumen Word menggunakan GroupDocs.Assembly.
        {{< landing/code title="Cara Mengisi Daftar dalam Dokumen">}}
        ```csharp {style=abap}
        // Sisipkan template ini di halaman dokumen:
        // Indikator kinerja manajer
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Tentukan path template
        string template = "Bulleted List Template.docx";

        // Atur path file output
        string result = "Result Report.docx"

        // Ambil data manajer dari sumber JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Hasilkan laporan dengan data yang diisi
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Grafik Pie dalam Presentasi PPTX"
      content: |
        Anda dapat membuat [Grafik Pie](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) menggunakan template dan data XML. Tingkatkan laporan Anda dengan representasi data yang menarik secara visual.
        {{< landing/code title="Cara Mewakili Data dalam Grafik Pie">}}
        ```csharp {style=abap}
        // Tambahkan template judul grafik ke presentasi:
        // Pendapatan pelanggan <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Sertakan juga template data grafik:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Tentukan path template grafik
        string template = "Pie Chart Template.pptx";

        // Atur path file output
        string result = "Result Report.pptx"

        // Ambil data pelanggan dari sumber XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Hasilkan grafik dan simpan hasilnya
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---