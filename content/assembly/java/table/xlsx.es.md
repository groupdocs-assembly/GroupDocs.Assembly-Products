



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: es
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Agrega tablas a documentos XLSX utilizando Java"
head_description: "Con GroupDocs.Assembly for Java, los desarrolladores pueden integrar rápidamente tablas en documentos y correos electrónicos, extrayendo datos de fuentes dinámicas."

############################# Header ############################
title: "Rellena tablas en archivos XLSX con nuestra API Java" 
description: "GroupDocs.Assembly for Java simplifica el proceso de llenar tablas en documentos XLSX con datos de diversas entradas."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtén Tu Prueba Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) es una herramienta para generar documentos e informes mediante la inserción automática de datos en plantillas pre-diseñadas. Puedes agregar tablas, listas, gráficos e imágenes sin esfuerzo. Sus características avanzadas te permiten situar contenido con precisión dentro de tus documentos. Compatible con más de 50 tipos de archivos, incluidos PDF, MS Office y formatos de correo.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para insertar datos en una tabla XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) te ayuda a llenar plantillas de tablas para XLSX y otros formatos. Usa datos dinámicos de tus fuentes para crear tablas de manera eficiente.
      
      1. Configura una plantilla XLSX con marcadores de posición para filas y columnas de tabla.
      2. Extrae datos de cualquier fuente de entrada compatible.
      3. Filtra o preprocesa los datos para ajustarlos a tus necesidades.
      4. Genera el documento final con la tabla completada.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de ejemplo"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Usa estas etiquetas en un marcador de fila de tabla dentro de tu plantilla
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Define la ruta al archivo de plantilla
        String template = "table_template.xlsx";

        // Carga datos desde tu fuente elegida
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Guarda el archivo de salida con la tabla poblada
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Crea documentos con tablas llenas de datos"
  description: "GroupDocs.Assembly for Java facilita la automatización de la creación de tablas en tus documentos. También soporta la adición de elementos como gráficos, listas e imágenes usando plantillas."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Características Principales de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera informes a partir de múltiples formatos de datos"
      content: "La API funciona sin problemas con JSON, XML, CSV y otros formatos para llenar tablas en tus documentos con datos organizados."

    # feature loop
    - title: "Presenta información visualmente"
      content: "GroupDocs.Assembly te ayuda a construir tablas, listas y gráficos profesionales, así como insertar enlaces, texto e imágenes, para un aspecto pulido."

    # feature loop
    - title: "Coloca contenido en la tabla con precisión"
      content: "Utiliza una sintaxis flexible basada en LINQ para agregar filas y columnas de manera dinámica. Personaliza la apariencia, como estilos y colores de fuente, programáticamente."

    # feature loop
    - title: "Compatible con múltiples formatos"
      content: "Trabaja con MS Office, OpenOffice, PDF, HTML y más. Fusiona tablas en cualquier formato de archivo soportado sin esfuerzo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crea una tabla llena de datos de manera dinámica"
      content: |
        Este ejemplo muestra cómo llenar una tabla en un documento XLSX utilizando datos de entrada dinámicos.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Diseña una plantilla con un marcador de posición para la tabla
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Establece la ubicación del archivo de plantilla
          String template = "table_template.xlsx";

          // Carga datos de tu fuente preferida
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Prepara un objeto de datos que contenga los campos necesarios
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Crea una instancia de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarda el documento con la tabla poblada
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Descargar el resultado"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.xlsx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Explora las funciones de GroupDocs.Assembly de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descargar desde Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Conocer sobre la licencia"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Características clave a primera vista"
    exclude: "table"
    description: "Nuestra API simplifica la creación de documentos profesionales al automatizar el llenado de tablas junto con otros componentes poderosos."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produce tablas detalladas en varios formatos"
    exclude: "XLSX"
    description: "Con Java, puedes llenar plantillas con datos y generar informes detallados en más de 50 tipos de archivos."
    items: 
          
        # format loop 1
        - name: "Agregar una tabla a un PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Agregar una tabla a un DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar una tabla a un PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Agregar una tabla a un XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---