



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: es
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Crea Listas Dinámicas en PPTX con JavaScript"
head_description: "Diseña e inserta listas en plantillas de PPTX utilizando la API de GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Incorpora Listas Basadas en Datos en Archivos PPTX con Node.js" 
description: "GroupDocs.Assembly for Node.js via Java ofrece herramientas poderosas para añadir listas flexibles impulsadas por datos a documentos PPTX."
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
    title: "Pasos para Insertar una Lista en un Archivo PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita la adición de listas detalladas y basadas en datos a tus plantillas PPTX.
      
      1. Crea una plantilla PPTX y define marcadores de posición para la lista.
      2. Proporciona la ruta del archivo de la plantilla.
      3. Carga datos desde fuentes compatibles como JSON o XML.
      4. Guarda el documento con la lista generada.
   
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
        const template = "list_template.pptx";

        // Obtén los datos de la fuente que deseas utilizar
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Guarda el archivo con la lista incorporada
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
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
        Este ejemplo demuestra cómo añadir dinámicamente una lista a un documento PPTX utilizando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Añade un marcador de posición en tu plantilla para la lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifica la ruta de archivo de la plantilla
          const template = "numlist_template.pptx";

          // Carga datos para rellenar la lista
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Prepara la fuente de datos con los detalles requeridos
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Inicializa el DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Guarda el documento final con la lista incluida
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "Crea Documentos en Múltiples Formatos"
    exclude: "PPTX"
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