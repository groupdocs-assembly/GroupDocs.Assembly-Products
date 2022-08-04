---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/net/hyperlink/pptx/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: ".NET API para insertar dinámicamente hipervínculos en PPTX Documentos"
head_description: "GroupDocs.Assembly .NET API permite a los desarrolladores insertar dinámicamente hipervínculos a correos electrónicos, informes o documentos como PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG y más."

############################# Header ############################
title: "Inserte dinámicamente hipervínculos a PPTX Documentos e informes a través de la API de .NET"
description: "GroupDocs.Assembly .NET API permite a los programadores insertar dinámicamente hipervínculos a informes, correos electrónicos y documentos de Office como PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, EML, HTML, MSG y más."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo insertar dinámicamente hipervínculos en informes, correos electrónicos y varios documentos?"
    content: |
       Esta página web explicará cómo los usuarios pueden insertar dinámicamente hipervínculos a su informe, mensaje de correo electrónico y varios tipos de documentos dentro de sus propias aplicaciones .NET. Los hipervínculos son la columna vertebral de la World Wide Web y se pueden utilizar para vincular diferentes páginas, documentos o hacer clic en para saltar a una nueva sección dentro del documento actual. GroupDocs.Assembly .NET es una API muy poderosa que ayuda a los desarrolladores de software a agregar hipervínculos dinámicamente dentro de sus documentos o informes con solo un par de líneas de código. Ha incluido soporte para algunos de los tipos de documentos más populares, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint y muchos más. Admitía varias funciones avanzadas, como Insertar enlaces a la página del documento, Insertar enlaces a celdas, editar hipervínculos, mostrar texto en lugar del hipervínculo, insertar dinámicamente enlaces desde marcadores, insertar hipervínculos a una diapositiva de presentación y muchas más.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Inserción de hipervínculos a documentos de procesamiento de texto a través de .NET"
      content_left: |
       GroupDocs.Assembly .NET API brinda soporte completo para insertar y editar hipervínculos dentro de varios tipos de documentos. El siguiente ejemplo de código C# .NET muestra cómo agregar hipervínculos dentro de un documento de Word con facilidad. 

      title_right: "Cómo agregar hipervínculos en un archivo de Word"
      content_right: |
        * Configuración de documentos de origen y destino
        * Establezca la expresión Uri, así como la expresión de texto de visualización
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "f4a8031406d44941d400088b718f7730"
      gistfile: "insert_hyperlinks_to_word_document.cs"

    - title_left: "Insertar dinámicamente hipervínculos en hojas de cálculo a través de .NET"
      content_left: |
       GroupDocs.Assembly .NET API es totalmente compatible con la adición y el procesamiento de hipervínculos dentro de los archivos de hojas de cálculo. Puede editar fácilmente su ubicación o reemplazarla por una nueva. El siguiente código de C# muestra la facilidad con la que los usuarios pueden insertar hipervínculos en sus archivos de hoja de cálculo dentro de sus propias aplicaciones .NET.

      title_right: "Add hipervínculos a documentos de hoja de cálculo"
      content_right: |
        * Configuración de archivos de hoja de cálculo de origen y destino
        * Establezca la expresión Uri, así como la expresión de texto de visualización
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "c2f9cd8bb06f9a7a2c444621ebf82696"
      gistfile: "insert_hyperlinks_in_spreadsheet_documents.cs"

    - title_left: "Agregue hipervínculos a la presentación de PowerPoint a través de la API de .NET"
      content_left: |
       GroupDocs.Assembly para .NET ayuda a los profesionales del software a crear aplicaciones para administrar varios tipos de documentos. El siguiente ejemplo de código demuestra cómo los desarrolladores de software pueden agregar hipervínculos dentro de sus documentos de presentación de PowerPoint. 

      title_right: "Cómo agregar hipervínculos en presentaciones"
      content_right: |
        * Configuración de archivos de presentación de origen y destino
        * Establecer Uri y mostrar expresiones de texto
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "49e1ca9eccc41942372c23c14f98ecef"
      gistfile: "insert_hyperlinks_in_presentation_documents.cs"

    - title_left: ".NET API para insertar hipervínculos en correos electrónicos"
      content_left: |
       GroupDocs.Assembly .NET API permite a los profesionales del software insertar hipervínculos dentro de sus documentos de correo electrónico. El siguiente código .NET demuestra la facilidad con la que los programadores pueden agregar hipervínculos a sus mensajes de correo electrónico y enviarlos a otros usuarios desde sus propias aplicaciones .NET. 

      title_right: "Agregar hipervínculos a documentos de correo electrónico"
      content_right: |
        * Configuración de archivos de hoja de cálculo de origen y destino
        * Establecer Uri y mostrar expresiones de texto
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) para ensamblar el documento. es compatible
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "8c119b4faa0334179854e164d87d3e7b"
      gistfile: "insert_hyperlinks_in_email_documents.cs"  

    - title_left: "Requisitos del sistema"
      content_left: |
        Las API de GroupDocs.Assembly .NET son compatibles con todas las principales plataformas y sistemas operativos. Para obtener una guía completa de requisitos del sistema, visite [requisitos del sistema](https://docs.groupdocs.com/assembly/net/system-requirements/) Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema:
         * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
         * Entorno de desarrollo: Visual Studio, Xamarin, MonoDevelop, etc.
         * Marcos: .NET Framework, .NET Standard, .NET Core, Mono
         * Obtenga la última versión de las API GroupDocs.Assembly .NET de [NuGet](https://www.nuget.org/packages/GroupDocs.Assembly/)
        
      title_right: "Por qué usar GroupDocs.Assembly"
      content_right: |
        * Permita a los usuarios crear documentos personalizados a partir de plantillas.
        * No se requiere software adicional para crear y automatizar documentos
        * Capacidad para generar un documento de salida basado en la fuente de datos
        * Insertar dinámicamente el contenido del documento en el informe
        * Adjunte dinámicamente archivos adjuntos de correo electrónico e inserte hipervínculos en informes
        * Eliminación automática de párrafos vacíos
        * Soporte completo para múltiples formatos de datos
        * Soporte de archivos adjuntos de correo electrónico dinámico

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---