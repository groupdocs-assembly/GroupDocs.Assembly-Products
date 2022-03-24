---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API para automatización de documentos, ensamblaje y generación de informes"
head_description: "C# .NET API de generación de informes, ensamblaje y automatización de documentos. Cree documentos PDF Word Excel PPTX HTML y de correo electrónico a partir de plantillas personalizadas."

############################# Header ############################
title: ".NET Automatización de documentos y API de generación de informes"
description: "Genere informes en aplicaciones .NET definiendo plantillas y fusionando los datos."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "/border/groupdocs-assembly-net.svg"
        product: "GroupDocs.Assembly"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Visión de conjunto"

            # button loop
            - link: "#features"
              text: "Características"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/assembly"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly para .NET API lo ayuda a crear potentes aplicaciones de automatización de documentos y generación de informes con capacidades para generar informes a partir de plantillas personalizadas en C#, ASP.NET y otras aplicaciones relacionadas con .NET. Con solo unas pocas líneas de código, la biblioteca de informes de .NET reúne de manera inteligente los datos proporcionados a partir de la plantilla de documento definida y genera hermosos informes en el formato de salida preferido al obtener datos de varias fuentes de datos (bases de datos, XML, JSON, ODATA, CSV, Objetos .NET personalizados).

      Es compatible con la sintaxis de plantilla basada en LINQ y los usuarios pueden generar fácilmente documentos de salida en todos los formatos de archivos comerciales comúnmente utilizados, como PDF, HTML, correo electrónico de Outlook, oficina de Microsoft Word, hojas de cálculo de Excel, presentaciones de PowerPoint y diapositivas. Las propiedades de formato de los elementos de la plantilla también se pueden configurar mediante la manipulación de texto, HTML y bloques condicionales, imágenes, gráficos, códigos de barras, hipervínculos, tablas dinámicas, etc.

      GroupDocs.Assembly para .NET se puede utilizar para desarrollar aplicaciones en cualquier entorno de desarrollo que se dirija a la plataforma .NET. Es compatible con todos los lenguajes basados en .NET y es compatible con los sistemas operativos más populares (Windows, Linux, MacOS) donde se pueden instalar marcos Mono o .NET (incluido .NET Core).
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Assembly para .NET:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Visión de conjunto"
          content: |
            * Formulación de datos
            * Formateo de datos
            * Automatización de datos
            * Crear plantilla
            * Formato de elemento de plantilla
            * La generación del informe
      
      ## TAB TWO ##
      tab_two:
        description: |
          Los [formatos de archivo de documento] admitidos (https://docs.groupdocs.com/assembly/net/supported-document-formats/) para la API de generación de documentos .NET se enumeran a continuación.

        left:
          enable: true
          table:
            # table loop
            - title: "Formatos de oficina de Microsoft"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML (XML)
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML (XML)
                * **PowerPoint**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **Outlook**: EML, EMLX, MSG, MHT

            # table loop
            - title: "Fuentes de datos admitidas"
              content: |
                * Base de datos
                * XML
                * OData
                * JSON
                * CSV
                * Objetos .NET personalizados
                * Hoja de cálculo como tabla de datos
                * Tabla de procesamiento de textos como tabla de datos

        right:
          enable: true
          table:
            # table loop
            - title: "Otros formatos"
              content: |
                * **OpenOffice Document Formats**: ODT, OTT, ODS, ODP
                * **Email**: MHT, MHTML
                * **Web**: HTML
                * **Markdown Documentación File**: MD
                * **Other**: TXT

            # table loop
            - title: "Compatibilidad con montaje entre formatos"
              content: |
                * Word Processing **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * Spreadsheet **TO** Spreadsheet, HTML, PDF, XPS, TIFF, MHTML
                * Presentation **TO** Presentation, HTML, PDF, XPS, TIFF
                * Email **TO** Word Processing, Email, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML & TXT **TO** Word Processing, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Assembly for .NET apoya siguiendo Sistemas operativos, Frameworks & Gerente de empaquetacións:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * .NET Framework 2.0 o superior
                * Mono Framework 1.2 o superior

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Gerente de empaquetación"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entornos de desarrollo"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Características ############################
features:
    enable: true
    title: "Características de GroupDocs.Assembly para .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Funciona con múltiples formatos de datos"

      # feature loop
      - icon: "fas fa-eye"
        content: "Capaz de manipular datos usando fórmulas y operaciones de datos secuenciales"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Cadenas de formato en la sintaxis de la plantilla para que sean Superior, Inferior, Capital, Primera mayúscula"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Realizar formato numérico ordinal, cardinal y alfabético en la sintaxis de plantilla"

      # feature loop
      - icon: "fas fa-code"
        content: "Definir variables en documentos de plantilla y comentarios de texto de soporte dentro de etiquetas de sintaxis de plantilla"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Inserte dinámicamente el contenido de los documentos externos en sus informes"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Genere dinámicamente una imagen de código de barras en informes y establezca el color de fondo para documentos HTML"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Asigne atributos dinámicamente al cuerpo del mensaje de correo electrónico e inserte hipervínculos en los informes"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Crear archivos adjuntos de mensajes de correo electrónico de forma dinámica"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Compatibilidad con el campo NEXT analógico de Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Actualizar campos al ensamblar documentos de procesamiento de texto"

      # feature loop
      - icon: "fas fa-columns"
        content: "Calcule la fórmula mientras ensambla documentos de hoja de cálculo"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Formato numérico, texto, imagen, gráfico, elementos de fecha y hora de la plantilla"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Cargar y guardar formatos de documentos de presentación POT y OTP ensamblados"

      # feature loop
      - icon: "fas fa-print"
        content: "Use la sintaxis basada en LINQ para la plantilla y realice el formato de texto condicional de los elementos de la plantilla"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Cambiar el formato de archivo del documento ensamblado usando la extensión de archivo o especificaciones explícitas"

      # feature loop
      - icon: "fas fa-lock"
        content: "Lista ordenada admitida para Markdown: guarde correos electrónicos y documentos de Word recién ensamblados en Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Admite informes de numerosos tipos, por ejemplo, gráficos, listas, tablas, imágenes y más"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Errores de sintaxis de plantilla en línea en documentos generados en lugar de lanzamiento de excepciones"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Cargue documentos de plantilla desde HTML con recursos y guarde Word, Excel, PowerPoint y correos electrónicos ensamblados en HTML con recursos"

      # feature loop
      - icon: "fas fa-heading"
        content: "Agregue dinámicamente la numeración de la lista de reinicio en formatos de documentos de Word y correo electrónico con cuerpos HTML y RTF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Inserte dinámicamente imágenes y documentos desde bytes codificados en Base64 and adjust checkbox value settings of Word documents"

      # feature loop
      - icon: "fas fa-cube"
        content: "Estire la imagen en el cuadro de texto de Word, Excel, presentaciones y correos electrónicos mientras conserva la relación de imagen"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Agregue dinámicamente enlaces y marcadores a formatos de documentos y asigne nombres a los rangos de celdas de las hojas de cálculo de Excel"

    more_feature:
      # more_feature_loop
      - title: "Soporte para elementos de plantilla"
        content: |
          GroupDocs.Assembly para .NET API le brinda control para trabajar con numerosos elementos de plantilla. Puede trabajar con bloques de texto formateado, bloques HTML, imágenes, gráficos, hipervínculos y códigos de barras (a través de fuentes de código de barras). Los bloques repetidos y los bloques condicionales también son compatibles, incluidos los elementos de la lista y las filas de la tabla. También puede fusionar dinámicamente celdas de tablas que contengan el mismo texto en función de expresiones de plantilla para hojas de cálculo, presentaciones, documentos y correos electrónicos con cuerpos HTML y RTF.

      # more_feature_loop
      - title: "Trabajar con informes de lista"
        content: |
          Usando GroupDocs.Assembly para .NET API, puede trabajar con informes de lista de los siguientes tres tipos:

          * Lista con viñetas
          * Lista numerada
          * Colored Lista numerada

      # more_feature_loop
      - title: "Trabajar con informes de gráficos"
        content: |
          GroupDocs.Assembly para .NET admite el siguiente tipo de informes de gráficos:

          * Gráfico de burbujas, que muestra tres dimensiones de datos
          * Gráfico de columnas
          * Gráfico circular
          * Gráfico de dispersión
          * Gráfico de series (a color)

      # more_feature_loop
      - title: "Trabajar con informes de tablas"
        content: |
          GroupDocs.Assembly para .NET admite los siguientes tipos de informes de tabla:

          * Tabla maestro-detalle
          * Tabla con filas resaltadas
          * Tabla con contenido alternativo
          * Tabla con Filtrado, Agrupación y Ordenación
          
          También puede usar las bandas de datos en las filas de la tabla.

      # more_feature_loop
      - title: "Integración fácil"
        content: |
          Puede integrar fácilmente GroupDocs.Assembly para la API de .NET con su aplicación de .NET usando solo unas pocas líneas de código. El siguiente es un código de ejemplo para generar un informe en un documento abierto format:

          ```cs
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Assembly ofrece API de visualización de documentos para otros entornos de desarrollo populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Assembly for Java"
          image: "/border/groupdocs-assembly-java.svg"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
