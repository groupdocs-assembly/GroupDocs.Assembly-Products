---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/net/barcode/md/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OXPS EML EMLX MSG 

############################# Head ############################
head_title: "Cree y agregue imágenes de códigos de barras en documentos y correos electrónicos a través de .NET"
head_description: "GroupDocs.Assembly .NET API permite a los desarrolladores generar e insertar dinámicamente imágenes de códigos de barras dentro de documentos (PDF DOC, DOCX, RTF, XLSX, CSV, PPTX) y mensajes de correo electrónico con facilidad."

############################# Header ############################
title: "Genere e inserte imágenes de código de barras en mddocumentos UPPER a través de la API de .NET"
description: "GroupDocs.Assembly .NET brinda soporte completo para la creación, edición y adición de imágenes dinámicas de códigos de barras dentro de documentos MD usando C# y VB.NET API."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo realizar la generación de imágenes de código de barras en documentos?"
    content: |
       Esta página ayudará a los usuarios a comprender y aprender cómo generar e insertar dinámicamente imágenes de códigos de barras en sus documentos y mensajes de correo electrónico dentro de C#, ASP.NET y otras aplicaciones relacionadas con .NET. GroupDocs.Assembly .NET es una API muy poderosa que brinda a los usuarios la capacidad de automatizar y generar informes en muchos formatos de archivo líderes dentro de sus propias aplicaciones .NET sin dependencias externas. Admite algunos formatos de archivo muy comunes, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint y diapositivas. Es totalmente compatible con algunas simbologías de códigos de barras lineales y 2D comunes. También puede personalizar fácilmente el tamaño de la imagen del código de barras, los colores frontal y posterior, la fuente y la ubicación del texto del código de barras, configurar la resolución de la imagen del código de barras y más. También admite la creación de documentos personalizados a partir de plantillas y datos obtenidos de varias fuentes, como bases de datos, XML, JSON, OData, objetos y más.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Generación de Códigos de Barras en MD Documentos vía .NET"
      content_left: |
       GroupDocs.Assembly .NET brinda soporte completo para agregar y administrar códigos de barras dentro de MD documentos. El siguiente ejemplo de código C# .NET demuestra cómo generar e insertar imágenes de código de barras dentro de un documento MD. 

      title_right: "Cómo usar imágenes de código de barras en MD"
      content_right: |
        * Cree una instancia de [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) con los siguientes parámetros
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "8576f622912b355ce69966077033dcac"
      gistfile: "generate_barcodes_in_spreadsheets.cs"

    - title_left: "Establecer resolución de imagen de código de barras en MD a través de .NET"
      content_left: |
       GroupDocs.Assembly .NET brinda soporte completo para agregar y administrar códigos de barras dentro de MD documentos. Puede configurar fácilmente la resolución del código de barras con solo un par de líneas de código. El siguiente código permite a los usuarios establecer una resolución horizontal y vertical de 300 DPI. 

      title_right: "Resolución de código de barras mejorada en MD"
      content_right: |
        * Cree una instancia de [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método BarcodeSettings.Resolution para establecer la resolución de la imagen del código de barras en 300 DPI.

      gisthash: "9d8d743bd67b4bce5a4a7f1250deef26"
      gistfile: "set_barcode_image_resolution.cs"

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