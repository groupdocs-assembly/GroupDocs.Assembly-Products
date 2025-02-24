



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:04
draft: false
lang: es
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generar códigos de barras en documentos PDF con C#"
head_description: "La API GroupDocs.Assembly for .NET permite a los desarrolladores generar e incrustar dinámicamente imágenes de códigos de barras en documentos y correos electrónicos."

############################# Header ############################
title: "Añadir códigos de barras a documentos PDF utilizando nuestra API .NET" 
description: "GroupDocs.Assembly for .NET ofrece soporte completo para crear e incrustar códigos de barras dinámicamente en documentos PDF."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Prueba Gratuita"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Descripción general de GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Aprender más"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) está diseñado para ayudarlo a generar documentos e informes integrando datos de una amplia variedad de fuentes. Rellene documentos con texto o datos numéricos, cree gráficos, tablas y listas, o inserte imágenes y códigos de barras sobre la marcha. Utilice un marcado avanzado para colocar datos precisamente donde se necesiten. Soporta más de 50 formatos, incluyendo PDF, archivos de MS Office y correos electrónicos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para agregar un código de barras generado a un documento PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilita la inserción de códigos de barras en plantillas en formatos como PDF. Soporta más de 60 tipos de códigos de barras, incluidos formatos unidimensionales y bidimensionales.
      
      1. Cree una plantilla con etiquetas específicas para la ubicación del código de barras (nota: las plantillas PDF no son compatibles).
      2. Recupere datos de cualquier fuente de datos soportada.
      3. Configure propiedades adicionales como el tamaño del código de barras o la resolución.
      4. Guarde el documento final con el código de barras insertado como un PDF.
   
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
        // Inserte esta etiqueta en su plantilla para generar un código de barras en el documento final.
        // <<barcode [barcode_expression] -barcode_type>>

        // Especifique la ruta del archivo de la plantilla.
        // El soporte para las plantillas PDF no está disponible en este momento.
        string template = "barcode_template.docx";

        // Recupere datos de su fuente.
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Guarde el documento con el código de barras generado.
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Generar documentos llenando plantillas con datos"
  description: "GroupDocs.Assembly for .NET está diseñado para simplificar la creación de documentos en formatos populares. Agregue gráficos, listas, tablas, hipervínculos, imágenes y códigos de barras utilizando plantillas y marcado avanzados."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Características de GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crear informes a partir de datos empresariales"
      content: "Nuestra API llena documentos de manera eficiente en formatos de oficina populares utilizando datos de fuentes como JSON, XML y CSV."

    # feature loop
    - title: "Utilizar elementos visuales para mostrar datos"
      content: "GroupDocs.Assembly admite la incorporación de elementos nativos como listas, tablas y gráficos, junto con texto, hipervínculos, imágenes y códigos de barras generados dinámicamente."

    # feature loop
    - title: "Insertar datos en cualquier parte del documento"
      content: "Utilice la sintaxis basada en LINQ para colocar datos exactamente donde se necesitan. Los arreglos se pueden insertar utilizando bucles for-each, y el formato (por ejemplo, color) se puede personalizar programáticamente."

    # feature loop
    - title: "Soporta una amplia gama de formatos"
      content: "Procesar formatos de archivo populares como MS Office, OpenOffice, PDF, HTML y varios formatos de correo electrónico. Incruste un documento dentro de otro según sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo generar un código de barras dinámicamente"
      content: |
        Este ejemplo demuestra cómo incrustar un código de barras generado dinámicamente en un documento PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Utilice esta plantilla para insertar un código de barras en el documento.
          // <<barcode [barcode_expression] -barcode_type>>

          // Especifique la ruta al archivo de plantilla.
          // El soporte para las plantillas PDF no está disponible en este momento.
          string template = "barcode_template.docx";

          // Recupere datos de su fuente elegida.
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // Cree un objeto de origen de datos con solo los datos necesarios.
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // Inicialice DocumentAssembler.
          DocumentAssembler asm = new DocumentAssembler();

          // Establezca propiedades adicionales del código de barras.
          asm.BarcodeSettings.Resolution = 1200;
          asm.BarcodeSettings.BaseYDimension = 5f;

          // Guarde el documento final con el código de barras incrustado.
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "Explorar características clave"
    exclude: "barcode"
    description: "Nuestra solución está diseñada para optimizar sus necesidades de procesamiento de documentos empresariales."
    items: 
          
        # operation loop 1
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Crear y añadir dinámicamente códigos de barras a documentos"

        # operation loop 2
        - name: "Visualizar datos con diagramas"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Rellenar varios tipos de diagramas con datos"

        # operation loop 3
        - name: "Combinar documentos"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Integrar el contenido de un documento en otro"

        # operation loop 4
        - name: "Mostrar datos con listas"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Generar listas en documentos utilizando datos específicos"

        # operation loop 5
        - name: "Organizar datos en tablas"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Recuperar datos de cualquier fuente y completar tablas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crear informes en formatos populares"
    exclude: "PDF"
    description: ".NET admite la generación de informes en más de 50 formatos, lo que le permite combinar datos y plantillas para obtener resultados excepcionales."
    items: 
          
        # format loop 1
        - name: "Agregar un código de barras a un PDF"
          format: "PDF"
          link: "/assembly/net/barcode/pdf/"
          description: "Formato de Documento Portable de Adobe"
          
        # format loop 2
        - name: "Agregar un código de barras a un DOCX"
          format: "DOCX"
          link: "/assembly/net/barcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar un código de barras a un PPTX"
          format: "PPTX"
          link: "/assembly/net/barcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Agregar un código de barras a un XLSX"
          format: "XLSX"
          link: "/assembly/net/barcode/xlsx/"
          description: "Hoja de Cálculo XML Abierta de Microsoft Excel"


          

---