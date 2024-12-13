



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: pt
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Incorporar um documento em outro em DOCX com a API C#"
head_description: "Mescle documentos DOCX usando C#. Com o GroupDocs.Assembly, combine arquivos de forma contínua em apenas algumas etapas."

############################# Header ############################
title: "Combine documentos no formato DOCX" 
description: "Com o GroupDocs.Assembly for .NET, você pode rapidamente incorporar um documento DOCX em outro. Esta API fornece ferramentas robustas para fusões precisas de documentos."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) é uma ferramenta poderosa para composição e manipulação de documentos. Permite aos usuários incorporar um documento em outro, possibilitando uma fusão contínua de conteúdo. Com suporte a mais de 50 formatos — incluindo PDFs, arquivos do MS Office e muito mais — você pode organizar, editar e personalizar a saída final para atender às suas necessidades.

############################# Steps ############################
steps:
    enable: true
    title: "Como mesclar um documento em um arquivo DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) permite que você incorpore rapidamente um documento em outro arquivo DOCX. Mescle e personalize o conteúdo de forma eficiente.
      
      1. Projetar um template DOCX com marcadores de posição para o documento embutido.
      2. Defina o caminho do arquivo para o template.
      3. Especifique o caminho do arquivo do documento a ser incorporado.
      4. Salve o arquivo final com o conteúdo embutido.
   
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
        // Adicione esta tag ao seu template para marcar o ponto de inserção
        // <<doc [doc_expression]>>

        // Especifique o caminho do arquivo para o template
        string template = "doc_template.docx";

        // Forneça o caminho do documento a ser incorporado
        DataSourceInfo data 
            = new DataSourceInfo("insert.docx", "doc_expression");

        // Salve o documento mesclado
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Otimize a fusão de documentos com ferramentas avançadas"
  description: "A biblioteca GroupDocs.Assembly for .NET simplifica a incorporação de um documento em outro, oferecendo suporte a vários formatos de arquivo e opções de personalização para uma integração perfeita."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Recursos principais do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere relatórios a partir dos seus dados empresariais"
      content: "Preencha automaticamente documentos com dados de JSON, XML, CSV ou outras fontes, garantindo fluxos de trabalho precisos e eficientes."

    # feature loop
    - title: "Enriqueça documentos com elementos visuais"
      content: "GroupDocs.Assembly permite incluir tabelas, gráficos e listas, além de texto, links, imagens e códigos de barras gerados dinamicamente."

    # feature loop
    - title: "Coloque e formate dados com precisão"
      content: "Templates baseados em LINQ oferecem controle sobre o posicionamento de dados, permitindo gerenciar loops para arrays e aplicar estilização, como personalização de cor."

    # feature loop
    - title: "Funciona com vários formatos de arquivo"
      content: "Incorpore documentos entre si em formatos como MS Office, PDFs, HTML, OpenOffice e muito mais."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como incorporar uma imagem em um documento programaticamente"
      content: |
        Este exemplo demonstra como inserir uma imagem em um documento DOCX usando GroupDocs.Assembly.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Adicione uma tag de marcador de posição em seu template
          // <<image [expression]>>

          // Especifique o caminho do arquivo para o template
          string template = "template.docx";

          // Defina o caminho para o arquivo de imagem
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inicialize uma instância de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o documento com a imagem incorporada
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "Descubra nossas ferramentas poderosas"
    exclude: "document"
    description: "Explore os recursos que o GroupDocs.Assembly oferece para a incorporação e fusão de documentos com precisão."
    items: 
          
        # operation loop 1
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "Criar e adicionar códigos de barras a documentos dinamicamente"

        # operation loop 2
        - name: "Visualizar dados com diagramas"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "Preencher vários tipos de diagramas com dados"

        # operation loop 3
        - name: "Mesclar documentos"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "Combinar o conteúdo de um documento em outro"

        # operation loop 4
        - name: "Mostrar dados com listas"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "Gerar listas em documentos usando dados específicos"

        # operation loop 5
        - name: "Organizar dados em tabelas"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "Recuperar dados de qualquer fonte e preencher tabelas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Mescle documentos em diversos formatos"
    exclude: "DOCX"
    description: "Com a API .NET, você pode combinar documentos em mais de 50 formatos suportados. Incorpore arquivos ou seções em seus documentos finais sem esforço."
    items: 
          
        # format loop 1
        - name: "Incorporar um documento em um PDF"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Incorporar um documento em um DOCX"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Incorporar um documento em um PPTX"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Incorporar um documento em um XLSX"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---