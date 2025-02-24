



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: pt
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Insira Tabelas em Documentos PPTX com JavaScript"
head_description: "Use o GroupDocs.Assembly for Node.js via Java para inserir rapidamente tabelas em documentos ou e-mails, extraindo dados de várias fontes."

############################# Header ############################
title: "Adicione Tabelas a Arquivos PPTX com Node.js" 
description: "Com o GroupDocs.Assembly for Node.js via Java, preencher tabelas em documentos PPTX é direto, utilizando dados de múltiplas fontes."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inicie Seu Teste Gratuito"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introdução ao GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) é uma ferramenta poderosa para automação da criação de documentos. Permite inserir tabelas, gráficos, listas e imagens em modelos, com placement de conteúdo preciso. Suporta mais de 50 formatos de arquivo, incluindo PDF, Word e e-mail, tornando mais ágil a geração de relatórios e outras tarefas.

############################# Steps ############################
steps:
    enable: true
    title: "Como Adicionar Dados a uma Tabela em PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) permite que você preencha rapidamente modelos de tabela para arquivos PPTX usando fontes de dados dinâmicas.
      
      1. Crie um modelo PPTX com espaços reservados para linhas e colunas da tabela.
      2. Carregue dados de uma fonte suportada como JSON ou CSV.
      3. Organize e formate os dados conforme necessário.
      4. Gere o documento com a tabela preenchida.
   
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
        // Inclua estas tags nos espaços reservados de linhas da tabela do seu modelo
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifique o caminho do arquivo do modelo
        const template = "table_template.pptx";

        // Carregue seus dados a partir de uma fonte escolhida
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // Salve o documento final com a tabela preenchida
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Adicione Tabelas Baseadas em Dados a Documentos"
  description: "O GroupDocs.Assembly for Node.js via Java permite aos usuários criar tabelas automaticamente, além de embutir gráficos, imagens e listas utilizando fluxos de trabalho baseados em modelos."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Principais Recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere Tabelas a Partir de Dados Estruturados"
      content: "Recupere dados de JSON, XML, CSV e outros formatos para preencher tabelas de documentos automaticamente."

    # feature loop
    - title: "Crie Conteúdo Visual Polido"
      content: "Use o GroupDocs.Assembly para projetar tabelas, gráficos e listas profissionais, além de adicionar links, imagens e texto para um visual refinado do documento."

    # feature loop
    - title: "Colocação Dinâmica de Conteúdo em Tabelas"
      content: "Adicione linhas e colunas programaticamente usando modelos baseados em LINQ, e personalize estilos como fontes, cores e alinhamentos."

    # feature loop
    - title: "Funciona Sem Interrupções em Vários Formatos"
      content: "Crie ou edite facilmente tabelas em MS Office, OpenOffice, PDF, HTML e outros formatos, integrando-as em arquivos conforme necessário."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como Preencher Programaticamente uma Tabela"
      content: |
        Este exemplo demonstra como preencher uma tabela em um documento PPTX com dados de uma fonte externa.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Projete um modelo com espaços reservados para a tabela
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifique o caminho do arquivo para o modelo
          const template = "table_template.pptx";

          // Carregue os dados necessários de sua fonte
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Organize os dados na estrutura necessária
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Inicialize o DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salve o documento de saída com a tabela preenchida
          asm.assembleDocument(template, "result.pptx", data);
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
            link: "/examples/assembly/formats/assembly_table.pptx"
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
    title: "Recursos Principais em um Relance"
    exclude: "table"
    description: "Nossa API automatiza a criação de tabelas e aprimora a geração de documentos com ferramentas e modelos versáteis."
    items: 
          
        # operation loop 1
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Criar e adicionar códigos de barras a documentos dinamicamente"

        # operation loop 2
        - name: "Visualizar dados com diagramas"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Preencher vários tipos de diagramas com dados"

        # operation loop 3
        - name: "Mesclar documentos"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Combinar o conteúdo de um documento em outro"

        # operation loop 4
        - name: "Mostrar dados com listas"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "Gerar listas em documentos usando dados específicos"

        # operation loop 5
        - name: "Organizar dados em tabelas"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Recuperar dados de qualquer fonte e preencher tabelas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Gere Tabelas em Diversos Formatos"
    exclude: "PPTX"
    description: "Com Node.js via Java, preencha modelos e crie tabelas abrangentes em mais de 50 tipos de arquivos suportados."
    items: 
          
        # format loop 1
        - name: "Adicionar uma tabela a um PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Adicionar uma tabela a um DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Adicionar uma tabela a um PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Adicionar uma tabela a um XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---