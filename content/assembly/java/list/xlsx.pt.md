



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:09
draft: false
lang: pt
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Crie listas em documentos XLSX usando Java"
head_description: "Projete e insira listas dinâmicas em seus templates XLSX com a API GroupDocs.Assembly for Java."

############################# Header ############################
title: "Adicione listas dinâmicas a arquivos XLSX com nossa API Java" 
description: "GroupDocs.Assembly for Java fornece ferramentas flexíveis para gerar e inserir listas ricas em dados diretamente em documentos XLSX."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Experimente Gratuitamente"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) facilita o design de documentos profissionais extraindo dados de múltiplas fontes. Utilize para criar listas, tabelas, gráficos ou textos, posicionando esses elementos exatamente onde necessário, utilizando recursos avançados de template. Com suporte para mais de 50 formatos, incluindo PDFs, arquivos do MS Office e documentos de e-mail, ele ajuda a automatizar e agilizar seu fluxo de trabalho.

############################# Steps ############################
steps:
    enable: true
    title: "Como adicionar uma lista orientada a dados a um documento XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) permite que você insira rapidamente listas ricas em dados em templates XLSX. Personalize e organize o conteúdo com eficiência.
      
      1. Crie um template XLSX e marque os locais reservados para a lista.
      2. Defina o caminho do arquivo para o template.
      3. Extraia dados de formatos suportados como JSON ou XML.
      4. Salve o documento final com a lista adicionada.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "Documento de exemplo"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // Inclua esta tag no seu template onde a lista deve aparecer
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // Defina o caminho do arquivo do template
        String template = "list_template.xlsx";

        // Extraia dados da fonte escolhida
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // Salve o documento com a lista embutida
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Gere documentos a partir de templates com integração de dados"
  description: "GroupDocs.Assembly for Java simplifica a adição de listas dinâmicas, tabelas, gráficos e outros componentes em templates de documentos."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "Principais Recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Construa relatórios com dados de diversas fontes"
      content: "Utilize dados de formatos como JSON, XML e CSV para preencher listas e outros componentes de forma eficiente."

    # feature loop
    - title: "Adicione listas e outros elementos de dados de forma integrada"
      content: "GroupDocs.Assembly possibilita a inserção de listas, gráficos, tabelas e mais, junto a textos, imagens e links para criar documentos refinados."

    # feature loop
    - title: "Controle precisamente onde os dados aparecem"
      content: "Templates baseados em LINQ permitem definir locais exatos para suas listas e dados. Utilize loops para criar listas detalhadas automaticamente e aplicar formatação personalizada."

    # feature loop
    - title: "Suporta vários formatos de documento"
      content: "Crie ou edite arquivos em formatos como MS Office, PDF, OpenOffice, HTML e e-mail. Una conteúdos de múltiplos documentos conforme necessário."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como criar uma lista programaticamente"
      content: |
        Este exemplo mostra como adicionar uma lista dinamicamente em um arquivo XLSX usando GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Adicione uma tag de espaço reservado em seu template para a lista
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // Forneça o caminho do arquivo para o seu template
          String template = "numlist_template.xlsx";

          // Extraia os dados necessários para preencher a lista
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // Prepare a fonte de dados com os detalhes necessários
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // Inicialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o documento de saída com a lista concluída
          asm.assembleDocument(template, "result.xlsx", data);
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar o resultado"
            icon: "download"
            link: "/examples/assembly/formats/assembly_list.xlsx"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Explore os recursos do GroupDocs.Assembly gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar do Maven"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "Saiba mais sobre licenciamento"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Descubra do que GroupDocs.Assembly é capaz"
    exclude: "list"
    description: "Projete e gere documentos ricos em conteúdo com ferramentas avançadas de integração de dados."
    items: 
          
        # operation loop 1
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "Criar e adicionar códigos de barras a documentos dinamicamente"

        # operation loop 2
        - name: "Visualizar dados com diagramas"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "Preencher vários tipos de diagramas com dados"

        # operation loop 3
        - name: "Mesclar documentos"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "Combinar o conteúdo de um documento em outro"

        # operation loop 4
        - name: "Mostrar dados com listas"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "Gerar listas em documentos usando dados específicos"

        # operation loop 5
        - name: "Organizar dados em tabelas"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "Recuperar dados de qualquer fonte e preencher tabelas"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Produza documentos em vários formatos"
    exclude: "XLSX"
    description: "Java suporta mais de 50 formatos, permitindo criar documentos estruturados combinando dados e templates."
    items: 
          
        # format loop 1
        - name: "Criar uma lista em um PDF"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Criar uma lista em um DOCX"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Criar uma lista em um PPTX"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Criar uma lista em um XLSX"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---