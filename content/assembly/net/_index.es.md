---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: es
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "API .NET para Automatización de Documentos, Ensamblaje y Generación de Informes"
head_description: "API C# .NET para automatización de documentos, ensamblaje y generación de informes. Crea documentos PDF, Word, Excel, PPTX, HTML y de correo electrónico a partir de plantillas personalizadas."

############################# Header ############################
title: "API de Automatización de Documentos y Generación de Informes en .NET"
description: "Genera informes en aplicaciones .NET definiendo plantillas y fusionando datos."
words:
  for: "para"

actions:
  main: "Descargar Prueba a través de Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "¿Listo para Comenzar?"
  description: "Prueba las características de GroupDocs.Assembly gratis o solicita una licencia."

release:
  title: "Versión {0} lanzada"
  notes: "Ver novedades"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Rellenar un Gráfico en DOCX Usando C#"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Ruta a la plantilla principal
    string template = "chart_template.docx";

    // Recuperar datos de productividad de los gerentes de la fuente
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Crear una instancia de DataSourceInfo con los datos
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Establecer colores del gráfico usando otro DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Rellenar la plantilla con datos y guardarla en la salida
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Resumen de GroupDocs.Assembly"
  description: "Solución .NET para automatizar la creación de documentos con integración de datos avanzada."
  features:
    # feature loop
    - title: "Agregar Datos Empresariales a Plantillas de Documentos con C#"
      content: "Generación de informes simplificada: Con GroupDocs.Assembly for .NET, puedes insertar sin esfuerzo datos de fuentes como JSON o XML en plantillas predefinidas."

    # feature loop
    - title: "Procesar Objetos de Datos Nativos"
      content: "Los tipos de documentos soportados incluyen objetos embebidos como diagramas, gráficos, tablas y listas que pueden ser poblados automáticamente con datos."

    # feature loop
    - title: "Características Adicionales"
      content: "GroupDocs.Assembly for .NET proporciona amplias opciones de personalización. Diseña programáticamente objetos de datos, genera códigos de barras, usa fuentes de datos en línea a través de URL y guarda la salida en varios formatos."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Assembly for .NET es compatible con los siguientes sistemas operativos, marcos y gestores de paquetes."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo soportados"
  description: |
    GroupDocs.Assembly for .NET puede procesar los siguientes [formatos de archivo](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos de Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Imágenes y Otros Formatos
        * **Portable:** PDF
        * **Imágenes:** SVG, TIFF
        * **Otros formatos de oficina:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Otros formatos
        * **Web:** HTML, MHTML
        * **Correos electrónicos:** EML, MSG, EMLX
        * **Otros:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Características de GroupDocs.Assembly"
  description: "Crea documentos e informes utilizando modelos de datos avanzados."

  items:
    # feature loop
    - icon: "preview"
      title: "Representación Avanzada de Datos"
      content: "Soporta una amplia gama de objetos de datos como gráficos, listas, tablas, imágenes y más."

    # feature loop
    - icon: "manipulate"
      title: "Manipulación de Datos"
      content: "Aplica fórmulas y operaciones secuenciales para formatear y mostrar datos de manera efectiva."

    # feature loop
    - icon: "two_pages"
      title: "Amplia Gama de Formatos Soportados"
      content: "Trabaja sin problemas con todos los formatos de documentos comunes para plantillas o archivos de salida."

    # feature loop
    - icon: "document_settings"
      title: "Marcado de Plantilla Rico"
      content: "Aprovecha el formateo numérico ordinal, cardinal y alfabético en las plantillas."

    # feature loop
    - icon: "text"
      title: "Incluir Códigos de Barras"
      content: "Genera imágenes de códigos de barras dinámicamente e insértalas en tus documentos."

    # feature loop
    - icon: "add"
      title: "Formateo de Datos"
      content: "Formatea cadenas en plantillas como mayúsculas, minúsculas, capitalizadas o estilos de primera letra en mayúscula."

    # feature loop
    - icon: "manipulate"
      title: "Manipulación de Contenido del Documento"
      content: "Inserta dinámicamente contenido de documentos externos en tus informes."

    # feature loop
    - icon: "convert"
      title: "Guardar en Varios Formatos"
      content: "Especifica el formato de archivo de salida usando extensiones de archivo o configuraciones detalladas."

    # feature loop
    - icon: "update"
      title: "Procesamiento de Datos Flexible"
      content: "Inserta imágenes y documentos dinámicamente usando bytes codificados en Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Fragmentos de código para operaciones típicas de GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Lista con Viñetas en un Documento de Microsoft Word"
      content: |
        [Listas con viñetas](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) son una forma común de presentar datos empresariales. Aquí tienes un ejemplo de cómo agregar una lista a un documento de Word usando GroupDocs.Assembly.
        {{< landing/code title="Cómo Poblar una Lista en Documentos">}}
        ```csharp {style=abap}
        // Inserta esta plantilla en una página del documento:
        // Indicadores de rendimiento de los gerentes
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Especifica la ruta de la plantilla
        string template = "Bulleted List Template.docx";

        // Establece la ruta del archivo de salida
        string result = "Result Report.docx"

        // Recupera datos de los gerentes de una fuente JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Genera el informe con los datos llenos
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Gráficos Circulares en Presentaciones PPTX"
      content: |
        Puedes crear [Gráficos Circulares](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) usando plantillas y datos XML. Mejora tus informes con representaciones visuales atractivas de datos.
        {{< landing/code title="Cómo Representar Datos en un Gráfico Circular">}}
        ```csharp {style=abap}
        // Agrega la plantilla del título del gráfico a la presentación:
        // Ingresos de los clientes <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Incluye también la plantilla de datos del gráfico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Especifica la ruta de la plantilla del gráfico
        string template = "Pie Chart Template.pptx";

        // Establece la ruta del archivo de salida
        string result = "Result Report.pptx"

        // Recupera datos de los clientes de una fuente XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Genera el gráfico y guarda el resultado
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---