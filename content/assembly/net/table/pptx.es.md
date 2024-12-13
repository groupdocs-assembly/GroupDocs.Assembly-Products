



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: es
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Crea tablas en documentos PPTX con C#"
head_description: "La API GroupDocs.Assembly for .NET permite a los desarrolladores añadir y llenar tablas en documentos y correos electrónicos con datos de fuentes dinámicas."

############################# Header ############################
title: "Genera tablas de datos en documentos PPTX utilizando nuestra API .NET" 
description: "GroupDocs.Assembly for .NET permite llenar dinámicamente tablas en documentos PPTX con datos de diversas fuentes."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Prueba Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Visión general de GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) está diseñado para crear documentos e informes llenando plantillas con datos de múltiples fuentes. Inserta datos estructurados en tablas, listas y gráficos sin esfuerzo, o incrusta imágenes de manera dinámica. La sintaxis avanzada asegura una colocación precisa de los datos. Soporta más de 50 formatos, incluidos PDFs, documentos de MS Office y archivos de correo electrónico.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo llenar una tabla en un documento PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) te permite llenar dinámicamente tablas en plantillas para formatos como PPTX. Inserta datos de diversas fuentes en tus tablas.
      
      1. Crea una plantilla PPTX con marcadores de posición para la tabla.
      2. Obtén datos de cualquier fuente soportada.
      3. Filtra los datos para incluir solo la información necesaria.
      4. Guarda el documento con la tabla poblada.
   
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
        // Añade estas etiquetas en una fila de plantilla de tabla
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Establece la ruta del archivo para la plantilla
        string template = "table_template.pptx";

        // Obtén datos de una fuente soportada
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Guarda el documento con la tabla llena de datos
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Genera documentos con tablas dinámicas"
  description: "GroupDocs.Assembly for .NET optimiza la creación de documentos al automatizar el llenado de tablas y soportar elementos adicionales como gráficos, listas e imágenes a través de plantillas y marcado avanzado."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Características Clave de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crea informes a partir de datos estructurados"
      content: "La API procesa datos de fuentes como JSON, XML y CSV para llenar tablas en documentos de oficina de manera eficiente y precisa."

    # feature loop
    - title: "Visualiza los datos"
      content: "GroupDocs.Assembly permite la creación de tablas, listas y gráficos, además de incrustar texto, enlaces e imágenes para un diseño profesional de documentos."

    # feature loop
    - title: "Posiciona datos de tabla con precisión"
      content: "Utiliza sintaxis basada en LINQ para añadir dinámicamente filas y columnas a las tablas. Personaliza estilos, incluidos colores y formatos, programáticamente."

    # feature loop
    - title: "Soporta una amplia variedad de formatos"
      content: "Maneja sin problemas formatos de archivo populares como MS Office, OpenOffice, PDF y HTML. Inserta tablas pobladas en tipos de documentos soportados sin complicaciones."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo llenar dinámicamente una tabla de datos"
      content: |
        Este ejemplo demuestra cómo llenar una tabla en un documento PPTX utilizando datos dinámicos.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepara una plantilla con un marcador de posición para la tabla
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Especifica la ruta del archivo para la plantilla
          string template = "table_template.pptx";

          // Recupera datos de tu fuente elegida
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crea un objeto fuente de datos con los datos necesarios
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Inicializa DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarda el documento completado con la tabla poblada
          asm.AssembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "Explora características clave"
    exclude: "table"
    description: "Nuestra solución simplifica la creación de documentos profesionales con tablas pobladas dinámicamente y elementos adicionales."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crea informes con tablas detalladas"
    exclude: "PPTX"
    description: ".NET permite la creación de informes comprensivos llenando plantillas con tablas y otros elementos de datos en más de 50 formatos soportados."
    items: 
          
        # format loop 1
        - name: "Agregar una tabla a un PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Agregar una tabla a un DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar una tabla a un PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Agregar una tabla a un XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---