



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:55
draft: false
lang: pt
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Gere listas em documentos PPTX com C#"
head_description: "A API GroupDocs.Assembly for .NET permite que desenvolvedores criem e integrem dinamicamente listas preenchidas com dados em documentos e modelos."

############################# Header ############################
title: "Adicione listas baseadas em dados a documentos PPTX usando nossa API .NET" 
description: "A GroupDocs.Assembly for .NET oferece poderosas ferramentas para gerar e integrar listas dinamicamente em documentos PPTX."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar Avaliação Gratuita"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "Visão geral do GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) foi projetado para otimizar a criação de documentos e relatórios ao integrar dados de várias fontes de forma fluida. Preencha modelos com listas, gráficos, tabelas, códigos de barras ou texto, e posicione o conteúdo com precisão usando marcação avançada. Com suporte a mais de 50 formatos — incluindo PDFs, arquivos do MS Office e e-mails — é ideal para automatizar fluxos de trabalho de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para adicionar uma lista preenchida com dados a um documento PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilita a inserção de listas orientadas a dados em templates PPTX. Crie e personalize listas com precisão.
      
      1. Prepare um template PPTX com espaços reservados para a lista.
      2. Defina o caminho para o modelo.
      3. Recupere dados de fontes suportadas como JSON ou XML.
      4. Salve o documento final com a lista embutida.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de exemplo"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // Adicione esta tag ao seu modelo para marcar onde a lista aparecerá
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Especifique o caminho para o arquivo de modelo
        string template = "list_template.pptx";

        // Recupere dados da sua fonte escolhida
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Salve o documento com a lista gerada
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pptx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Crie documentos preenchendo modelos com dados estruturados"
  description: "O GroupDocs.Assembly for .NET simplifica a construção de documentos orientados a dados. Adicione listas, tabelas, códigos de barras, gráficos, imagens e outros elementos dinamicamente com templates avançados."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere relatórios a partir de dados empresariais"
      content: "A API preenche documentos em formatos populares usando dados de fontes como JSON, XML, CSV, etc., com precisão e eficiência."

    # feature loop
    - title: "Use listas e outros elementos para apresentar dados"
      content: "O GroupDocs.Assembly permite embutir listas, tabelas e gráficos juntamente com texto, códigos de barras, hyperlinks e imagens para criar documentos bem estruturados."

    # feature loop
    - title: "Insira dados precisamente onde necessário"
      content: "Aproveite a sintaxe baseada em LINQ para posicionar listas e outros elementos de dados com precisão. Use loops para preencher listas dinamicamente e aplicar formatação personalizada programaticamente."

    # feature loop
    - title: "Suporta múltiplos formatos de documento"
      content: "Gere e gerencie documentos em vários formatos, como MS Office, OpenOffice, PDF, HTML e arquivos de e-mail. Integre vários documentos em um com facilidade."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como gerar uma lista dinamicamente"
      content: |
        Este exemplo demonstra como embutir uma lista gerada dinamicamente em um documento PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Adicione uma tag de espaço reservado ao seu modelo para a lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Especifique o caminho para o arquivo de modelo
          string template = "numlist_template.pptx";

          // Recupere os dados para preencher a lista
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Crie um objeto de fonte de dados com as informações necessárias
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inicialize o DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o documento final com a lista gerada
          asm.AssembleDocument(template, "result.pptx", data);
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar o resultado"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.pptx"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Explore os recursos do GroupDocs.Assembly gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar do Nuget"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "Saiba mais sobre licenciamento"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explore as principais capacidades"
    exclude: "list"
    description: "Nossa plataforma é desenvolvida para simplificar a criação e integração de conteúdo de documentos orientados a dados."
    items: 
          
        # operation loop 1
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/pptx/"
          description: "Criar e adicionar códigos de barras a documentos dinamicamente"

        # operation loop 2
        - name: "Visualizar dados com diagramas"
          operation: "chart"
          link: "/assembly/net/chart/pptx/"
          description: "Preencher vários tipos de diagramas com dados"

        # operation loop 3
        - name: "Mesclar documentos"
          operation: "document"
          link: "/assembly/net/document/pptx/"
          description: "Combinar o conteúdo de um documento em outro"

        # operation loop 4
        - name: "Mostrar dados com listas"
          operation: "list"
          link: "/assembly/net/list/pptx/"
          description: "Gerar listas em documentos usando dados específicos"

        # operation loop 5
        - name: "Organizar dados em tabelas"
          operation: "table"
          link: "/assembly/net/table/pptx/"
          description: "Recuperar dados de qualquer fonte e preencher tabelas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crie documentos estruturados em formatos populares"
    exclude: "PPTX"
    description: "O .NET suporta mais de 50 formatos, permitindo que você mescle dados e templates de forma fluida para produzir resultados estruturados e polidos."
    items: 
          
        # format loop 1
        - name: "Criar uma lista em um PDF"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Criar uma lista em um DOCX"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Criar uma lista em um PPTX"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Criar uma lista em um XLSX"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---