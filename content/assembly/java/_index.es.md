---
############################# Static ############################
layout: "landing"
date: 2025-03-17T13:11:11
draft: false

lang: es
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "Biblioteca Java para Creación, Automatización y Generación de Informes de Documentos"
head_description: "Biblioteca Java para automatizar la creación de documentos y generar informes. Crea documentos PDF, Word, Excel, PPTX, HTML y de correo electrónico usando plantillas personalizadas."

############################# Header ############################
title: "API Java para Automatizar Informes y Documentos"
description: "Simplifica la generación de informes en Java fusionando datos con plantillas."
words:
  for: "para"

actions:
  main: "Obtén Prueba a través de Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "¿Listo para Comenzar?"
  description: "Prueba las características de GroupDocs.Assembly gratis o solicita una licencia."

release:
  title: "Versión {0} lanzada"
  notes: "Ver novedades"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Generar un Gráfico en DOCX con Java"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Ruta a la plantilla principal
    String template = "chart_template.docx";

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
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Resumen de GroupDocs.Assembly"
  description: "Una biblioteca Java diseñada para la creación automatizada de documentos e integración de datos sin interrupciones."
  features:
    # feature loop
    - title: "Fusionar Datos Empresariales en Plantillas con Java"
      content: "Crea fácilmente informes profesionales incrustando datos de JSON, XML u otras fuentes en plantillas pre diseñadas usando GroupDocs.Assembly for Java."

    # feature loop
    - title: "Trabajar con Objetos Embebidos"
      content: "Puebla automáticamente elementos como tablas, gráficos y diagramas en documentos usando datos de fuentes externas."

    # feature loop
    - title: "Personalización Avanzada"
      content: "GroupDocs.Assembly for Java ofrece características flexibles como generar códigos de barras, extraer datos en línea a través de URL y exportar la salida en diferentes formatos."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Assembly for Java funciona sin problemas con sistemas operativos, marcos de desarrollo y gestores de paquetes populares."
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
    GroupDocs.Assembly for Java soporta una amplia gama de [formatos de documento](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
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
  title: "Capacidades Clave de GroupDocs.Assembly"
  description: "Crea documentos y informes profesionales con manejo de datos avanzado."

  items:
    # feature loop
    - icon: "preview"
      title: "Elementos de Datos Visuales"
      content: "Agrega y formatea elementos como gráficos, tablas, imágenes y listas directamente en tus documentos."

    # feature loop
    - icon: "manipulate"
      title: "Transformación de Datos"
      content: "Utiliza fórmulas, ordenamientos y otras herramientas para organizar y presentar tus datos de manera efectiva."

    # feature loop
    - icon: "two_pages"
      title: "Soporte para Varios Formatos"
      content: "Trabaja fácilmente con tipos de archivo comunes tanto para plantillas como para archivos de salida."

    # feature loop
    - icon: "document_settings"
      title: "Formateo Avanzado de Plantillas"
      content: "Personaliza las plantillas con opciones de formateo numérico, alfabético y otras avanzadas."

    # feature loop
    - icon: "text"
      title: "Generación Dinámica de Códigos de Barras"
      content: "Crea y coloca rápidamente imágenes de códigos de barras en documentos según sea necesario."

    # feature loop
    - icon: "add"
      title: "Estilización de Texto Flexible"
      content: "Aplica transformaciones de texto como mayúsculas, minúsculas, estilo título u otros estilos en las plantillas."

    # feature loop
    - icon: "manipulate"
      title: "Importar Contenido Externo"
      content: "Incorpora dinámicamente contenido de archivos externos al generar documentos."

    # feature loop
    - icon: "convert"
      title: "Exportar en Varios Formatos"
      content: "Guarda documentos finales en varios formatos de archivo utilizando extensiones o configuraciones especificadas."

    # feature loop
    - icon: "update"
      title: "Incorporación Dinámica de Medios"
      content: "Inserta imágenes u otro contenido usando datos codificados en Base64 durante la creación de documentos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Explora código de ejemplo para tareas comunes con GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Crear una Lista con Viñetas en Word"
      content: |
        Aprende a agregar [listas con viñetas](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) a documentos de Word para una representación organizada de datos. Este ejemplo muestra cómo generar una lista en Word usando GroupDocs.Assembly.
        {{< landing/code title="Crear una Lista con Viñetas en Word">}}
        ```java {style=abap}
        // Inserta esta plantilla en una página del documento:
        // Indicadores de rendimiento de los gerentes
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Especifica la ruta de la plantilla
        String template = "Bulleted List Template.docx";

        // Establece la ruta del archivo de salida
        String result = "Result Report.docx"

        // Recupera datos de los gerentes de una fuente JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Genera el informe con los datos llenos
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Crear Gráficos Circulares en PPTX"
      content: |
        Usa plantillas y XML para agregar [gráficos circulares](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) a tus presentaciones. Haz que tus informes sean más atractivos al incluir gráficos circulares para visualizar datos.
        {{< landing/code title="Crear Gráficos Circulares en PPTX">}}
        ```java {style=abap}   
        // Agrega la plantilla del título del gráfico a la presentación:
        // Ingresos de los clientes <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Incluye también la plantilla de datos del gráfico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Especifica la ruta de la plantilla del gráfico
        String template = "Pie Chart Template.pptx";

        // Establece la ruta del archivo de salida
        String result = "Result Report.pptx"

        // Recupera datos de los clientes de una fuente XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Genera el gráfico y guarda el resultado
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---