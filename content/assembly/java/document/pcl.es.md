---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/java/document/pcl"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "API de Java: agregar contenido de documentos externos a pcl_formatos de archivo SUPERIORES"
head_description: "GroupDocs.Assembly Java API permite la inserción dinámica del contenido de documentos externos en varios formatos de archivo como PDF, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG y más."

############################# Header ############################
title: "API de Java para insertar el contenido de un documento externo en otros formatos de archivo admitidos"
description: "GroupDocs.Assembly para Java proporciona funciones para insertar contenido de documentos externos en informes, correos electrónicos y varios formatos de archivo compatibles como PDF, DOC, DOCX, XLSX, CSV, PPTX, EML, MSG y más."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo insertar el contenido de un documento externo en otros formatos de archivo populares a través de Java?"
    content: |
       Un documento o archivo es una copia electrónica o una copia impresa que contiene información que el usuario puede recuperar en una etapa posterior. Según Wikipedia, un documento puede estar estructurado, como documentos tabulares, listas, formularios o tablas científicas, semiestructurado como un libro o un artículo de periódico, o no estructurado como una nota escrita a mano. GroupDocs.Assembly para Java es una API muy útil que permite a los desarrolladores de software crear potentes aplicaciones para la automatización de documentos y la generación de informes. Es totalmente compatible con la identificación y el trabajo con numerosos formatos de documentos, como PDF, Microsoft Word, hojas de cálculo de Excel, PowerPoint, HTML, correo electrónico de Outlook y muchos más. Admite numerosas funciones avanzadas para trabajar con informes, como la manipulación de elementos de plantilla, informes de listas, informes de gráficos, informes de tablas, etc. Además, la API también es totalmente compatible con varias funciones avanzadas relacionadas con la adición y modificación de contenido de documentos, como agregar contenido a una página de documento, insertar datos en celdas de hojas de cálculo, reemplazar contenido, agregar contenido a una diapositiva de presentación y mucho más. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Agregue contenido de archivo externo a un documento de Word a través de Java"
      content_left: |
       GroupDocs.Assembly Java API ayuda a los programadores de computadoras a manejar tareas de manipulación de documentos dentro de sus propias aplicaciones Java. Es totalmente compatible con el contenido del archivo de un documento externo para varios tipos de tipos de documentos. El siguiente ejemplo de código Java muestra cómo agregar el contenido de un archivo externo a un documento de procesamiento de Word con solo un par de líneas de código. 

      title_right: "Cómo insertar el contenido del documento en el archivo PCL"
      content_right: |
        * Configuración de la plantilla del documento de origen
        * Configuración del informe del documento de destino
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) método para ensamblar el documento. es compatible
          * La secuencia desde la que leer un documento de plantilla.
          * La corriente para escribir un documento de resultados.
          * Especifica opciones adicionales para cargar y guardar documentos.
          * Proporciona información sobre los objetos de origen de datos que se utilizarán.

      gisthash: "abb65f9e514add59870865121ed3c526"
      gistfile: "insert_documents_to_word_processing.java"

    - title_left: "Agregar contenido de archivos externos a mensajes de correo electrónico a través de Java"
      content_left: |
       GroupDocs.Assembly Java API ha incluido funcionalidad para la inserción de contenido de documentos externos dinámicos en varios formatos de archivo de documentos populares y mensajes de correo electrónico. El siguiente código Java muestra cómo los programadores pueden agregar contenido de documentos externos a sus documentos de correo electrónico sin ninguna aplicación externa.

      title_right: "Cómo agregar el contenido del archivo al documento PCL"
      content_right: |
        * Configuración de la plantilla del documento de origen
        * Configuración del informe del documento de destino
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) método para ensamblar el documento. es compatible
          * La secuencia desde la que leer un documento de plantilla.
          * La corriente para escribir un documento de resultados.
          * Especifica opciones adicionales para cargar y guardar documentos.
          * Proporciona información sobre los objetos de origen de datos que se utilizarán.

      gisthash: "b72d7608548993ffbe62f97c798ba021"
      gistfile: "Insert_dynamic_documents_to_emails.java"

    - title_left: "Requisitos del sistema"
      content_left: |
        Las API de GroupDocs.Assembly Java son compatibles con todas las principales plataformas y sistemas operativos. Puede generar documentos en Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice y más de 50 formatos. Para obtener una guía completa de requisitos del sistema, visite [requisitos del sistema](https://docs.groupdocs.com/assembly/java/system-requirements/) Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema:
         * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
         * Compatibilidad con versiones de Java: J2SE 7.0 (1.7), J2SE 8.0 (1.8) o superior
         * Obtenga la última versión de las API Java de GroupDocs.Assembly de [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/)
        
      title_right: "Por qué usar GroupDocs.Assembly"
      content_right: |
        * Cree documentos personalizados a partir de plantillas.
        * Adjunte dinámicamente archivos adjuntos de correo electrónico.
        * No se requiere software adicional para crear y automatizar documentos.
        * Genera un documento de salida basado en la fuente de datos.
        * Insertar dinámicamente el contenido del documento en el informe
        * Aplicar fórmula durante el montaje de la hoja de cálculo.
        * Proporciona soporte para múltiples formatos de datos
        * Soporte de operaciones de datos secuenciales.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---