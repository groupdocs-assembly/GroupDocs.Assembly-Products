---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:12
draft: false

lang: id
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

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
head_title: "Perpustakaan Java untuk Pembuatan, Otomasi & Pelaporan Dokumen"
head_description: "Perpustakaan Java untuk mengotomatisasi pembuatan dokumen dan menghasilkan laporan. Buat dokumen PDF, Word, Excel, PPTX, HTML, dan email menggunakan template kustom."

############################# Header ############################
title: "API Java untuk Mengotomatisasi Laporan dan Dokumen"
description: "Sederhanakan pembuatan laporan di Java dengan menggabungkan data dengan template."
words:
  for: "untuk"

actions:
  main: "Dapatkan Uji Coba melalui Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Lisensi"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Siap untuk Memulai?"
  description: "Coba fitur GroupDocs.Assembly secara gratis atau minta lisensi."

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Hasilkan Grafik di DOCX dengan Java"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Path ke template utama
    String template = "chart_template.docx";

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
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Ikhtisar GroupDocs.Assembly"
  description: "Perpustakaan Java yang dirancang untuk pembuatan dokumen otomatis dan integrasi data yang mulus."
  features:
    # feature loop
    - title: "Gabungkan Data Bisnis ke dalam Template dengan Java"
      content: "Buat laporan profesional dengan mudah dengan memasukkan data dari JSON, XML, atau sumber lain ke dalam template yang telah dirancang menggunakan GroupDocs.Assembly for Java."

    # feature loop
    - title: "Bekerja dengan Objek Tertanam"
      content: "Isi elemen secara otomatis seperti tabel, grafik, dan diagram dalam dokumen menggunakan data dari sumber eksternal."

    # feature loop
    - title: "Kustomisasi Canggih"
      content: "GroupDocs.Assembly for Java menawarkan fitur fleksibel seperti menghasilkan barcode, menarik data online melalui URL, dan mengekspor output dalam berbagai format."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Assembly for Java bekerja dengan mulus dengan sistem operasi, framework, dan pengelola paket populer."
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
    GroupDocs.Assembly for Java mendukung berbagai [format dokumen](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Kemampuan Utama GroupDocs.Assembly"
  description: "Buat dokumen profesional dan laporan dengan penanganan data yang canggih."

  items:
    # feature loop
    - icon: "preview"
      title: "Elemen Data Visual"
      content: "Tambahkan dan format elemen seperti grafik, tabel, gambar, dan daftar langsung di dokumen Anda."

    # feature loop
    - icon: "manipulate"
      title: "Transformasi Data"
      content: "Gunakan formula, penyortiran, dan alat lainnya untuk mengatur dan menyajikan data Anda secara efektif."

    # feature loop
    - icon: "two_pages"
      title: "Dukungan untuk Berbagai Format"
      content: "Dengan mudah bekerja dengan tipe file umum untuk template dan file output."

    # feature loop
    - icon: "document_settings"
      title: "Format Template yang Ditingkatkan"
      content: "Kustomisasi template dengan opsi format numerik, alfabetik, dan lainnya."

    # feature loop
    - icon: "text"
      title: "Pembuatan Barcode Dinamis"
      content: "Dengan cepat buat dan sisipkan gambar barcode ke dalam dokumen sesuai kebutuhan."

    # feature loop
    - icon: "add"
      title: "Gaya Teks Fleksibel"
      content: "Terapkan transformasi teks seperti huruf besar, huruf kecil, gaya judul, atau gaya lain dalam template."

    # feature loop
    - icon: "manipulate"
      title: "Impor Konten Eksternal"
      content: "Sisipkan konten dari file eksternal secara dinamis saat menghasilkan dokumen."

    # feature loop
    - icon: "convert"
      title: "Ekspor dalam Berbagai Format"
      content: "Simpan dokumen akhir dalam berbagai format file menggunakan ekstensi atau konfigurasi yang ditentukan."

    # feature loop
    - icon: "update"
      title: "Sisipan Media Dinamis"
      content: "Sisipkan gambar atau konten lain menggunakan data yang terenkode Base64 saat pembuatan dokumen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Jelajahi kode sampel untuk tugas umum dengan GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Buat Daftar Bertitik di Word"
      content: |
        Pelajari cara menambahkan [daftar bertitik](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) ke dokumen Word untuk representasi data yang terorganisir. Contoh ini menunjukkan cara menghasilkan daftar di Word menggunakan GroupDocs.Assembly.
        {{< landing/code title="Buat Daftar Bertitik di Word">}}
        ```java {style=abap}
        // Sisipkan template ini di halaman dokumen:
        // Indikator kinerja manajer
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Tentukan path template
        String template = "Bulleted List Template.docx";

        // Atur path file output
        String result = "Result Report.docx"

        // Ambil data manajer dari sumber JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Hasilkan laporan dengan data yang diisi
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Buat Grafik Pie di PPTX"
      content: |
        Gunakan template dan XML untuk menambahkan [grafik pie](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) ke presentasi Anda. Buat laporan Anda lebih menarik dengan menyertakan grafik pie untuk memvisualisasikan data.
        {{< landing/code title="Buat Grafik Pie di PPTX">}}
        ```java {style=abap}   
        // Tambahkan template judul grafik ke presentasi:
        // Pendapatan pelanggan <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Sertakan juga template data grafik:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Tentukan path template grafik
        String template = "Pie Chart Template.pptx";

        // Atur path file output
        String result = "Result Report.pptx"

        // Ambil data pelanggan dari sumber XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Hasilkan grafik dan simpan hasilnya
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---