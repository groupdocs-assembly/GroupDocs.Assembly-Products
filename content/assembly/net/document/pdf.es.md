---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/net/document/pdf/"
otherformats: HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Inserte el contenido del documento externo en los correos electrónicos y el archivo PDF a través de la API de .NET"
head_description: "GroupDocs.Assembly .NET API permite a los programadores insertar dinámicamente el contenido del documento externo en PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG y otros formatos de archivo."

############################# Header ############################
title: "Inserte el contenido del documento externo en archivos de Office y mensajes de correo electrónico a través de la API de .NET"
description: "GroupDocs.Assembly .NET API es totalmente compatible con la inserción dinámica del contenido de documentos externos en informes, correos electrónicos y documentos de Office como PDF DOCX, XLSX, CSV, PPTX, MSG y más."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo insertar el contenido del documento externo en otros archivos, informes y correos electrónicos a través de .NET?"
    content: |
       Un documento o archivo de documento hace referencia a un conjunto de información digital y no digital que el usuario puede recuperar en una etapa posterior. Un documento informático o digital es un archivo creado por una aplicación de software que se puede almacenar dentro de un sistema informático. Por lo general, se utiliza un procesador de textos o un editor de texto para crear un documento electrónico en un sistema informático. GroupDocs.Assembly para .NET es una API muy útil que ayuda a los desarrolladores de software a crear un potente software de aplicación que se puede usar para crear y administrar sus documentos con facilidad. Permite a los desarrolladores de software insertar dinámicamente el contenido de un documento externo en informes, correos electrónicos y documentos de Office. Proporcionó compatibilidad con algunos de los tipos de documentos más utilizados, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint y muchos más. Además, algunas funciones avanzadas relacionadas con la inserción y edición de contenido de documentos son totalmente compatibles, como insertar contenido en una página de documento, insertar en celdas de hoja de cálculo, editar o reemplazar contenido, insertar contenido en una diapositiva de presentación y muchas más.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Inserte el contenido del documento externo en un archivo de Word a través de .NET"
      content_left: |
       GroupDocs.Assembly .NET API permite a los desarrolladores de software insertar fácilmente el contenido de un documento externo en varios tipos de documentos y mensajes de correo electrónico. El siguiente ejemplo de código .NET muestra cómo insertar el contenido de un documento externo en un documento de procesamiento de Word con solo un par de líneas de código.

      title_right: "Cómo agregar el contenido del documento al archivo PDF"
      content_right: |
        * Establecer plantilla de documento abierto de origen
        * Establecer informe de documento abierto de destino
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) para generar un informe en formato de documento abierto. es compatible
          * Carga un documento de plantilla desde la ruta de origen especificada
          * Rellena el documento de plantilla con datos de las fuentes únicas o múltiples especificadas
          * Almacena el documento de resultados en la ruta de destino utilizando las LoadSaveOptions proporcionadas.
          * Información sobre objetos de origen de datos.

      gisthash: "c4dc0be4f8ab8c2ba4ee6a78673ca1cd"
      gistfile: "dynamic_documents_insertion_to_word_processing.cs"

    - title_left: "Inserte el contenido del documento externo en correos electrónicos a través de .NET"
      content_left: |
       GroupDocs.Assembly .NET API permite agregar y administrar varios tipos de documentos y contenidos dentro de los documentos. Permite insertar dinámicamente el contenido de un documento externo en varios tipos de documentos y formatos de archivo de correo electrónico. El siguiente código de C# muestra la facilidad con la que los usuarios pueden insertar el contenido de un documento externo en sus documentos y mensajes de correo electrónico dentro de sus propias aplicaciones .NET. 

      title_right: "Agregue el contenido del documento a un mensaje de correo electrónico a través de C#"
      content_right: |
        * Establecer plantilla de documento abierto de origen
        * Establecer informe de documento abierto de destino
        * Crear una instancia de la clase [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) para generar un informe en formato de documento abierto. es compatible
          * Carga un documento de plantilla desde la ruta de origen especificada
          * Rellena el documento de plantilla con datos de las fuentes únicas o múltiples especificadas
          * Almacena el documento de resultados en la ruta de destino utilizando las LoadSaveOptions proporcionadas.
          * Información sobre objetos de origen de datos.

      gisthash: "8fe014550c5f05467da6910a7ee16f18"
      gistfile: "dynamic_documents_insertion_to_emails_dotnet.cs"

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