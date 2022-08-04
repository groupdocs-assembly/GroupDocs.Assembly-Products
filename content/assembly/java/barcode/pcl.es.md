---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/java/barcode//pcl/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS XML OXPS MD EML EMLX MSG 

############################# Head ############################
head_title: "API de Java para generar documentos de imágenes de código de barras y mensajes de correo electrónico"
head_description: "GroupDocs.Assembly Java API permite a los programadores crear y agregar códigos de barras en documentos (PDF, DOC, DOCX, RTF, XLSX, CSV, PPTX) y mensajes de correo electrónico (EML EMLX MSG)."

############################# Header ############################
title: "Java Barcodes Generator API: cree códigos de barras 1D y 2D en documentos PCL"
description: "GroupDocs.Assembly Java API permite generar y agregar imágenes de código de barras 1D y 2D dentro de mensajes PDF HTML, XPS, PS, TXT, EPUB, PCL, SVG, documentos y correos electrónicos (EML, EMLX, MSG)."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo generar e insertar códigos de barras en documentos y correos electrónicos?"
    content: |
       Los códigos de barras se están volviendo populares y se usan en todas partes en estos días. Comenzó a aparecer en las tiendas de abarrotes a mediados de la década de 1970 y hoy se puede encontrar en libros, boletos, hospitales para rastrear medicamentos, tiendas de autopartes y muchos más. Esta página web explicará cómo crear y agregar dinámicamente imágenes de códigos de barras dentro de documentos y correos electrónicos en aplicaciones Java. GroupDocs.Assembly para Java es una API muy útil que ayuda a los desarrolladores de software a crear potentes aplicaciones de generación de informes y automatización de documentos. Brinda soporte para manejar muchos formatos de documentos populares como PDF, HTML, XPS, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint, correo electrónico de Outlook y muchos más. La API de Java facilita la creación e inserción de imágenes de códigos de barras en documentos y mensajes de correo electrónico con solo un par de líneas de código. También admite la modificación de las propiedades de la imagen del código de barras, como escalar la imagen del código de barras, alterar los colores del frente y del fondo, cambiar la resolución de la imagen del código de barras, la ubicación del texto del código de barras, cambiar las fuentes y más. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Cree códigos de barras en PCL documentos a través de Java"
      content_left: |
       GroupDocs.Assembly Java ha incluido una funcionalidad completa para insertar y editar códigos de barras dentro de documentos PCL. El siguiente ejemplo de código Java demuestra cómo crear y usar imágenes de código de barras dentro de un documento PCL con solo un par de líneas de código. 

      title_right: "¿Cómo agregar códigos de barras en archivos PCL?"
      content_right: |
       * Cree una instancia de [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
       * Crear objeto de fuente de datos de muestra
       * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.DataSourceInfo...-) método con los siguientes parámetros
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones de carga y guardado de documentos.
          * Detalles Información sobre los objetos de origen de datos que se utilizarán.

      gisthash: "ebb6d8215f329f457f843e9a9fc48c9c"
      gistfile: "generate_barcodes_in_presentations.java"     

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