



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: es
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generar listas en documentos XLSX con C#"
head_description: "La API GroupDocs.Assembly for .NET permite a los desarrolladores crear e incrustar dinámicamente listas llenas de datos en documentos y plantillas."

############################# Header ############################
title: "Agrega listas impulsadas por datos a documentos XLSX usando nuestra API .NET" 
description: "GroupDocs.Assembly for .NET ofrece herramientas potentes para generar e incrustar listas dinámicamente en documentos XLSX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Prueba Gratuita"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Visión general de GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) está diseñado para optimizar la creación de documentos e informes mediante la integración fluida de datos de diversas fuentes. Rellena plantillas con listas, gráficos, tablas, códigos de barras o texto, y coloca el contenido con precisión utilizando un marcado avanzado. Con soporte para más de 50 formatos, incluidos PDFs, archivos de MS Office y correos electrónicos, es ideal para automatizar flujos de trabajo de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para añadir una lista llenada de datos a un documento XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilita la inserción de listas impulsadas por datos en plantillas XLSX. Crea y personaliza listas de manera efectiva.
      
      1. Prepara una plantilla XLSX con marcadores de posición para la lista.
      2. Establece la ruta a la plantilla.
      3. Recupera datos de fuentes compatibles como JSON o XML.
      4. Guarda el documento final con la lista incrustada.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de ejemplo"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Agrega esta etiqueta a tu plantilla para marcar dónde aparecerá la lista
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Especifica la ruta al archivo de la plantilla
        string template = "list_template.xlsx";

        // Recupera datos de tu fuente elegida
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Guarda el documento con la lista generada
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Crea documentos rellenando plantillas con datos estructurados"
  description: "GroupDocs.Assembly for .NET simplifica la construcción de documentos impulsados por datos. Agrega listas, tablas, códigos de barras, gráficos, imágenes y otros elementos dinámicamente con plantillas avanzadas."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Funciones de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Generar informes a partir de datos empresariales"
      content: "La API pobla documentos en formatos populares utilizando datos de fuentes como JSON, XML, CSV, etc., con precisión y eficiencia."

    # feature loop
    - title: "Utiliza listas y otros elementos para presentar datos"
      content: "GroupDocs.Assembly te permite incrustar listas, tablas y gráficos junto con texto, códigos de barras, hiperenlaces e imágenes para crear documentos bien estructurados."

    # feature loop
    - title: "Inserta datos precisamente donde se necesiten"
      content: "Aprovecha la sintaxis basada en LINQ para posicionar listas y otros elementos de datos con precisión. Usa bucles para poblar listas dinámicamente y aplica formato personalizado de manera programática."

    # feature loop
    - title: "Soporta múltiples formatos de documentos"
      content: "Genera y gestiona documentos en varios formatos como MS Office, OpenOffice, PDF, HTML y archivos de correo electrónico. Integra fácilmente múltiples documentos en uno."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo generar una lista dinámicamente"
      content: |
        Este ejemplo demuestra cómo incrustar una lista generada dinámicamente en un documento XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Agrega una etiqueta de marcador de posición a tu plantilla para la lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Especifica la ruta al archivo de la plantilla
          string template = "numlist_template.xlsx";

          // Recupera los datos para poblar la lista
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Crea un objeto de origen de datos con la información necesaria
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inicializa DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarda el documento final con la lista generada
          asm.AssembleDocument(template, "result.xlsx", data);
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Descargar el resultado"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.xlsx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Explora las funciones de GroupDocs.Assembly de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descargar desde Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Conocer sobre la licencia"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explora capacidades clave"
    exclude: "list"
    description: "Nuestra plataforma está construida para simplificar la creación y la integración del contenido de documentos impulsados por datos."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crea documentos estructurados en formatos populares"
    exclude: "XLSX"
    description: ".NET soporta más de 50 formatos, lo que te permite fusionar datos y plantillas sin problemas para obtener resultados estructurados y pulidos."
    items: 
          
        # format loop 1
        - name: "Crear una lista en un PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Crear una lista en un DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Crear una lista en un PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Crear una lista en un XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---