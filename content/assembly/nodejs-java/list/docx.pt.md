



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: pt
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Crie Listas Dinâmicas em DOCX com JavaScript"
head_description: "Projete e insira listas em templates DOCX utilizando a API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Incorpore Listas Baseadas em Dados em Arquivos DOCX com Node.js" 
description: "GroupDocs.Assembly for Node.js via Java oferece ferramentas poderosas para adicionar listas flexíveis e impulsionadas por dados a documentos DOCX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comece Grátis"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) simplifica a criação de documentos extraindo dados de diversas fontes e incorporando-os em templates. Use-o para construir listas, tabelas, gráficos e outros elementos, com opções de formatação e posicionamento precisas. Suportando mais de 50 formatos, incluindo PDF, MS Office e emails, ajuda a automatizar seu processo de geração de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para Inserir uma Lista em um Arquivo DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita a adição de listas detalhadas e baseadas em dados aos seus templates DOCX.
      
      1. Crie um template DOCX e defina marcadores de posição para a lista.
      2. Forneça o caminho do arquivo do template.
      3. Carregue dados de fontes suportadas, como JSON ou XML.
      4. Salve o documento com a lista gerada.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de exemplo"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // Coloque esta tag em seu template para marcar onde a lista irá.
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Defina o caminho do arquivo para seu template.
        const template = "list_template.docx";

        // Busque dados da fonte que deseja usar.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Salve o arquivo com a lista incorporada.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Gere Documentos com Dados Integrados"
  description: "Com GroupDocs.Assembly for Node.js via Java, você pode incorporar listas, tabelas, gráficos e outros elementos em templates, economizando tempo e esforço."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Destaques do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere Relatórios de Múltiplas Fontes de Dados"
      content: "Importe dados de JSON, XML, CSV ou outros formatos para preencher listas e outros componentes de forma eficiente."

    # feature loop
    - title: "Adicione Listas e Outros Elementos Visuais"
      content: "GroupDocs.Assembly permite incorporar listas, tabelas, gráficos e mais ao lado de texto, imagens e links para resultados polidos."

    # feature loop
    - title: "Posicione e Estilize Dados Precisamente"
      content: "Templates baseados em LINQ permitem controlar exatamente onde listas e outros dados aparecem, utilizar loops para itens repetidos e personalizar estilos de acordo com suas necessidades."

    # feature loop
    - title: "Funciona em Vários Formatos"
      content: "Crie documentos em formatos como MS Office, PDF, OpenOffice, HTML e emails. Mescle conteúdo de várias fontes em um único arquivo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crie Programaticamente uma Lista em um Documento"
      content: |
        Este exemplo demonstra como adicionar dinamicamente uma lista a um documento DOCX usando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Adicione um marcador de posição em seu template para a lista.
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifique o caminho do arquivo do template.
          const template = "numlist_template.docx";

          // Carregue dados para preencher a lista.
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // Prepare a fonte de dados com os detalhes necessários.
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // Inicialize o DocumentAssembler.
          const asm = new assemblyLib.DocumentAssembler();

          // Salve o documento final com a lista incluída.
          asm.assembleDocument(template, "result.docx", data);
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar o resultado"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.docx"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Explore os recursos do GroupDocs.Assembly gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar do NPM"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "Saiba mais sobre licenciamento"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explore as Funcionalidades do GroupDocs.Assembly"
    exclude: "list"
    description: "Desenhe e gere documentos ricos em dados sem esforço utilizando ferramentas de integração poderosas."
    items: 
          
        # operation loop 1
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Criar e adicionar códigos de barras a documentos dinamicamente"

        # operation loop 2
        - name: "Visualizar dados com diagramas"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Preencher vários tipos de diagramas com dados"

        # operation loop 3
        - name: "Mesclar documentos"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Combinar o conteúdo de um documento em outro"

        # operation loop 4
        - name: "Mostrar dados com listas"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Gerar listas em documentos usando dados específicos"

        # operation loop 5
        - name: "Organizar dados em tabelas"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Recuperar dados de qualquer fonte e preencher tabelas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Crie Documentos em Vários Formatos"
    exclude: "DOCX"
    description: "Node.js via Java suporta mais de 50 formatos de arquivo, facilitando a fusão de templates e dados em resultados profissionais."
    items: 
          
        # format loop 1
        - name: "Criar uma lista em um PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Criar uma lista em um DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Criar uma lista em um PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Criar uma lista em um XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---