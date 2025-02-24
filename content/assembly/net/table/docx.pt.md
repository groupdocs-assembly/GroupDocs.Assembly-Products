



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: pt
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Crie tabelas em documentos DOCX com C#"
head_description: "A API GroupDocs.Assembly for .NET permite que os desenvolvedores adicionem e preencham tabelas em documentos e e-mails com dados de fontes dinâmicas."

############################# Header ############################
title: "Gere tabelas de dados em documentos DOCX usando nossa API .NET" 
description: "GroupDocs.Assembly for .NET facilita o preenchimento dinâmico de tabelas em documentos DOCX com dados de várias fontes."
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
    title: "Visão Geral do GroupDocs.Assembly for .NET"
    link: "/assembly/net/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) foi desenvolvido para criar documentos e relatórios preenchendo modelos com dados de múltiplas fontes. Insira dados estruturados em tabelas, listas e gráficos de forma simples, ou insira imagens dinamicamente. A sintaxe avançada garante a colocação precisa dos dados. Suporta mais de 50 formatos, incluindo PDFs, documentos MS Office e arquivos de e-mail.

############################# Steps ############################
steps:
    enable: true
    title: "Como preencher uma tabela em um documento DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/net/) permite que você preencha dinamicamente tabelas em modelos para formatos como DOCX. Insira dados de várias fontes nas suas tabelas.
      
      1. Crie um modelo DOCX com espaços reservados para a tabela.
      2. Recupere dados de qualquer fonte suportada.
      3. Filtre os dados para incluir apenas as informações necessárias.
      4. Salve o documento com a tabela preenchida.
   
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
        // Adicione essas tags em uma linha de tabela do modelo
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Defina o caminho do arquivo para o modelo
        string template = "table_template.docx";

        // Recupere dados de uma fonte suportada
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Salve o documento com a tabela preenchida com dados
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Gere documentos com tabelas dinâmicas"
  description: "GroupDocs.Assembly for .NET simplifica a criação de documentos ao automatizar o preenchimento de tabelas e suportar elementos adicionais como gráficos, listas e imagens através de modelos e marcação avançada."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Principais Características do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crie relatórios a partir de dados estruturados"
      content: "A API processa dados de fontes como JSON, XML e CSV para preencher tabelas em documentos de escritório de forma eficiente e precisa."

    # feature loop
    - title: "Exiba dados visualmente"
      content: "GroupDocs.Assembly possibilita a criação de tabelas, listas e gráficos, além de embutir texto, links e imagens para um design profissional de documentos."

    # feature loop
    - title: "Posicione precisamente os dados da tabela"
      content: "Utilize uma sintaxe baseada em LINQ para adicionar dinamicamente linhas e colunas à tabela. Personalize estilos, incluindo cores e formatação, programaticamente."

    # feature loop
    - title: "Suporta uma ampla gama de formatos"
      content: "Gerencie facilmente formatos de arquivo populares como MS Office, OpenOffice, PDF e HTML. Insira tabelas preenchidas de forma integrada em tipos de documentos suportados."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como preencher dinamicamente uma tabela de dados"
      content: |
        Este exemplo demonstra como preencher uma tabela em um documento DOCX usando dados dinâmicos.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepare um modelo com um espaço reservado para a tabela
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // Especifique o caminho do arquivo para o modelo
          string template = "table_template.docx";

          // Recupere dados da fonte escolhida
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crie um objeto de fonte de dados com os dados necessários
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Inicialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o documento finalizado com a tabela preenchida
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    title: "Explore principais recursos"
    exclude: "table"
    description: "Nossa solução simplifica a criação de documentos profissionais com tabelas populadas dinamicamente e elementos adicionais."
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
    title: "Crie relatórios com tabelas detalhadas"
    exclude: "DOCX"
    description: ".NET permite a criação de relatórios abrangentes preenchendo modelos com tabelas e outros elementos de dados em mais de 50 formatos suportados."
    items: 
          
        # format loop 1
        - name: "Adicionar uma tabela a um PDF"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Adicionar uma tabela a um DOCX"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Adicionar uma tabela a um PPTX"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Adicionar uma tabela a um XLSX"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---