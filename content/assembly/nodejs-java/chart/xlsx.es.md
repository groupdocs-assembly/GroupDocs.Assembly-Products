



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: es
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Inserta Gráficos en Archivos XLSX con JavaScript"
head_description: "Con GroupDocs.Assembly for Node.js via Java, los desarrolladores pueden crear y agregar rápidamente gráficos dinámicos a documentos utilizando fuentes de datos en vivo."

############################# Header ############################
title: "Agrega Gráficos a Archivos XLSX Usando Node.js" 
description: "GroupDocs.Assembly for Node.js via Java simplifica el proceso de integrar gráficos en documentos XLSX con entrada de datos en tiempo real."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Empieza Gratis Hoy"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Resumen de GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) es una solución robusta para crear documentos y reportes automatizados. Agrega gráficos, tablas, imágenes, códigos de barras y listas a archivos con precisión. Esta versátil plataforma soporta más de 50 formatos, incluyendo PDFs, documentos de Office y correos electrónicos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para Agregar un Gráfico a un Documento XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita la incorporación de gráficos a archivos XLSX. Elige entre tipos de gráficos como barras, líneas o circulares.
      
      1. Diseña una plantilla XLSX con marcadores de posición para gráficos.
      2. Carga datos desde una fuente soportada.
      3. Configura las opciones del gráfico, incluyendo tipo, colores y etiquetas.
      4. Exporta el documento con el gráfico incrustado.
   
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
        // Incluye esta etiqueta en tu plantilla para generar un gráfico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifica la ruta del archivo de plantilla
        const template = "chart_template.xlsx";

        // Extrae datos de tu sistema de origen
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Guarda el documento final con el gráfico incrustado
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Incorpora Gráficos Sin Esfuerzo en Tus Documentos"
  description: "GroupDocs.Assembly for Node.js via Java permite generar documentos ricos en características en tipos de archivos populares. Utiliza plantillas para agregar gráficos, tablas, códigos de barras, listas, imágenes y más, con actualizaciones de datos en tiempo real."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Características Principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Transforma Datos en Gráficos Profesionales"
      content: "Convierte datos de fuentes como JSON, XML o CSV en gráficos de alta calidad que pueden ser incrustados directamente en documentos."

    # feature loop
    - title: "Crea Visuales Impresionantes"
      content: "Genera gráficos de barras, gráficos circulares y gráficos de líneas que funcionan a la perfección con otros elementos del documento como imágenes, tablas y códigos de barras."

    # feature loop
    - title: "Estilo y Posicionamiento de Gráficos Flexibles"
      content: "Utiliza plantillas LINQ para controlar la ubicación y el estilo de los gráficos, incluyendo colores, diseños y etiquetas, para una presentación pulida."

    # feature loop
    - title: "Soporta Muchos Formatos de Archivo"
      content: "Genera documentos en formatos como MS Office, PDF, OpenOffice y HTML, con gráficos perfectamente integrados para un acabado profesional."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Generar e Insertar Gráficos Dinámicamente"
      content: |
        Este ejemplo ilustra cómo crear e incrustar gráficos en archivos XLSX de manera programática.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Configura una plantilla con un marcador de posición para el gráfico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Define la ruta al archivo de plantilla
          const template = "table_template.xlsx";

          // Recupera datos de una fuente elegida
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Prepara un objeto de datos que contenga la información del gráfico
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Elige el tipo de gráfico y personaliza su apariencia
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Inicializa DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Guarda el documento actualizado con el gráfico incrustado
          asm.assembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Descubre Características Avanzadas"
    exclude: "chart"
    description: "Esta plataforma simplifica la creación de documentos con herramientas diseñadas para la visualización de datos e integración seamless."
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
    title: "Genera Informes en Múltiples Formatos de Archivo"
    exclude: "XLSX"
    description: "Node.js via Java soporta más de 50 formatos, facilitando la combinación de plantillas con datos para producir documentos pulidos."
    items: 
          
        # format loop 1
        - name: "Gráficos en PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Gráficos en DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Gráficos en PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Gráficos en XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---