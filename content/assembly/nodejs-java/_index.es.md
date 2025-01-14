---
############################# Static ############################
layout: "landing"
date: 2025-01-14T15:37:19
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
head_title: "{index-content-nodejs-java.head_title}"
head_description: "{index-content-nodejs-java.head_description}"

############################# Header ############################
title: "{index-content-nodejs-java.title}"
description: "{index-content-nodejs-java.description}"
words:
  for: "para"

actions:
  main: "{index-content-nodejs-java.actions_main}"
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
  title: "{index-content-nodejs-java.code_title}"
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
  description: "{index-content-nodejs-java.overview_description}"
  features:
    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_1.title}"
      content: "{index-content-nodejs-java.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_2.title}"
      content: "{index-content-nodejs-java.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-nodejs-java.overview_feature_3.title}"
      content: "{index-content-nodejs-java.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "{index-content-nodejs-java.platforms_description}"
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
    {index-content-nodejs-java.formats_description}
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
  title: "{index-content-nodejs-java.features.title}"
  description: "{index-content-nodejs-java.features.description}"

  items:
    # feature loop
    - icon: "preview"
      title: "{index-content-nodejs-java.features.feature_1.title}"
      content: "{index-content-nodejs-java.features.feature_1.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_2.title}"
      content: "{index-content-nodejs-java.features.feature_2.content}"

    # feature loop
    - icon: "two_pages"
      title: "{index-content-nodejs-java.features.feature_3.title}"
      content: "{index-content-nodejs-java.features.feature_3.content}"

    # feature loop
    - icon: "document_settings"
      title: "{index-content-nodejs-java.features.feature_4.title}"
      content: "{index-content-nodejs-java.features.feature_4.content}"

    # feature loop
    - icon: "text"
      title: "{index-content-nodejs-java.features.feature_5.title}"
      content: "{index-content-nodejs-java.features.feature_5.content}"

    # feature loop
    - icon: "add"
      title: "{index-content-nodejs-java.features.feature_6.title}"
      content: "{index-content-nodejs-java.features.feature_6.content}"

    # feature loop
    - icon: "manipulate"
      title: "{index-content-nodejs-java.features.feature_7.title}"
      content: "{index-content-nodejs-java.features.feature_7.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-nodejs-java.features.feature_8.title}"
      content: "{index-content-nodejs-java.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-nodejs-java.features.feature_9.title}"
      content: "{index-content-nodejs-java.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "{index-content-nodejs-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-nodejs-java.code_title_sample_1}"
      content: |
        {index-content-nodejs-java.code_samples_sample_1_content_1} {index-content-nodejs-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_1}">}}
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
    - title: "{index-content-nodejs-java.code_title_sample_2}"
      content: |
        {index-content-nodejs-java.code_samples_sample_2_content_1} {index-content-nodejs-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-nodejs-java.code_title_sample_2}">}}
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