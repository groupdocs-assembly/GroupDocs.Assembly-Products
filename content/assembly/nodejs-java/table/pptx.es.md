



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: es
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Inserta Tablas en Documentos PPTX con JavaScript"
head_description: "Utiliza GroupDocs.Assembly for Node.js via Java para incrustar rápidamente tablas en documentos o correos electrónicos, extrayendo datos de diversas fuentes."

############################# Header ############################
title: "Agrega Tablas a Archivos PPTX sin Complicaciones con Node.js" 
description: "Con GroupDocs.Assembly for Node.js via Java, llenar tablas en documentos PPTX es directo, utilizando datos de múltiples fuentes."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comienza Tu Prueba Gratuita"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introducción a GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) es una herramienta poderosa para automatizar la creación de documentos. Te permite insertar tablas, gráficos, listas e imágenes en plantillas, con una colocación de contenido precisa. Apoyando más de 50 formatos de archivo, incluidos PDF, Word y correos electrónicos, agiliza la generación de informes y otras tareas.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo Agregar Datos a una Tabla en PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) te permite poblar rápidamente las plantillas de tabla para archivos PPTX utilizando fuentes de datos dinámicas.
      
      1. Crea una plantilla PPTX con marcadores de posición para las filas y columnas de la tabla.
      2. Carga datos desde una fuente soportada como JSON o CSV.
      3. Organiza y formatea los datos según sea necesario.
      4. Genera el documento con la tabla completada.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de ejemplo"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Incluye estas etiquetas en los marcadores de fila de tu plantilla
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifica la ruta del archivo de plantilla
        const template = "table_template.pptx";

        // Carga tus datos desde una fuente elegida
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Guarda el documento final con la tabla completada
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Agrega Tablas Basadas en Datos a Documentos"
  description: "GroupDocs.Assembly for Node.js via Java permite a los usuarios crear tablas automáticamente, mientras también incrustan gráficos, imágenes y listas utilizando flujos de trabajo basados en plantillas."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Características Principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera Tablas a Partir de Datos Estructurados"
      content: "Extrae datos de JSON, XML, CSV y otros formatos para poblar automáticamente tablas en documentos."

    # feature loop
    - title: "Crea Contenido Visual Pulido"
      content: "Utiliza GroupDocs.Assembly para diseñar tablas, gráficos y listas profesionales, y agregar enlaces, imágenes y texto para una apariencia de documento refinada."

    # feature loop
    - title: "Colocación de Contenido Dinámico en Tablas"
      content: "Añade filas y columnas programáticamente utilizando plantillas basadas en LINQ y personaliza estilos como fuentes, colores y alineación."

    # feature loop
    - title: "Funciona sin Problemas a Través de Formatos"
      content: "Crea o edita fácilmente tablas en MS Office, OpenOffice, PDF, HTML y otros formatos, integrándolas en archivos según sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo Población Programáticamente una Tabla"
      content: |
        Este ejemplo demuestra cómo llenar una tabla en un documento PPTX con datos de una fuente externa.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Diseña una plantilla con marcadores de posición para la tabla
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifica la ruta del archivo a la plantilla
          const template = "table_template.pptx";

          // Carga los datos requeridos desde tu fuente
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Organiza los datos en la estructura necesaria
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Inicializa DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Guarda el documento de salida con la tabla completada
          asm.assembleDocument(template, "result.pptx", data);
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Explora las funciones de GroupDocs.Assembly de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descargar desde NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Conocer sobre la licencia"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Características Clave a Simple Vista"
    exclude: "table"
    description: "Nuestra API automatiza la creación de tablas y mejora la generación de documentos con herramientas y plantillas versátiles."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Genera Tablas en una Variedad de Formatos"
    exclude: "PPTX"
    description: "Con Node.js via Java, pobla plantillas y crea tablas completas en más de 50 tipos de archivo soportados."
    items: 
          
        # format loop 1
        - name: "Agregar una tabla a un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Agregar una tabla a un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar una tabla a un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Agregar una tabla a un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---