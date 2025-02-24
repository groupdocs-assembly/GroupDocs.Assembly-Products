



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: pt
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Crie gráficos em arquivos PDF com C#"
head_description: "A API GroupDocs.Assembly for .NET permite que os desenvolvedores gerem e insiram gráficos ou diagramas em documentos dinamicamente usando dados em tempo real."

############################# Header ############################
title: "Incorpore gráficos em arquivos PDF com a API .NET" 
description: "GroupDocs.Assembly for .NET oferece uma maneira poderosa de preencher arquivos PDF com dados dinâmicos e integrar gráficos de forma eficiente."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Experimente Grátis"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Assembly for .NET?"
    link: "/assembly/net/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/) é uma ferramenta projetada para otimizar a criação de documentos e relatórios ao integrar dados de várias fontes. Gere gráficos, tabelas, listas, códigos de barras e imagens dinamicamente. Opções de formatação avançadas permitem o posicionamento e a personalização precisos do seu conteúdo. Suporta mais de 50 formatos de arquivo, incluindo PDFs, documentos do MS Office e e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Como adicionar um gráfico a um documento PDF"
    content: |
      [GroupDocs.Assembly](/assembly/net/) facilita a geração e a incorporação de gráficos em seus templates PDF. Suporta uma variedade de tipos de gráficos, como gráficos de barras, pizza e linhas.
      
      1. Projete um template com locais designados para o gráfico (templates PDF não são suportados).
      2. Recupere seus dados de uma fonte compatível.
      3. Defina opções do gráfico como tipo, rótulos e esquema de cores.
      4. Exporte o documento com o gráfico como um arquivo PDF.
   
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
        // Inclua esta tag no seu template para gerar um gráfico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Especifique o caminho do arquivo para seu template
        // Atualmente, templates PDF não são suportados.
        string template = "chart_template.docx";

        // Carregue os dados da sua fonte preferida
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Salve o documento com o gráfico incorporado
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Adicione gráficos dinâmicos aos seus documentos com facilidade"
  description: "GroupDocs.Assembly for .NET simplifica a criação de documentos orientados a dados em formatos amplamente utilizados. Utilize templates para inserir gráficos, tabelas, códigos de barras, listas, hiperlinks e imagens com integração avançada de dados dinâmicos."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Principais recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Converta dados em gráficos profissionais"
      content: "Transforme dados de JSON, XML, CSV e outras fontes em gráficos visualmente atraentes com apenas alguns passos usando nossa API."

    # feature loop
    - title: "Crie conteúdo visualmente envolvente"
      content: "GroupDocs.Assembly suporta múltiplos tipos de gráficos como gráficos de barras, gráficos de pizza e gráficos de linhas. Combine estes com tabelas, códigos de barras, imagens e outros elementos para criar relatórios profissionais."

    # feature loop
    - title: "Posicione e personalize gráficos com precisão"
      content: "Com a sintaxe LINQ, você pode gerar e posicionar gráficos dinamicamente exatamente onde for necessário. Personalize facilmente estilos, cores e layouts para atender suas necessidades."

    # feature loop
    - title: "Funciona com vários formatos de arquivo"
      content: "Produza documentos em formatos populares como MS Office, PDF, OpenOffice e HTML. Incorpore gráficos de forma integrada em qualquer formato suportado com total compatibilidade."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crie um gráfico programaticamente"
      content: |
        Este exemplo demonstra como criar e incorporar dinamicamente um gráfico em um documento PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Prepare um template com um espaço reservado para o gráfico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Forneça o caminho para o arquivo do template
          // Atualmente, templates PDF não são suportados.
          string template = "table_template.docx";

          // Recupere os dados da sua fonte
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crie um objeto de dados com as informações necessárias
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configure propriedades do gráfico, como tipo e aparência
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inicialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Exporte o documento com o gráfico incluído
          asm.AssembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "Descubra as principais capacidades"
    exclude: "chart"
    description: "Nossa plataforma ajuda a criar documentos envolventes, orientados a dados, adaptados às suas necessidades."
    items: 
          
        # operation loop 1
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "Criar e adicionar códigos de barras a documentos dinamicamente"

        # operation loop 2
        - name: "Visualizar dados com diagramas"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "Preencher vários tipos de diagramas com dados"

        # operation loop 3
        - name: "Mesclar documentos"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "Combinar o conteúdo de um documento em outro"

        # operation loop 4
        - name: "Mostrar dados com listas"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "Gerar listas em documentos usando dados específicos"

        # operation loop 5
        - name: "Organizar dados em tabelas"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "Recuperar dados de qualquer fonte e preencher tabelas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crie relatórios visualmente ricos em múltiplos formatos"
    exclude: "PDF"
    description: ".NET permite gerar documentos com gráficos integrados em mais de 50 formatos suportados, combinando templates com seus dados de forma harmoniosa."
    items: 
          
        # format loop 1
        - name: "Gráficos em PDF"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Gráficos em DOCX"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Gráficos em PPTX"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Gráficos em XLSX"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---