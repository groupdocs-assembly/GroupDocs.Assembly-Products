



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: es
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Crea listas en documentos DOCX utilizando Java"
head_description: "Diseña e incrusta dinámicamente listas en tus plantillas DOCX con la API de GroupDocs.Assembly for Java."

############################# Header ############################
title: "Añade listas dinámicas a archivos DOCX con nuestra API de Java" 
description: "GroupDocs.Assembly for Java proporciona herramientas flexibles para generar e insertar listas ricas en datos directamente en documentos DOCX."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Pruébalo Gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) facilita el diseño de documentos profesionales extrayendo datos de múltiples fuentes. Úsalo para crear listas, tablas, gráficos o texto, y coloca estos elementos exactamente donde los necesites utilizando características avanzadas de plantillas. Con soporte para más de 50 formatos, incluidos PDFs, archivos de MS Office y documentos de correo electrónico, ayuda a automatizar y mejorar tu flujo de trabajo.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo añadir una lista basada en datos a un documento DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) te permite insertar rápidamente listas ricas en datos en las plantillas DOCX. Personaliza y organiza el contenido sin esfuerzo.
      
      1. Crea una plantilla DOCX y marca los lugares reservados para la lista.
      2. Establece la ruta del archivo de la plantilla.
      3. Obtén datos de formatos compatibles como JSON o XML.
      4. Guarda el documento final con la lista añadida.
   
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
        // Incluye esta etiqueta en tu plantilla donde debe aparecer la lista
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Define la ruta del archivo de la plantilla
        String template = "list_template.docx";

        // Extrae datos de tu fuente elegida
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Guarda el documento con la lista incrustada
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Genera documentos a partir de plantillas con integración de datos"
  description: "GroupDocs.Assembly for Java simplifica la incorporación de listas dinámicas, tablas, gráficos y otros componentes en las plantillas de documentos."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Características Clave de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Genera informes con datos de diversas fuentes"
      content: "Utiliza datos de formatos como JSON, XML y CSV para poblaciones de listas y otros componentes de manera eficiente."

    # feature loop
    - title: "Incorpora listas y otros elementos de datos sin complicaciones"
      content: "GroupDocs.Assembly permite la inserción de listas, gráficos, tablas y más, junto con texto, imágenes y enlaces para crear documentos pulidos."

    # feature loop
    - title: "Control preciso sobre dónde aparecen los datos"
      content: "Las plantillas basadas en LINQ te permiten definir ubicaciones exactas para tus listas y datos. Usa bucles para crear listas detalladas automáticamente y aplicar formato personalizado."

    # feature loop
    - title: "Soporta diversos formatos de documentos"
      content: "Crea o edita archivos en formatos como MS Office, PDF, OpenOffice, HTML y correo electrónico. Une contenido de múltiples documentos según sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo crear una lista programáticamente"
      content: |
        Este ejemplo muestra cómo añadir dinámicamente una lista a un archivo DOCX utilizando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Añade una etiqueta de marcador de posición en tu plantilla para la lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Proporciona la ruta del archivo a tu plantilla
          String template = "numlist_template.docx";

          // Extrae los datos necesarios para poblar la lista
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Prepara la fuente de datos con los detalles necesarios
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inicializa DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarda el documento de salida con la lista completada
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_list.docx"
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
    title: "Descubre lo que GroupDocs.Assembly puede hacer"
    exclude: "list"
    description: "Diseña y genera fácilmente documentos ricos en contenido con herramientas avanzadas de integración de datos."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/java/barcode/docx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/java/chart/docx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/java/document/docx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/java/list/docx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/java/table/docx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produce documentos en varios formatos"
    exclude: "DOCX"
    description: "Java admite más de 50 formatos, permitiéndote crear documentos estructurados al combinar datos y plantillas."
    items: 
          
        # format loop 1
        - name: "Crear una lista en un PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Crear una lista en un DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Crear una lista en un PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Crear una lista en un XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---