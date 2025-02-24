



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: es
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Generar gráficos en documentos PPTX usando Java"
head_description: "La API GroupDocs.Assembly for Java permite a los desarrolladores crear e insertar gráficos dinámicos en documentos de manera fluida, impulsados por datos en tiempo real."

############################# Header ############################
title: "Añadir gráficos a documentos PPTX con la API de Java" 
description: "GroupDocs.Assembly for Java simplifica el proceso de incrustar gráficos en documentos PPTX utilizando datos en tiempo real."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Empieza a usarlo gratis"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Introducción a GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) es una solución versátil para automatizar la creación de documentos e informes. Permite agregar gráficos, tablas, listas, códigos de barras e imágenes directamente en sus archivos, con herramientas avanzadas para un formato y una integración de datos precisos. La plataforma admite más de 50 formatos, incluidos PDF, archivos de Microsoft Office y correos electrónicos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para incrustar un gráfico en un documento PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) simplifica el proceso de insertar gráficos en plantillas PPTX. Elige entre una variedad de estilos de gráficos, incluidos gráficos de barras, circulares y de líneas.
      
      1. Crea una plantilla PPTX con marcadores de posición para el gráfico.
      2. Carga tus datos desde una fuente compatible.
      3. Establece las opciones del gráfico, como tipo, etiquetas y colores.
      4. Guarda el documento con el gráfico incluido.
   
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
        // Añade esta etiqueta a tu plantilla para incluir un gráfico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Proporciona la ruta del archivo a tu plantilla
        String template = "chart_template.pptx";

        // Extrae los datos necesarios de tu fuente
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Guarda el documento final con el gráfico incrustado
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Incorpora gráficos dinámicos en tus documentos con facilidad"
  description: "GroupDocs.Assembly for Java proporciona una forma simple de construir documentos ricos en datos en formatos populares. Utiliza plantillas para insertar gráficos, tablas, códigos de barras, listas, enlaces e imágenes con actualizaciones dinámicas de tus datos."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Convierte datos en gráficos"
      content: "Utiliza la API para transformar datos de JSON, XML, CSV u otras fuentes en gráficos claros y profesionales para tus documentos."

    # feature loop
    - title: "Crea contenido visualmente impactante"
      content: "GroupDocs.Assembly admite varios formatos visuales, incluidos gráficos de barras, gráficos circulares y gráficos de líneas, que se pueden combinar con tablas, códigos de barras, imágenes y más para informes mejorados."

    # feature loop
    - title: "Colocación y estilo de gráficos personalizables"
      content: "Con una sintaxis basada en LINQ, puedes generar y posicionar gráficos dinámicamente en el documento, ajustando estilos, colores y diseños para satisfacer tus necesidades de diseño."

    # feature loop
    - title: "Admite múltiples formatos de documento"
      content: "Genera documentos en formatos como MS Office, PDF, OpenOffice y HTML. Los gráficos se integran perfectamente en cualquier formato compatible para resultados profesionales."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Generar e incrustar gráficos de manera programática"
      content: |
        Este ejemplo demuestra cómo crear e incrustar un gráfico en un documento PPTX de forma programática.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Prepara una plantilla con un marcador de posición para el gráfico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Especifica la ruta del archivo a la plantilla
          String template = "table_template.pptx";

          // Carga datos desde tu fuente elegida
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crea un objeto de datos con la información relevante
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configura el tipo y la apariencia del gráfico
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inicializa DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Guarda el documento completado con el gráfico incrustado
          asm.assembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "Explora capacidades poderosas"
    exclude: "chart"
    description: "Esta plataforma simplifica el proceso de diseño de documentos visualmente atractivos y centrados en los datos, adaptados a tus necesidades."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Genera informes completos en diversos formatos"
    exclude: "PPTX"
    description: "Java te permite crear documentos con gráficos integrados en más de 50 formatos de archivo, asegurando una fusión fluida de plantillas y datos."
    items: 
          
        # format loop 1
        - name: "Gráficos en PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Gráficos en DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Gráficos en PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Gráficos en XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---