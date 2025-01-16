



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:02
draft: false
lang: pt
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Mesclar Documentos em PPTX com JavaScript"
head_description: "Combine arquivos PPTX usando JavaScript. GroupDocs.Assembly simplifica a mesclagem de documentos em apenas alguns passos simples."

############################# Header ############################
title: "Combine Conteúdo em Arquivos PPTX de Forma Eficiente" 
description: "Com GroupDocs.Assembly for Node.js via Java, integrar um arquivo PPTX a outro é rápido e preciso. Desfrute de ferramentas flexíveis e confiáveis para uma mesclagem perfeita."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Experimente Gratuitamente"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Visão Geral do GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) oferece uma maneira poderosa de gerenciar documentos. Mescle um arquivo em outro com eficiência, suportando mais de 50 formatos, como PDF e MS Office. Personalize layouts, edite conteúdo e organize documentos exatamente como necessário.

############################# Steps ############################
steps:
    enable: true
    title: "Como Mesclar um Documento em um Arquivo PPTX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita a inserção de um arquivo PPTX em outro com opções personalizáveis.
      
      1. Desenhe um template PPTX com espaços reservados para o conteúdo.
      2. Defina o caminho do arquivo para o template.
      3. Forneça o caminho do arquivo para mesclar.
      4. Exporte o arquivo final com o conteúdo combinado.
   
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
        // Insira esta tag em seu template para definir onde o documento será incorporado
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Defina o caminho do arquivo para o template principal
        const template = "doc_template.pptx";

        // Forneça o caminho do documento que deseja mesclar
        const data 
            = new assemblyLib.DataSourceInfo("insert.pptx", "doc_expression");

        // Salve a saída final com o documento incorporado
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Ferramentas Poderosas para Integração de Documentos"
  description: "GroupDocs.Assembly for Node.js via Java torna a incorporação de arquivos em diversos formatos fácil e totalmente personalizável. Forneça resultados consistentes e profissionais a cada vez."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere Relatórios com Dados Empresariais"
      content: "Extraia dados de fontes JSON, XML ou CSV para criar relatórios e documentos abrangentes de forma rápida e precisa."

    # feature loop
    - title: "Adicione Elementos Visuais Ricos"
      content: "GroupDocs.Assembly permite incluir tabelas, gráficos, listas, imagens e códigos de barras junto com texto e hyperlinks."

    # feature loop
    - title: "Posicionamento Preciso de Dados"
      content: "Utilize templates LINQ para posicionar os dados exatamente onde pertencem, lidar com itens repetidos como arrays e personalizar estilos de maneira eficiente."

    # feature loop
    - title: "Funciona com uma Variedade de Formatos"
      content: "Mescle conteúdo de forma contínua em formatos como PDFs, arquivos do MS Office, HTML e OpenOffice, oferecendo flexibilidade para todos os projetos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Incorpore uma Imagem em um Documento Programaticamente"
      content: |
        Este exemplo demonstra como inserir uma imagem em um arquivo PPTX usando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Adicione um espaço reservado no template para a imagem
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifique o caminho para o arquivo do template
          const template = "template.pptx";

          // Defina o caminho para a imagem que deseja incorporar
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // Inicialize o objeto DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Salve o documento com a imagem incluída
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
            link: "/examples/assembly/formats/assembly_document.pptx"
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
    title: "Recursos Essenciais em Resumo"
    exclude: "document"
    description: "Explore as ferramentas abrangentes que GroupDocs.Assembly oferece para uma mesclagem de documentos eficiente e sem problemas."
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
    title: "Combine Documentos em Vários Formatos"
    exclude: "PPTX"
    description: "Use Node.js via Java para mesclar conteúdo em mais de 50 formatos de arquivo, garantindo resultados profissionais e acabados."
    items: 
          
        # format loop 1
        - name: "Incorporar um documento em um PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Incorporar um documento em um DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Incorporar um documento em um PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Incorporar um documento em um XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---