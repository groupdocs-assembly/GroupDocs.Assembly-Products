



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: es
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Agregar Códigos de Barras a Archivos XLSX Usando JavaScript"
head_description: "Genera e incrusta códigos de barras en tus documentos y correos electrónicos con la API de GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Crear Códigos de Barras para Archivos XLSX Usando Node.js" 
description: "Con GroupDocs.Assembly for Node.js via Java, puedes generar, personalizar e incrustar dinámicamente códigos de barras en documentos XLSX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comienza Ahora"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introducción a GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) te permite crear documentos profesionales combinando datos de múltiples fuentes. Agrega gráficos, tablas, listas, imágenes y códigos de barras a tus archivos. Utiliza plantillas para organizar el contenido exactamente donde corresponde. Funciona con más de 50 formatos, incluidos PDFs, documentos de Office y correos electrónicos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para Agregar un Código de Barras en Archivos XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita la inserción de códigos de barras en documentos XLSX. Soporta más de 60 tipos de códigos de barras, incluidos formatos 1D y 2D.
      
      1. Crea una plantilla XLSX con marcadores de posición para los códigos de barras.
      2. Recupera datos de una fuente compatible.
      3. Configura las opciones del código de barras, como tamaño y resolución.
      4. Guarda el documento final con el código de barras incrustado.
   
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
        // Usa esta etiqueta en la plantilla para incluir un código de barras en el documento de salida
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifica la ruta al archivo de plantilla
        const template = "barcode_template.xlsx";

        // Carga los datos requeridos desde tu fuente
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Guarda el documento con el código de barras aplicado
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Generar Documentos con Plantillas Basadas en Datos"
  description: "Con GroupDocs.Assembly for Node.js via Java, puedes crear archivos profesionales en formatos populares mediante la inclusión fluida de gráficos, tablas, listas, enlaces, imágenes y códigos de barras."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Características Principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Construir Informes con Datos Empresariales"
      content: "Utiliza la API para rellenar plantillas con datos de formatos como JSON, XML y CSV de manera rápida y precisa."

    # feature loop
    - title: "Agregar Elementos Visuales"
      content: "GroupDocs.Assembly permite la inserción de elementos como gráficos, tablas, listas, texto, enlaces, imágenes y códigos de barras en tiempo real."

    # feature loop
    - title: "Controlar la Ubicación de los Datos"
      content: "Con plantillas basadas en LINQ, puedes posicionar datos con precisión, iterar sobre arreglos y aplicar formato personalizado programáticamente."

    # feature loop
    - title: "Compatible con Muchos Formatos"
      content: "Trabaja con archivos como documentos de MS Office, PDFs, HTML, archivos de OpenOffice y correos electrónicos. Combina múltiples documentos cuando sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ejemplo: Generar un Código de Barras Programáticamente"
      content: |
        Este ejemplo demuestra cómo generar e insertar programáticamente un código de barras en un documento XLSX.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Diseña una plantilla con un marcador de posición para el código de barras
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifica la ruta del archivo de plantilla
          const template = "barcode_template.xlsx";

          // Recupera datos desde tu fuente
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Crea un objeto fuente de datos con los detalles requeridos
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Inicializa una instancia de DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Configura la configuración del código de barras
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Guarda el documento con el código de barras incluido
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.xlsx"
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
    title: "Explora Características Clave"
    exclude: "barcode"
    description: "Simplifica el procesamiento de documentos con herramientas avanzadas y capacidades de automatización."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formatos de Archivo Soportados para la Creación de Informes"
    exclude: "XLSX"
    description: "Node.js via Java maneja más de 50 tipos de archivos, facilitando la combinación de datos y el procesamiento de plantillas para obtener resultados de alta calidad."
    items: 
          
        # format loop 1
        - name: "Agregar un código de barras a un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Agregar un código de barras a un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar un código de barras a un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Agregar un código de barras a un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---