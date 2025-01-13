---
############################# Static ############################
layout: "family"
date:  2025-01-13T15:11:22
draft: false

product: "Assembly"
product_tag: "assembly"

lang: id

############################# Head ############################
head_title: "API & Aplikasi Penyusunan Dokumen .NET, Java oleh GroupDocs"
head_description: "Dapatkan Solusi Otomasi & Pelaporan Dokumen All-in-One untuk aplikasi .NET dan Java. Hasilkan semua dokumen umum dari template dan data kustom."

############################# Header ############################
title: "Solusi Otomasi dan Pelaporan Dokumen"
description:  |
  Buat laporan terperinci menggunakan template dan sumber data dengan aplikasi dan API lintas platform kami.

  Hasilkan laporan dalam format seperti Word, Excel, Presentasi, dan banyak lagi menggunakan template dengan markup yang fleksibel.

  Isi grafik, barcode, tabel, dan elemen lainnya dengan data dari sumber seperti JSON, XML, CSV, dll.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Pilih platform Anda"
  title: "Independensi platform"
  description: "GroupDocs.Assembly kompatibel dengan sistem operasi dan framework berikut:"
  details_link_title: "Pelajari lebih lanjut"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Editor teks lainnya
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Fitur Utama GroupDocs.Assembly"
  description: "Solusi ini membantu Anda membuat laporan dalam format dokumen yang populer, secara otomatis diisi dengan data bisnis Anda. Otomatisasi tugas pembuatan dokumen Anda."

  items:
    # items loop
    - icon: "additional"
      title: "Isi template dengan data"
      content: "Isi laporan menggunakan data dari sumber yang didukung."

    # items loop
    - icon: "manipulate"
      title: "Markup yang fleksibel"
      content: "Tambahkan data ke dokumen dengan cara yang dapat disesuaikan."

    # items loop
    - icon: "structure"
      title: "Fitur dokumen asli"
      content: "Tampilkan data menggunakan tabel, grafik, dan barcode."

    # items loop
    - icon: "merge"
      title: "Semua format populer"
      content: "Mendukung semua format dokumen yang umum digunakan."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Hasilkan laporan yang kustomisasi dengan baik"
  description: "GroupDocs.Assembly contoh kode"
  items:
    # code sample loop
    - title: "Menggunakan Barcode yang Dihasilkan"
      content: |
       GroupDocs.Assembly memungkinkan markup barcode dalam template laporan. Saat membuat laporan, sebuah barcode dihasilkan berdasarkan markup dan data yang disediakan. Tentukan path ke template yang berisi teks, objek data, dan markup. Juga, tentukan sumber data untuk mengisi barcode dengan konten.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Buat instance kelas DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Tentukan path ke template
            var tmp_path = "barcode_template.docx";

            //Tentukan path untuk dokumen hasil
            var res_path = "result.docx";

            //Buat instance dari datasource
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Panggil AssembleDocument untuk menghasilkan laporan
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Buat instance kelas DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Tentukan path ke template
            String tmp_path = "barcode_template.docx";

            //Tentukan path untuk dokumen hasil
            String res_path = "result.docx";

            //Buat instance dari datasource
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Panggil AssembleDocument untuk menghasilkan laporan
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // Buat instance kelas DocumentAssembler
            const assembler = new assemblyLib.DocumentAssembler();
            
            //Tentukan path ke template
            const tmp_path = "barcode_template.docx";

            //Tentukan path untuk dokumen hasil
            const res_path = "result.docx";

            //Buat instance dari datasource
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // Panggil AssembleDocument untuk menghasilkan laporan
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Mendukung lebih dari 50 format file"
  description: "GroupDocs.Assembly bekerja dengan hampir semua format file populer"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistik produk kami"
  description: "Jelajahi metrik produk untuk mendapatkan wawasan tentang kemajuan, dampak, dan pertumbuhan kami."

  items:
    # items loop
    - number: "50+"
      title: "Format yang Didukung"
      content: "Kami mendukung lebih dari 50 format dokumen yang paling banyak digunakan."

    # items loop
    - number: "650k"
      title: "Unduhan NuGet"
      content: "GroupDocs.Assembly untuk .NET adalah pustaka populer dengan lebih dari 650.000 unduhan di NuGet."

    # items loop
    - number: "18k"
      title: "Unduhan Maven"
      content: "Pengembang Java telah mengunduh GroupDocs.Assembly di Maven lebih dari 18.000 kali."

    # items loop
    - number: "150+"
      title: "Pelanggan Puas"
      content: "Produk kami dipercaya oleh pengembang individu dan perusahaan terkemuka di seluruh dunia untuk menciptakan solusi inovatif."


############################# Customers ###############################
customers:
  enable: true
  title: "Pelanggan Kami yang Puas"
  description: "Perpustakaan GroupDocs digunakan oleh beberapa merek paling terkenal dan dihormati di seluruh dunia."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Siap untuk Memulai?"
  description: "Uji fitur GroupDocs.Assembly secara gratis di platform Anda."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Pertanyaan yang Sering Diajukan"
  description: "Jelajahi Pertanyaan yang Sering Diajukan kami."

  items:
    # items loop
    - question: "Apakah GroupDocs.Assembly memerlukan pustaka eksternal untuk menyusun dokumen?"
      answer: "Tidak, GroupDocs.Assembly bekerja secara independen dan tidak memerlukan pustaka pihak ketiga seperti Adobe Acrobat atau Microsoft Office."

    # items loop
    - question: "Bisakah saya menguji fitur GroupDocs.Assembly sebelum membeli?"
      answer: "Ya, Anda bisa! GroupDocs.Assembly menawarkan uji coba gratis. Instal dan eksplor fitur-fiturnya. Versi percobaan menambahkan 'badge percobaan' ke dokumen Anda dan hanya memproses 3 halaman pertama. Untuk pengalaman penuh, dapatkan lisensi sementara gratis selama 30 hari untuk mengakses semua fitur. Detail lebih lanjut tersedia di [lisensi sementara](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Jenis lisensi apa yang tersedia?"
      answer: "Mencari lisensi GroupDocs.Assembly? Kami menawarkan berbagai pilihan yang sesuai dengan kebutuhan Anda. Pilih berdasarkan ukuran tim, lokasi penerapan (kantor tunggal atau jarak jauh), dan apakah Anda perlu membagikan SDK/API dengan klien untuk distribusi. Sebagai alternatif, pilih lisensi penggunaan bulanan dengan rencana terukur—bayar hanya untuk apa yang Anda gunakan. Temukan opsi terbaik untuk Anda di [harga](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "API Low-Code GroupDocs.Assembly"
  description: "Hasilkan dokumen menggunakan aplikasi Anda melalui REST API berbasis cloud kami."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Gunakan API RESTful cURL untuk menambahkan data ke Word, Excel, PowerPoint, dan banyak template lainnya."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Tingkatkan aplikasi .NET Anda dengan menghasilkan laporan melalui Cloud SDK. Tampilkan data bisnis dalam format kustom Anda."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "SDK GroupDocs.Assembly menawarkan berbagai opsi untuk aplikasi Java untuk menghasilkan berbagai jenis dokumen."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Aplikasi Web GroupDocs.Assembly"
  description: "GroupDocs.Assembly menawarkan aplikasi web gratis untuk menghasilkan dokumen. Anda dapat memproses lebih dari 50 format file populer langsung di browser Anda, GRATIS."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Hasilkan laporan dalam format Excel, Word, PowerPoint, dan banyak jenis file lainnya langsung dari browser web Anda."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Buat dokumen Microsoft Word dari template dan sumber data."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Unggah template dan sumber data untuk menghasilkan laporan Excel secara gratis."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---