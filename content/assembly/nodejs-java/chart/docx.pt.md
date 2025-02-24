



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: pt
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Insira Gráficos em Arquivos DOCX com JavaScript"
head_description: "Com GroupDocs.Assembly for Node.js via Java, os desenvolvedores podem criar e incorporar rapidamente gráficos dinâmicos em documentos usando fontes de dados ao vivo."

############################# Header ############################
title: "Adicione Gráficos a Arquivos DOCX Usando Node.js" 
description: "GroupDocs.Assembly for Node.js via Java simplifica o processo de integração de gráficos em documentos DOCX com entrada de dados em tempo real."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comece Grátis Hoje"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Visão Geral do GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) é uma solução robusta para a criação de documentos e relatórios automatizados. Adicione gráficos, tabelas, imagens, códigos de barras e listas aos arquivos com precisão. Esta plataforma versátil suporta mais de 50 formatos, incluindo PDFs, documentos do Office e e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para Adicionar um Gráfico a um Documento DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita a adição de gráficos a arquivos DOCX. Escolha entre tipos de gráficos como gráfico de barras, gráfico de linhas ou gráfico de pizza.
      
      1. Projete um template DOCX com espaços reservados para gráficos.
      2. Carregue dados de uma fonte suportada.
      3. Configure opções do gráfico, incluindo tipo, cores e rótulos.
      4. Exporte o documento com o gráfico incorporado.
   
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
        // Inclua esta tag em seu template para gerar um gráfico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifique o caminho do arquivo do template
        const template = "chart_template.docx";

        // Extraia dados de seu sistema de origem
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // Salve o documento final com o gráfico incorporado
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Incorpore Gráficos de Forma Eficiente em Seus Documentos"
  description: "GroupDocs.Assembly for Node.js via Java facilita a geração de documentos repletos de recursos em formatos populares. Utilize templates para adicionar gráficos, tabelas, códigos de barras, listas, imagens e muito mais com atualizações de dados em tempo real."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Principais Recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Transforme Dados em Gráficos Profissionais"
      content: "Converta dados de fontes como JSON, XML ou CSV em gráficos de alta qualidade que podem ser incorporados diretamente em documentos."

    # feature loop
    - title: "Crie Visuais Impressionantes"
      content: "Gere gráficos de barras, gráficos de pizza e gráficos de linhas que funcionam perfeitamente com outros elementos do documento, como imagens, tabelas e códigos de barras."

    # feature loop
    - title: "Estilização e Posicionamento de Gráficos Flexíveis"
      content: "Utilize templates LINQ para controlar o posicionamento e a estilização dos gráficos, incluindo cores, layouts e rótulos, para uma apresentação polida."

    # feature loop
    - title: "Suporte a Muitos Formatos de Arquivo"
      content: "Gere documentos em formatos como MS Office, PDF, OpenOffice e HTML, com gráficos perfeitamente integrados para um acabamento profissional."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Gere e Insira Gráficos Dinamicamente"
      content: |
        Este exemplo ilustra como criar e incorporar gráficos em arquivos DOCX programaticamente.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Configure um template com um espaço reservado para o gráfico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Defina o caminho para o arquivo do template
          const template = "table_template.docx";

          // Recupere dados de uma fonte escolhida
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // Prepare um objeto de dados contendo as informações do gráfico
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // Escolha o tipo de gráfico e personalize sua aparência
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // Inicialize DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salve o documento atualizado com o gráfico incorporado
          asm.assembleDocument(template, "result.docx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.docx"
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
    title: "Descubra Recursos Avançados"
    exclude: "chart"
    description: "Esta plataforma simplifica a criação de documentos com ferramentas projetadas para visualização de dados e integração tranquila."
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
    title: "Gere Relatórios em Múltiplos Formatos de Arquivo"
    exclude: "DOCX"
    description: "Node.js via Java suporta mais de 50 formatos, facilitando a combinação de templates com dados para produzir documentos refinados."
    items: 
          
        # format loop 1
        - name: "Gráficos em PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Gráficos em DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Gráficos em PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Gráficos em XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---