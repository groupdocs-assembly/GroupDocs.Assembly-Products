



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:03:58
draft: false
lang: pt
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Adicione Códigos de Barras a Arquivos DOCX Usando JavaScript"
head_description: "Gere e incorpore códigos de barras em seus documentos e e-mails com a API GroupDocs.Assembly for Node.js via Java."

############################# Header ############################
title: "Crie Códigos de Barras para Arquivos DOCX Usando Node.js" 
description: "Com GroupDocs.Assembly for Node.js via Java, você pode gerar, personalizar e incorporar códigos de barras dinamicamente em documentos DOCX."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Começar"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introdução ao GroupDocs.Assembly for Node.js via Java"
    link: "/assembly/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/) permite que você crie documentos profissionais combinando dados de múltiplas fontes. Adicione gráficos, tabelas, listas, imagens e códigos de barras aos seus arquivos com precisão. Utilize templates para organizar o conteúdo exatamente onde ele pertence. Funciona com mais de 50 formatos, incluindo PDFs, documentos do Office e e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para Adicionar um Código de Barras em Arquivos DOCX"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/) facilita a incorporação de códigos de barras em documentos DOCX. Suporta mais de 60 tipos de código de barras, incluindo formatos 1D e 2D.
      
      1. Crie um template DOCX com espaços reservados para códigos de barras.
      2. Recupere dados de uma fonte compatível.
      3. Defina opções de código de barras, como tamanho e resolução.
      4. Salve o documento final com o código de barras incorporado.
   
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
        // Use esta tag no template para incluir um código de barras no documento de saída
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifique o caminho para o arquivo template
        const template = "barcode_template.docx";

        // Carregue os dados necessários da sua fonte
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // Salve o documento com o código de barras aplicado
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Gere Documentos com Templates Baseados em Dados"
  description: "Com GroupDocs.Assembly for Node.js via Java, você pode criar arquivos profissionais em formatos populares incorporando perfeitamente gráficos, tabelas, listas, links, imagens e códigos de barras."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere Relatórios com Dados Empresariais"
      content: "Use a API para preencher templates com dados de formatos como JSON, XML e CSV de forma rápida e precisa."

    # feature loop
    - title: "Adicione Elementos Visuais"
      content: "GroupDocs.Assembly suporta a inserção de elementos como gráficos, tabelas, listas, texto, links, imagens e códigos de barras em tempo real."

    # feature loop
    - title: "Controle a Posicionamento dos Dados"
      content: "Com templates baseados em LINQ, você pode posicionar dados com precisão, iterar sobre arrays e aplicar formatação personalizada programaticamente."

    # feature loop
    - title: "Compatível com Vários Formatos"
      content: "Trabalhe com arquivos como documentos do MS Office, PDFs, HTML, arquivos do OpenOffice e e-mails. Mescle múltiplos documentos quando necessário."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemplo: Gere um Código de Barras Programaticamente"
      content: |
        Este exemplo demonstra como gerar e inserir programaticamente um código de barras em um documento DOCX.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // Desenhe um template com um espaço reservado para o código de barras
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // Especifique o caminho do arquivo template
          const template = "barcode_template.docx";

          // Recupere dados da sua fonte
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // Crie um objeto de fonte de dados com os detalhes necessários
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // Inicialize uma instância do DocumentAssembler
          const asm = new assemblyLib.DocumentAssembler();

          // Configure as opções do código de barras
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // Salve o documento com o código de barras incluído
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    title: "Explore Recursos Principais"
    exclude: "barcode"
    description: "Simplifique o processamento de documentos com ferramentas avançadas e capacidades de automação."
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
    title: "Formatos de Arquivo Suportados para Criação de Relatórios"
    exclude: "DOCX"
    description: "Node.js via Java lida com mais de 50 tipos de arquivo, tornando simples a mesclagem de dados e o processamento de templates para resultados de alta qualidade."
    items: 
          
        # format loop 1
        - name: "Adicionar um código de barras a um PDF"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Adicionar um código de barras a um DOCX"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Adicionar um código de barras a um PPTX"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Adicionar um código de barras a um XLSX"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---