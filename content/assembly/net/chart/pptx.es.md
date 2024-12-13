



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: es
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cree gráficos en archivos PPTX con C#"
head_description: "La API GroupDocs.Assembly for .NET permite a los desarrolladores generar e insertar gráficos en documentos de forma dinámica utilizando datos en tiempo real."

############################# Header ############################
title: "Incorpore gráficos en archivos PPTX con la API .NET" 
description: "GroupDocs.Assembly for .NET ofrece una forma poderosa de llenar archivos PPTX con datos dinámicos e integrar gráficos sin esfuerzo."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Pruebe Gratis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) es una herramienta diseñada para optimizar la creación de documentos e informes integrando datos de diversas fuentes. Genere gráficos, tablas, listas, códigos de barras e imágenes de forma dinámica. Las opciones avanzadas de formato permiten una colocación precisa y personalización de su contenido. Soporta más de 50 formatos de archivo, incluidos PDF, documentos de MS Office y correos electrónicos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo añadir un gráfico a un documento PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilita la generación e inserción de gráficos en sus plantillas PPTX. Soporta una variedad de tipos de gráficos, como gráficos de barras, circulares y de líneas.
      
      1. Diseñe una plantilla PPTX con marcadores de posición para los gráficos.
      2. Recupere sus datos de una fuente compatible.
      3. Defina las opciones del gráfico como tipo, etiquetas y esquema de colores.
      4. Guarde el archivo actualizado con el gráfico incorporado.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de ejemplo"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Incluya esta etiqueta en su plantilla para generar un gráfico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Especifique la ruta del archivo para su plantilla
        string template = "chart_template.pptx";

        // Cargue datos de su fuente preferida
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Guarde el documento con el gráfico incorporado
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Agregue gráficos dinámicos a sus documentos sin esfuerzo"
  description: "GroupDocs.Assembly for .NET simplifica la creación de documentos impulsados por datos en formatos ampliamente utilizados. Utilice plantillas para insertar gráficos, tablas, códigos de barras, listas, hipervínculos e imágenes con una integración de datos dinámica y avanzada."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Convierta datos en gráficos profesionales"
      content: "Transforme datos de JSON, XML, CSV y otras fuentes en gráficos visualmente atractivos con solo unos pocos pasos utilizando nuestra API."

    # feature loop
    - title: "Cree contenido visualmente atractivo"
      content: "GroupDocs.Assembly soporta múltiples tipos de gráficos, como gráficos de barras, gráficos circulares y gráficos de líneas. Combínelos con tablas, códigos de barras, imágenes y otros elementos para crear informes profesionales."

    # feature loop
    - title: "Coloque y personalice gráficos con precisión"
      content: "Con la sintaxis LINQ, puede generar y colocar gráficos dinámicamente exactamente donde se necesiten. Personalice fácilmente estilos, colores y disposición para satisfacer sus requisitos."

    # feature loop
    - title: "Funciona con varios formatos de archivo"
      content: "Produzca documentos en formatos populares como MS Office, PDF, OpenOffice y HTML. Incorpore gráficos sin problemas en cualquier formato compatible con plena compatibilidad."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cree un gráfico programáticamente"
      content: |
        Este ejemplo demuestra cómo crear e incorporar dinámicamente un gráfico en un documento PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepare una plantilla con un marcador de posición para el gráfico.
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Proporcione la ruta al archivo de plantilla.
          string template = "table_template.pptx";

          // Recupere los datos de su fuente.
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Construya un objeto de datos con la información necesaria.
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configure las propiedades del gráfico, como tipo y apariencia.
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inicialice DocumentAssembler.
          DocumentAssembler asm = new DocumentAssembler();

          // Exporte el documento con el gráfico incluido.
          asm.AssembleDocument(template, "result.pptx", data, design);
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Assembly"
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
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Explora las funciones de GroupDocs.Assembly de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descargar desde Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Conocer sobre la licencia"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Descubra capacidades clave"
    exclude: "chart"
    description: "Nuestra plataforma le ayuda a crear documentos cautivadores impulsados por datos, adaptados a sus necesidades."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cree informes visualmente ricos en múltiples formatos"
    exclude: "PPTX"
    description: ".NET le permite generar documentos con gráficos integrados en más de 50 formatos compatibles, combinando plantillas con sus datos sin complicaciones."
    items: 
          
        # format loop 1
        - name: "Gráficos en PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Gráficos en DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Gráficos en PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Gráficos en XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---