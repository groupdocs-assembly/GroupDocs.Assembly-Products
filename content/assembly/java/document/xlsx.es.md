



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: es
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Inserte un documento en otro en XLSX usando Java"
head_description: "Combina archivos XLSX con Java. GroupDocs.Assembly simplifica el proceso de fusión de documentos en solo unas pocas líneas de código."

############################# Header ############################
title: "Incorpore contenido en archivos XLSX sin esfuerzo" 
description: "Utilice GroupDocs.Assembly for Java para insertar sin problemas un documento XLSX en otro. Obtenga resultados precisos con herramientas flexibles y confiables."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Consíguelo gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) es una solución versátil para el manejo de documentos. Le permite integrar un documento en otro, admitiendo más de 50 formatos como PDFs y archivos de MS Office. Personalice su salida fusionando, editando y organizando el contenido exactamente como lo desee.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para insertar un documento en un archivo XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) hace que la incorporación de un documento XLSX en otro sea simple y personalizable.
      
      1. Prepare una plantilla XLSX con marcadores de posición para el contenido embebido.
      2. Especifique la ruta del archivo para la plantilla.
      3. Proporcione la ruta del archivo para el documento que desea incorporar.
      4. Guarde el archivo de salida con el contenido fusionado.
   
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
        // Use esta etiqueta en su plantilla para marcar el lugar del documento embebido
        // <<doc [doc_expression]>>

        // Establezca la ruta del archivo para la plantilla principal
        String template = "doc_template.xlsx";

        // Proporcione la ruta al documento que desea insertar
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // Guarde el archivo final con el contenido embebido
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Herramientas avanzadas para simplificar la integración de documentos"
  description: "Con GroupDocs.Assembly for Java, la incorporación de documentos es directa y personalizable, sin importar el tipo de archivo. Logre resultados claros y consistentes en sus proyectos."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Aspectos destacados de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Cree informes utilizando datos empresariales"
      content: "Rellene documentos con datos de fuentes como JSON, XML o CSV de manera rápida y confiable, optimizando sus flujos de trabajo."

    # feature loop
    - title: "Mejore los documentos con contenido visual"
      content: "GroupDocs.Assembly le permite insertar tablas, gráficos y listas junto con texto, hiperenlaces, imágenes e incluso códigos de barras dinámicos."

    # feature loop
    - title: "Coloque los datos exactamente donde pertenecen"
      content: "Las plantillas LINQ ayudan a posicionar sus datos con precisión, manejar elementos repetidos como matrices y aplicar estilos personalizados sin complicaciones."

    # feature loop
    - title: "Compatible con diversos formatos de archivo"
      content: "Fusionar documentos a través de varios formatos, incluidos PDFs, HTML, archivos de MS Office y OpenOffice, garantiza flexibilidad para sus proyectos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo insertar programáticamente una imagen en un documento"
      content: |
        Este ejemplo muestra cómo incrustar una imagen en un archivo XLSX utilizando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Añada una etiqueta de marcador de posición en el archivo de plantilla
          // <<image [expression]>>

          // Defina la ruta a la plantilla
          String template = "template.xlsx";

          // Especifique la ruta de la imagen
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inicialice la instancia de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarde el archivo con la imagen embebida
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "Capacidades clave a simple vista"
    exclude: "document"
    description: "Descubra las amplias características que GroupDocs.Assembly ofrece para hacer que la integración y combinación de documentos sea eficiente y sin complicaciones."
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
    title: "Fusionar entre diferentes tipos de documentos"
    exclude: "XLSX"
    description: "Con Java, puede incorporar y combinar contenido en más de 50 formatos de archivo. Añada archivos sin problemas para crear resultados profesionales."
    items: 
          
        # format loop 1
        - name: "Incorporar un documento en un PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Incorporar un documento en un DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Incorporar un documento en un PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Incorporar un documento en un XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---