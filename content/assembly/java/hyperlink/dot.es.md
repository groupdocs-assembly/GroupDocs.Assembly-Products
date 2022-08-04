---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/java/hyperlink/dot/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Agregar hipervínculos a Office DOT Documentos e informes a través de la API de Java"
head_description: "GroupDocs.Assembl para Java admite la inserción dinámica de hipervínculos a documentos de oficina y correos electrónicos como PDF DOCX, RTF, XLSX, PPTX, EML, MSG y más dentro de aplicaciones Java."

############################# Header ############################
title: "Agregue hipervínculos a documentos y correos electrónicos de Office a través de la API de Java"
description: "GroupDocs.Assembly Java API permite a los profesionales del software agregar mediante programación hipervínculos a mensajes de correo electrónico y documentos de Office como PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, MSG y más."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo usar la API de Java para agregar hipervínculos a documentos de Office y correos electrónicos?"
    content: |
      Un hipervínculo es una palabra, frase o imagen en la que puede hacer clic para saltar a un nuevo documento o una nueva sección dentro del documento actual. Los hipervínculos son la columna vertebral de la web mundial y se utilizan para muchas funciones necesarias en la World Wide Web. GroupDocs.Assembly para Java es una API de generación de informes y automatización de documentos que ayuda a los desarrolladores de software a insertar dinámicamente hipervínculos dentro de sus documentos o informes con facilidad. La API es muy estable y es totalmente compatible con varias funciones avanzadas relacionadas con la administración de hipervínculos, como agregar hipervínculos a una página de documento, agregar enlaces a una diapositiva de presentación, agregar hipervínculos a celdas de hojas de cálculo, modificar contenido de hipervínculos, insertar dinámicamente enlaces de marcadores, eliminar enlaces no deseados. enlaces, mostrar texto en lugar de hipervínculo, y muchos más. Algunos tipos de documentos muy comunes como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint, etc. son totalmente compatibles.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Insertar hipervínculos a documentos de procesamiento de texto a través de Java"
      content_left: |
       GroupDocs.Assembly Java API es totalmente compatible con la inserción y edición de hipervínculos dentro de varios formatos de documentos de uso común. El siguiente ejemplo de código Java muestra cómo insertar hipervínculos dentro de un documento de Microsoft Word.

      title_right: "Insertar hipervínculos en el documento DOT a través de Java"
      content_right: |
        * Configuración de documentos de origen y destino
        * Establezca la expresión Uri, así como la expresión de texto de visualización
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) método para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "Agregar hipervínculos en hojas de cálculo a través de Java"
      content_left: |
       GroupDocs.Assembly Java API permite a los programadores de computadoras insertar y modificar hipervínculos dentro de sus documentos de hoja de cálculo con facilidad. Pueden acceder fácilmente, editar su ubicación o reemplazarlo por uno nuevo. El siguiente código Java demuestra la facilidad con la que los programadores pueden agregar hipervínculos dentro de sus hojas de cálculo.

      title_right: "Cómo insertar hipervínculos al archivo DOT"
      content_right: |
        * Configuración de archivos de hoja de cálculo de origen y destino
        * Establezca la expresión Uri, así como la expresión de texto de visualización
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) método para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "Insertar hipervínculos a la presentación de PowerPoint a través de Java"
      content_left: |
       GroupDocs.Assembly Java API facilita a los programadores el manejo de sus tareas relacionadas con la administración de documentos. Aquí hay un ejemplo de código Java que muestra cuán fácilmente los programadores de software pueden acceder a sus documentos de presentación de PowerPoint y agregar hipervínculos dentro de ellos.

      title_right: "Cómo insertar hipervínculos en presentaciones"
      content_right: |
        * Configuración de archivos de presentación de origen y destino
        * Establecer Uri y mostrar expresiones de texto
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) método para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "Use la API de Java para agregar hipervínculos en los correos electrónicos"
      content_left: |
       GroupDocs.Assembly para Java facilita a los desarrolladores de software agregar hipervínculos a sus mensajes de correo electrónico con solo un par de líneas de código Java. El siguiente ejemplo demuestra cuán fácilmente pueden los desarrolladores insertar hipervínculos dentro de sus documentos de correo electrónico y enviarlos a otros usuarios dentro de sus propias aplicaciones Java.

      title_right: "Cómo agregar hipervínculos a los correos electrónicos"
      content_right: |
        * Configuración de archivos de hoja de cálculo de origen y destino
        * Establecer Uri y mostrar expresiones de texto
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler)
        * Llame a [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) método para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

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