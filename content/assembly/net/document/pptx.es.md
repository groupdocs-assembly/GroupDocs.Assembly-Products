



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: es
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Incruste un documento en otro en PPTX con la API C#"
head_description: "Combina documentos PPTX utilizando C#. Con GroupDocs.Assembly, fusiona archivos sin problemas en solo unos pocos pasos."

############################# Header ############################
title: "Combina documentos en formato PPTX" 
description: "Con GroupDocs.Assembly for .NET, puedes incrustar rápidamente un documento PPTX dentro de otro. Esta API proporciona herramientas robustas para una fusión precisa de documentos."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) es una herramienta poderosa para la composición y manipulación de documentos. Permite a los usuarios incrustar un documento en otro, facilitando la fusión de contenido de manera fluida. Con soporte para más de 50 formatos, incluidos archivos PDF, MS Office y más, puedes organizar, editar y personalizar la salida final según tus necesidades.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo fusionar un documento en un archivo PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) te permite incrustar un documento dentro de otro archivo PPTX sin complicaciones. Fusiona y personaliza contenido fácilmente.
      
      1. Diseña una plantilla PPTX con marcadores de posición para el documento incrustado.
      2. Define la ruta del archivo para la plantilla.
      3. Especifica la ruta del archivo del documento a incrustar.
      4. Guarda el archivo final con el contenido incrustado.
   
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
        // Agrega esta etiqueta a tu plantilla para marcar el punto de inserción
        // <<doc [doc_expression]>>

        // Especifica la ruta del archivo para la plantilla
        string template = "doc_template.pptx";

        // Proporciona la ruta del documento a incrustar
        DataSourceInfo data 
            = new DataSourceInfo("insert.pptx", "doc_expression");

        // Guarda el documento fusionado
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimiza la fusión de documentos con herramientas avanzadas"
  description: "La biblioteca GroupDocs.Assembly for .NET simplifica la incorporación de un documento dentro de otro, soportando varios formatos de archivo y ofreciendo opciones de personalización para una integración fluida."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Características Clave de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera informes a partir de tus datos empresariales"
      content: "Puebla automáticamente documentos con datos de JSON, XML, CSV u otras fuentes, asegurando flujos de trabajo precisos y eficientes."

    # feature loop
    - title: "Enriquece documentos con elementos visuales"
      content: "GroupDocs.Assembly te permite incluir tablas, gráficos y listas, así como texto, enlaces, imágenes y códigos de barras generados dinámicamente."

    # feature loop
    - title: "Coloca y da formato a los datos con precisión"
      content: "Las plantillas basadas en LINQ te dan control sobre la ubicación de los datos, te permiten manejar bucles para arreglos y permiten estilos como la personalización de colores."

    # feature loop
    - title: "Funciona con múltiples formatos de archivo"
      content: "Incrusta fácilmente documentos dentro de otros en formatos como MS Office, PDFs, HTML, OpenOffice y más."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo incrustar una imagen en un documento programáticamente"
      content: |
        Este ejemplo demuestra cómo insertar una imagen en un documento PPTX utilizando GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Agrega una etiqueta de marcador de posición en tu plantilla
          // <<image [expression]>>

          // Especifica la ruta del archivo para la plantilla
          string template = "template.pptx";

          // Establece la ruta al archivo de imagen
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inicializa una instancia de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarda el documento con la imagen incrustada
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Descubre nuestras herramientas poderosas"
    exclude: "document"
    description: "Explora las características que GroupDocs.Assembly ofrece para incrustar y fusionar documentos con precisión."
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
    title: "Fusiona documentos en varios formatos"
    exclude: "PPTX"
    description: "Con la API .NET, puedes combinar documentos en más de 50 formatos soportados. Incrusta archivos o secciones sin esfuerzo en tus documentos finales."
    items: 
          
        # format loop 1
        - name: "Incorporar un documento en un PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Incorporar un documento en un DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Incorporar un documento en un PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Incorporar un documento en un XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---