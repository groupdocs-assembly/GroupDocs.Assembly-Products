



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: es
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Combina Documentos en PDF con JavaScript"
head_description: "Combina archivos PDF utilizando JavaScript. GroupDocs.Assembly simplifica la fusión de documentos en solo unos pocos pasos."

############################# Header ############################
title: "Combina Contenido en Archivos PDF de Forma Eficiente" 
description: "Con GroupDocs.Assembly for Node.js via Java, integrar un archivo PDF en otro es rápido y preciso. Disfruta de herramientas flexibles y confiables para una fusión sin complicaciones."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prueba Gratis"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Descripción General de GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) ofrece una forma potente de gestionar documentos. Combina un archivo en otro fácilmente mientras soporta más de 50 formatos, como PDF y MS Office. Personaliza diseños, edita contenido y organiza documentos exactamente como los necesitas.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo Fusionar un Documento en un Archivo PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita la inserción de un archivo PDF en otro con opciones personalizables.
      
      1. Diseña una plantilla con marcadores de posición para contenido incrustado (las plantillas PDF no son compatibles).
      2. Establece la ruta del archivo para la plantilla.
      3. Proporciona la ruta del archivo para el documento a fusionar.
      4. Guarda el documento completado con el contenido fusionado como un archivo PDF.
   
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
        // Inserta esta etiqueta en tu plantilla para definir dónde se incrustará el documento
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Establece la ruta del archivo para la plantilla principal
        // Actualmente, las plantillas PDF no son compatibles.
        const template = "doc_template.docx";

        // Proporciona la ruta para el documento que deseas fusionar
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // Guarda la salida final con el documento incrustado
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Herramientas Potentes para la Integración de Documentos"
  description: "GroupDocs.Assembly for Node.js via Java facilita la inserción de archivos en varios formatos y es completamente personalizable. Ofrece resultados consistentes y profesionales en cada ocasión."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Características Clave de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera Informes con Datos Empresariales"
      content: "Extrae datos de fuentes JSON, XML o CSV para crear informes y documentos completos de manera rápida y precisa."

    # feature loop
    - title: "Añade Elementos Visuales Ricos"
      content: "GroupDocs.Assembly te permite incluir tablas, gráficos, listas, imágenes y códigos de barras junto con texto y enlaces."

    # feature loop
    - title: "Colocación Precisa de Datos"
      content: "Utiliza plantillas LINQ para posicionar datos exactamente donde pertenecen, maneja elementos repetidos como arreglos y personaliza estilos con facilidad."

    # feature loop
    - title: "Trabaja con una Variedad de Formatos"
      content: "Fusiona contenido sin problemas entre formatos como PDFs, archivos de MS Office, HTML y OpenOffice, ofreciendo flexibilidad para todos los proyectos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Incrustar una Imagen en un Documento Programáticamente"
      content: |
        Este ejemplo muestra cómo insertar una imagen en un archivo PDF utilizando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Añade un marcador de posición en la plantilla para la imagen
          // <<image [expression]>>

          // Especifica la ruta al archivo de la plantilla
          // Actualmente, las plantillas PDF no son compatibles.
          String template = "template.docx";
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Establece la ruta a la imagen que deseas incrustar
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Inicializa el objeto DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Guarda el documento con la imagen incluida
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_document.pdf"
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
    title: "Características Clave de un Vistazo"
    exclude: "document"
    description: "Explora las herramientas completas que GroupDocs.Assembly ofrece para una fusión de documentos eficiente y fluida."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Combina Documentos en Muchos Formatos"
    exclude: "PDF"
    description: "Usa Node.js via Java para fusionar contenido en más de 50 formatos de archivo, asegurando resultados profesionales y pulidos."
    items: 
          
        # format loop 1
        - name: "Incorporar un documento en un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Incorporar un documento en un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Incorporar un documento en un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Incorporar un documento en un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---