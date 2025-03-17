---
############################# Static ############################
layout: "family"
date:  2025-03-17T13:11:11
draft: false

product: "Assembly"
product_tag: "assembly"

lang: es

############################# Head ############################
head_title: "APIs de .NET, Java, Node.js y Aplicaciones de Documentos en Línea de GroupDocs"
head_description: "Obtén una solución integral de automatización de documentos e informes para aplicaciones .NET, Java y Node.js. Genera todos los documentos comunes a partir de plantillas y datos personalizados."

############################# Header ############################
title: "Solución de Automatización de Documentos y Generación de Informes"
description:  |
  Crea informes detallados usando plantillas y fuentes de datos con nuestras aplicaciones y APIs multiplataforma.

  Genera informes en formatos como Word, Excel, Presentaciones y muchos más utilizando plantillas con marcado flexible.

  Puebla gráficos, códigos de barras, tablas y otros elementos con datos de fuentes como JSON, XML, CSV, etc.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Elige tu plataforma"
  title: "Independencia de plataforma"
  description: "GroupDocs.Assembly es compatible con los siguientes sistemas operativos y marcos:"
  details_link_title: "Aprende más"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Características clave de GroupDocs.Assembly"
  description: "Esta solución te ayuda a crear informes en formatos de documentos populares, automáticamente llenos de tus datos empresariales. Automatiza tus tareas de generación de documentos."

  items:
    # items loop
    - icon: "additional"
      title: "Poblar plantillas con datos"
      content: "Rellena informes usando datos de fuentes soportadas."

    # items loop
    - icon: "manipulate"
      title: "Marcado flexible"
      content: "Agrega datos a documentos de manera personalizable."

    # items loop
    - icon: "structure"
      title: "Características nativas de documentos"
      content: "Muestra datos usando tablas, gráficos y códigos de barras."

    # items loop
    - icon: "merge"
      title: "Todos los formatos populares"
      content: "Soporta todos los formatos de documentos comúnmente utilizados."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Generar informes bien personalizados"
  description: "Ejemplos de código de GroupDocs.Assembly"
  items:
    # code sample loop
    - title: "Usando Códigos de Barras Generados"
      content: |
       GroupDocs.Assembly permite el marcado de códigos de barras en plantillas de informes. Al crear un informe, se genera un código de barras basado en el marcado y datos proporcionados. Especifica la ruta a la plantilla que contiene el texto, objetos de datos y marcado. También, especifica la fuente de datos para llenar el código de barras con contenido.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Crea una instancia de la clase DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Especifica la ruta a la plantilla
            var tmp_path = "barcode_template.docx";

            //Especifica la ruta para el documento resultante
            var res_path = "result.docx";

            //Crea una instancia de la fuente de datos
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Llama a AssembleDocument para generar el informe
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Crea una instancia de la clase DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Especifica la ruta a la plantilla
            String tmp_path = "barcode_template.docx";

            //Especifica la ruta para el documento resultante
            String res_path = "result.docx";

            //Crea una instancia de la fuente de datos
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Llama a AssembleDocument para generar el informe
            assembler.assembleDocument(tmp_path, res_path, data);

            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Soporta más de 50 formatos de archivo"
  description: "GroupDocs.Assembly trabaja con casi todos los formatos de archivo populares."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Estadísticas de nuestro producto"
  description: "Explora las métricas del producto para obtener información sobre nuestro progreso, impacto y crecimiento."

  items:
    # items loop
    - number: "50+"
      title: "Formatos Soportados"
      content: "Soportamos más de 50 de los formatos de documentos más utilizados."

    # items loop
    - number: "650k"
      title: "Descargas de NuGet"
      content: "GroupDocs.Assembly para .NET es una biblioteca popular con más de 650,000 descargas en NuGet."

    # items loop
    - number: "18k"
      title: "Descargas de Maven"
      content: "Los desarrolladores de Java han descargado GroupDocs.Assembly en Maven más de 18,000 veces."

    # items loop
    - number: "150+"
      title: "Clientes Satisfechos"
      content: "Nuestros productos son confiables por desarrolladores individuales y empresas líderes en todo el mundo para crear soluciones innovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nuestros Clientes Satisfechos"
  description: "Las bibliotecas de GroupDocs son utilizadas por algunas de las marcas más renombradas y respetadas en todo el mundo."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "¿Listo para Comenzar?"
  description: "Prueba las características de GroupDocs.Assembly gratis en tu plataforma."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Preguntas Frecuentes"
  description: "Explora nuestras Preguntas Frecuentes."

  items:
    # items loop
    - question: "¿Requiere GroupDocs.Assembly alguna biblioteca externa para la composición de documentos?"
      answer: "No, GroupDocs.Assembly funciona de forma independiente y no requiere bibliotecas de terceros como Adobe Acrobat o Microsoft Office."

    # items loop
    - question: "¿Puedo probar las características de GroupDocs.Assembly antes de comprarlo?"
      answer: "¡Sí, puedes! GroupDocs.Assembly ofrece una prueba gratuita. Instálalo y explora sus características. La versión de prueba agrega 'etiquetas de prueba' a tus documentos y solo procesa las primeras 3 páginas. Para la experiencia completa, obtén una licencia temporal gratuita de 30 días para acceder a todas las funciones. Más detalles están disponibles en [licencia temporal](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "¿Qué tipos de licencias están disponibles?"
      answer: "¿Buscas una licencia para GroupDocs.Assembly? Ofrecemos una variedad de opciones para satisfacer tus necesidades. Elige según el tamaño de tu equipo, la ubicación de implementación (oficina única o remota) y si necesitas compartir el SDK/API con clientes para distribución. Alternativamente, elige una licencia de uso mensual con planes de pago por uso, pagando solo por lo que utilizas. Encuentra la mejor opción para ti en [precios](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "APIs de Bajo Código de GroupDocs.Assembly"
  description: "Genera documentos usando tu aplicación a través de nuestra API REST basada en la nube."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Utiliza la API RESTful cURL para agregar datos a Word, Excel, PowerPoint y muchas otras plantillas."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Mejora tus aplicaciones .NET generando informes a través del SDK en la Nube. Muestra datos empresariales en tu formato personalizado."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "El SDK de GroupDocs.Assembly ofrece diferentes opciones para aplicaciones Java para generar varios tipos de documentos."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Aplicaciones Web de GroupDocs.Assembly"
  description: "GroupDocs.Assembly ofrece una aplicación web gratuita para generar documentos. Puedes procesar más de 50 formatos de archivo populares directamente en tu navegador, GRATIS."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Genera informes en Excel, Word, PowerPoint y muchos otros tipos de archivos directamente desde tu navegador web."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Crea documentos de Microsoft Word a partir de plantillas y fuentes de datos."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Sube una plantilla y una fuente de datos para generar informes de Excel gratis."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---