---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: es
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Kit de Herramientas de Node.js para Construir, Automatizar y Personalizar Documentos"
head_description: "Biblioteca Node.js para automatizar flujos de trabajo de documentos. Genera archivos PDF, Word, Excel, PowerPoint, HTML y de correo electrónico a partir de tus plantillas."

############################# Header ############################
title: "API Node.js para la Automatización Simplificada de Documentos e Informes"
description: "Optimiza la generación de informes en JavaScript fusionando tus datos con plantillas predefinidas."
words:
  for: "para"

actions:
  main: "Inicia tu Prueba en NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "¿Listo para Comenzar?"
  description: "Prueba las características de GroupDocs.Assembly gratis o solicita una licencia."

release:
  title: "Versión {0} lanzada"
  notes: "Ver novedades"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Crear un Gráfico en un Documento de Word Usando Node.js"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Ruta a la plantilla principal
    const template = "chart_template.docx";

    // Recuperar datos de productividad de los gerentes de la fuente
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Crear una instancia de DataSourceInfo con los datos
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Establecer colores del gráfico usando otro DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Rellenar la plantilla con datos y guardarla en la salida
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Resumen de GroupDocs.Assembly"
  description: "Una biblioteca Node.js diseñada para crear documentos programáticamente con manejo de datos integrado."
  features:
    # feature loop
    - title: "Integra Datos Empresariales en Plantillas con JavaScript"
      content: "Genera informes pulidos al incrustar JSON, XML u otros datos en plantillas con GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Gestiona Contenido Integrado"
      content: "Rellena automáticamente tablas, gráficos y otros elementos visuales en tus documentos utilizando datos externos."

    # feature loop
    - title: "Opciones Personalizables"
      content: "GroupDocs.Assembly for Node.js via Java te permite agregar características como códigos de barras, obtener datos de URL y exportar archivos en varios formatos."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Assembly for Node.js via Java se integra sin problemas con los sistemas operativos, marcos y gestores de paquetes líderes."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo soportados"
  description: |
    GroupDocs.Assembly for Node.js via Java admite una amplia gama de [formatos de documento](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "Funcionalidades Principales de GroupDocs.Assembly"
  description: "Crea documentos e informes dinámicos con potentes herramientas de gestión de datos."

  items:
    # feature loop
    - icon: "preview"
      title: "Visuales de Datos Ricos"
      content: "Inserta gráficos, tablas, imágenes y listas en tus documentos con total personalización."

    # feature loop
    - icon: "manipulate"
      title: "Transforma Tus Datos"
      content: "Aprovecha herramientas como fórmulas y ordenación para estructurar y mostrar información de manera efectiva."

    # feature loop
    - icon: "two_pages"
      title: "Amplia Compatibilidad de Formatos"
      content: "Trabaja sin problemas con formatos de archivo populares para plantillas y salidas."

    # feature loop
    - icon: "document_settings"
      title: "Personalización Avanzada de Plantillas"
      content: "Da formato a las plantillas con opciones de estilo numérico, alfabético y otros."

    # feature loop
    - icon: "text"
      title: "Genera Códigos de Barras Dinámicamente"
      content: "Crea e incrusta imágenes de códigos de barras directamente en tus documentos a demanda."

    # feature loop
    - icon: "add"
      title: "Estilo de Texto Flexible"
      content: "Aplica fácilmente estilos de texto como capitalización o mayúsculas en tus plantillas."

    # feature loop
    - icon: "manipulate"
      title: "Inserción Dinámica de Contenido"
      content: "Incluye contenido de archivos externos de manera dinámica durante la generación del documento."

    # feature loop
    - icon: "convert"
      title: "Exporta a Varios Formatos"
      content: "Guarda documentos en múltiples formatos con las configuraciones que especifiques."

    # feature loop
    - icon: "update"
      title: "Incrusta Medios Dinámicamente"
      content: "Inserta imágenes u otros elementos utilizando datos Base64 al crear documentos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Descubre ejemplos prácticos de cómo usar GroupDocs.Assembly para tareas comunes."
  items:
    # code sample loop
    - title: "Agregar una Lista con Viñetas en Documentos de Word"
      content: |
        Consulta cómo crear [listas con viñetas](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) en documentos de Word para organizar datos de manera efectiva. Este ejemplo demuestra cómo generar una lista con viñetas utilizando GroupDocs.Assembly.
        {{< landing/code title="Agregar una Lista con Viñetas en Documentos de Word">}}
        ```javascript {style=abap}
        // Inserta esta plantilla en una página del documento:
        // Indicadores de rendimiento de los gerentes
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifica la ruta de la plantilla
        const template = "Bulleted List Template.docx";

        // Establece la ruta del archivo de salida
        const result = "Result Report.docx"

        // Recupera datos de los gerentes de una fuente JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Genera el informe con los datos llenos
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Insertar Gráficos de Pastel en PowerPoint"
      content: |
        Aprende a usar plantillas y XML para agregar [gráficos de pastel](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) en tus presentaciones. Mejora tus informes con gráficos de pastel para presentar datos de forma visual y clara.
        {{< landing/code title="Insertar Gráficos de Pastel en PowerPoint">}}
        ```javascript {style=abap} 
        // Agrega la plantilla del título del gráfico a la presentación:
        // Ingresos de los clientes <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Incluye también la plantilla de datos del gráfico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifica la ruta de la plantilla del gráfico
        const template = "Pie Chart Template.pptx";

        // Establece la ruta del archivo de salida
        const result = "Result Report.pptx"

        // Recupera datos de los clientes de una fuente XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Genera el gráfico y guarda el resultado
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---