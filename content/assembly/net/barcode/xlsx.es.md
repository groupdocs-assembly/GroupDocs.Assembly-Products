---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/assembly/net/barcode/xlsx/"
otherformats: XLS XLT XLSM XLTX XLTM XLSB ODS 

############################# Head ############################
head_title: "Cómo generar y agregar códigos de barras en una hoja de cálculo de Excel a través de C#, ASP.NET"
head_description: "GroupDocs.Assembly .NET API admite la creación e inserción de imágenes de códigos de barras dentro de documentos de hojas de cálculo de Excel (XLS, XLT, XLSX, XLSM, XLTX, XLTM y XLSB)."

############################# Header ############################
title: "Creación y gestión de códigos de barras en XLSX hoja de cálculo a través de la API de .NET"
description: "Usando GroupDocs.Assembly .NET API, los desarrolladores de software pueden crear y administrar dinámicamente imágenes de código de barras en documentos Excel XLSX Spreadsheet dentro de aplicaciones C#, ASP.NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo agregar la generación de código de barras para hojas de cálculo?"
    content: |
       Esta página proporciona información sobre cómo generar códigos de barras en una hoja de cálculo de Excel utilizando la API de .NET. Los códigos de barras son códigos digitales que almacenan información legible por máquina que normalmente se utiliza para la identificación rápida de una gran cantidad de artículos. Aporta velocidad y precisión a su sistema, lo que reduce automáticamente el tiempo de una operación. GroupDocs.Assembly es una potente API de .NET que permite a los desarrolladores de software dibujar mediante programación numerosas imágenes de códigos de barras 1D y 2D con texto personalizado, apariencia y diferentes tipos de codificación dentro de la hoja de cálculo de Microsoft Excel en una ubicación particular. La API también facilita la administración del tamaño de la imagen del código de barras, los colores de primer plano y de fondo, el tamaño de la fuente, la resolución de la imagen, la corrección automática de texto y más. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Generación de Códigos de Barras en XLSX Hojas de Cálculo a través de .NET"
      content_left: |
       GroupDocs.Assembly .NET brinda soporte completo para agregar y administrar códigos de barras dentro de la hoja de cálculo XLSX. El siguiente ejemplo de código C# .NET demuestra cómo generar e insertar imágenes de código de barras dentro de un documento de hoja de cálculo de Microsoft Excel.

      title_right: "Cómo usar imágenes de código de barras en XLS"
      content_right: |
        * Cree una instancia de [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler)
        * Llame al método [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) con los siguientes parámetros
          * Stream para leer un documento de plantilla.
          * Stream para escribir el documento resultante.
          * Opciones adicionales para cargar y guardar documentos.
          * Información sobre objetos de origen de datos.

      gisthash: "8576f622912b355ce69966077033dcac"
      gistfile: "generate_barcodes_in_spreadsheets.cs"

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