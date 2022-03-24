---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de generador de informes dinámicos y ensamblaje de automatización de documentos de Java"
head_description: "API de Java para automatización de documentos, ensamblaje e informes. Cree informes a partir de plantillas personalizadas. Ensamble PDF Word Excel PPTX HTML de fuentes de datos DB, JSON, OData y XML."

############################# Header ############################
title: "API de Java para automatizar documentos e informes"
description: "Crear aplicaciones de automatización de documentos para obtener datos; colóquelo en plantillas personalizables y genere informes dinámicos a través de la API de Java."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "/border/groupdocs-assembly-java.svg"
        product: "GroupDocs.Assembly"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Assembly for Java API lo ayuda a desarrollar rápidamente aplicaciones de informes y automatización de documentos en Java para generar informes personalizados a partir de plantillas sin instalar ningún software externo. El motor de generación de informes obtiene datos del documento de plantilla, los ensambla y genera informes en el formato de salida especificado de acuerdo con la sintaxis definida. Le permite configurar e insertar propiedades de formato de elementos de plantilla de forma dinámica y admite varias fuentes de datos (JSON, XML, OData, bases de datos, CSV, hoja de cálculo como tabla de datos, tabla de procesamiento de texto como tabla de datos y bases de datos) para recuperar datos.

      La biblioteca de ensamblaje de documentos reconoce múltiples formatos de documentos y le permite crear plantillas en todos los tipos de archivos admitidos, como PDF, HTML, correo electrónico de Outlook, oficina de Microsoft Word, hojas de cálculo de Excel, presentaciones de PowerPoint y texto. Es compatible con la sintaxis de plantilla basada en LINQ y los usuarios también pueden configurar e insertar propiedades de formato de elementos de plantilla de forma dinámica.

      GroupDocs.Assembly para Java es fácil de integrar con aplicaciones Java nuevas o existentes. Es altamente compatible con todas las versiones de Java y es compatible con los sistemas operativos más populares (Windows, Linux, MacOS) que pueden ejecutar el tiempo de ejecución de Java.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Assembly para Java:

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
          Los [formatos de archivo de documento admitidos](https://docs.groupdocs.com/assembly/java/supported-document-formats/) para la API de generación de documentos de Java se enumeran a continuación.

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
          GroupDocs.Assembly for Java supports following Sistemas operativos, Frameworks & Gerente de empaquetacións:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * Java 7 (1.7) y superior

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entornos de desarrollo"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Herramienta de automatización de compilación"
              content: |
                * Maven

############################# Características ############################
features:
    enable: true
    title: "Características de GroupDocs.Assembly para Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Ajuste la imagen en el cuadro de texto de Word, Excel, presentaciones y correos electrónicos mientras conserva la relación de imagen"

      # feature loop
      - icon: "fas fa-eye"
        content: "Usar fórmulas y realizar operaciones de datos secuenciales: aplicar fórmulas durante el ensamblaje de la hoja de cálculo"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Aplicar formato Upper, Lower, Capital, FirstCap a cadenas en la sintaxis de plantilla"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Soporte de sintaxis de plantilla Formato de naturaleza numérica ordinal, cardinal y alfabética"

      # feature loop
      - icon: "fas fa-code"
        content: "Admite documentos de plantilla con variables personalizadas y comentarios de texto dentro de etiquetas de sintaxis de plantilla"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Insertar dinámicamente el contenido del documento en el informe"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Configure dinámicamente el color de fondo de los documentos HTML y genere códigos de barras en los informes"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Inserte dinámicamente hipervínculos en informes y aplique atributos al cuerpo del mensaje de correo electrónico"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Adjunte dinámicamente archivos adjuntos de correo electrónico y actualice campos durante el ensamblaje de documentos de procesamiento de texto"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Compatibilidad con NEXT Field Analogue de Microsoft Word"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Agregue dinámicamente enlaces y marcadores a formatos de documentos y asigne nombres a los rangos de celdas de las hojas de cálculo de Excel"

      # feature loop
      - icon: "fas fa-columns"
        content: "Cargar y guardar formatos de documentos de presentación POT y OTP ensamblados"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Formato de plantilla para elementos numéricos, de texto, de imagen, de fecha y hora y de gráfico"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Inserte dinámicamente imágenes y documentos desde bytes codificados en Base64"

      # feature loop
      - icon: "fas fa-print"
        content: "Sintaxis de plantilla basada en LINQ"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Cambiar formato de archivo ensamblado usando especificaciones explícitas o extensión de archivo"

      # feature loop
      - icon: "fas fa-lock"
        content: "Lista ordenada admitida para Markdown: guarde correos electrónicos y documentos de Word recién ensamblados en Markdown"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Genere varios tipos de informes, por ejemplo, gráficos, imágenes, tablas, listas y más"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Errores de sintaxis de plantilla en línea en documentos generados en lugar de lanzamiento de excepciones"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Reinicie dinámicamente una lista numerada en documentos de Word, así como correos electrónicos con cuerpos HTML y RTF"

      # feature loop
      - icon: "fas fa-heading"
        content: "Compatibilidad con tablas, enlaces automáticos, enlaces en línea e imágenes para documentos Markdown ensamblados"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Genere dinámicamente códigos de barras (GS1-128 AI 8102 Cupón extendido y cupón UPCA y GS1 Databar"

      # feature loop
      - icon: "fas fa-cube"
        content: "Cargue documentos de plantilla desde HTML con recursos y guarde Word, Excel, PowerPoint y correos electrónicos ensamblados en HTML con recursos"

    more_feature:
      # more_feature_loop
      - title: "Manipular elementos de plantilla"
        content: |
          Manipule numerosos elementos de plantilla con GroupDocs.Assembly para la API de Java. Los elementos de plantilla con los que puede trabajar incluyen bloques de texto, imágenes, hipervínculos, bloques HTML, códigos de barras (a través de fuentes de códigos de barras) y gráficos. También puede aplicar bloques repetidos y bloques condicionales para elementos de lista y filas de tablas. Fusión dinámica de celdas de tabla que contienen el mismo texto, basada en expresiones de plantilla para documentos, presentaciones, hojas de cálculo y correos electrónicos con cuerpos HTML y RTF.
      
      # more_feature_loop
      - title: "Manipular informes de lista"
        content: |
          El uso de GroupDocs.Assembly para la API de Java admite los siguientes tipos de informes de lista:

          * Lista con viñetas
          * Lista numerada
          * Colored Lista numerada

      # more_feature_loop
      - title: "Manipular informes de gráficos"
        content: |
          GroupDocs.Assembly para Java admite el siguiente tipo de informes de gráficos:

          * Gráfico de burbujas, que muestra tres dimensiones de datos
          * Gráfico de columnas
          * Gráfico circular
          * Gráfico de dispersión
          * Gráfico de series (a color)

      # more_feature_loop
      - title: "Manipular informes de tablas"
        content: |
          GroupDocs.Assembly para Java admite los siguientes tipos de informes de tabla:

          * Tabla maestro-detalle
          * Tabla con filas resaltadas
          * Tabla con contenido alternativo
          * Tabla con Filtrado, Agrupación y Ordenación

          También puede usar las bandas de datos en las filas de la tabla.

      # more_feature_loop
      - title: "Manipular informes de gráficos"
        content: |
          La integración de GroupDocs.Assembly para la API de Java con su aplicación Java es muy sencilla. Lo que sigue es un bloque de código de ejemplo que genera un informe en formato OpenDocument usando Java: 

          ```java
          DocumentAssembler assembler = new DocumentAssembler();
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
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
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "/border/groupdocs-assembly-net.svg"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---