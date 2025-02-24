



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: es
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Crea Listas Dinámicas en PDF con JavaScript"
head_description: "Diseña e inserta listas en plantillas de PDF utilizando la API de GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Incorpora Listas Basadas en Datos en Archivos PDF con Node.js" 
description: "GroupDocs.Assembly for Node.js via Java ofrece herramientas poderosas para añadir listas flexibles impulsadas por datos a documentos PDF."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comienza Gratis"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) simplifica la creación de documentos extrayendo datos de diversas fuentes e incorporándolos en plantillas. Úsalo para construir listas, tablas, gráficos y otros elementos, con opciones de posicionamiento y formato precisas. Soporta más de 50 formatos, incluyendo PDF, MS Office y correos electrónicos, ayudando a automatizar tu proceso de generación de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para Insertar una Lista en un Archivo PDF"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita la adición de listas detalladas y basadas en datos a tus plantillas PDF.
      
      1. Diseña una plantilla con marcadores de posición para la lista (las plantillas PDF no son soportadas).
      2. Proporciona la ruta del archivo de la plantilla.
      3. Carga datos desde fuentes compatibles como JSON o XML.
      4. Exporta el documento completado con la lista como un archivo PDF.
   
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
        // Coloca esta etiqueta en tu plantilla para marcar dónde irá la lista
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Establece la ruta del archivo para tu plantilla
        // Las plantillas PDF actualmente no son compatibles.
        const template = "list_template.docx";

        // Obtén los datos de la fuente que deseas utilizar
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Guarda el archivo con la lista incorporada
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Genera Documentos con Datos Integrados"
  description: "Con GroupDocs.Assembly for Node.js via Java, puedes incorporar listas, tablas, gráficos y otros elementos en plantillas, ahorrando tiempo y esfuerzo."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Aspectos destacados de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera Informes desde Múltiples Fuentes de Datos"
      content: "Importa datos de JSON, XML, CSV u otros formatos para rellenar listas y otros componentes de manera eficiente."

    # feature loop
    - title: "Añade Listas y Otros Elementos Visuales"
      content: "GroupDocs.Assembly te permite incorporar sin problemas listas, tablas, gráficos y más junto a texto, imágenes y enlaces para obtener resultados pulidos."

    # feature loop
    - title: "Coloca y Estiliza Datos con Precisión"
      content: "Las plantillas basadas en LINQ te permiten controlar exactamente dónde aparecen las listas y otros datos, usar bucles para elementos repetidos y personalizar estilos según tus necesidades."

    # feature loop
    - title: "Funciona en Múltiples Formatos"
      content: "Crea documentos en formatos como MS Office, PDF, OpenOffice, HTML y correos electrónicos. Combina contenido de diversas fuentes en un único archivo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crea Programáticamente una Lista en un Documento"
      content: |
        Este ejemplo demuestra cómo añadir dinámicamente una lista a un documento PDF utilizando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Añade un marcador de posición en tu plantilla para la lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifica la ruta de archivo de la plantilla
          // Las plantillas PDF actualmente no son compatibles.
          const template = "numlist_template.docx";

          // Carga datos para rellenar la lista
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Prepara la fuente de datos con los detalles requeridos
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Inicializa el DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Guarda el documento final con la lista incluida
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "Explora las Funciones de GroupDocs.Assembly"
    exclude: "list"
    description: "Diseña y genera documentos ricos en datos sin esfuerzo utilizando potentes herramientas de integración."
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
    title: "Crea Documentos en Múltiples Formatos"
    exclude: "PDF"
    description: "Node.js via Java soporta más de 50 formatos de archivo, facilitando la fusión de plantillas y datos en resultados profesionales."
    items: 
          
        # format loop 1
        - name: "Crear una lista en un PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Crear una lista en un DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Crear una lista en un PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Crear una lista en un XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---