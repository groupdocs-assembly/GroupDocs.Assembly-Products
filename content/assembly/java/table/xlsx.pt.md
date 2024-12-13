



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:56
draft: false
lang: pt
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adicione tabelas a documentos XLSX usando Java"
head_description: "Com GroupDocs.Assembly for Java, os desenvolvedores podem integrar rapidamente tabelas em documentos e emails, puxando dados de fontes dinâmicas."

############################# Header ############################
title: "Preencha tabelas em arquivos XLSX com nossa API Java" 
description: "GroupDocs.Assembly for Java simplifica o processo de preenchimento de tabelas em documentos XLSX com dados de várias entradas."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenha Seu Teste Gratuito"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) é uma ferramenta para gerar documentos e relatórios inserindo automaticamente dados em modelos pré-projetados. Você pode adicionar tabelas, listas, gráficos e imagens. Seus recursos avançados permitem posicionar o conteúdo com precisão dentro dos seus documentos. Compatível com mais de 50 tipos de arquivos, incluindo PDF, MS Office e formatos de email.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para inserir dados em uma tabela XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) ajuda você a preencher modelos de tabela para XLSX e outros formatos. Use dados dinâmicos de suas fontes para criar tabelas de forma eficiente.
      
      1. Configure um modelo XLSX com espaços reservados para linhas e colunas da tabela.
      2. Extraia dados de qualquer fonte de entrada suportada.
      3. Filtre ou pré-processe os dados para atender suas necessidades.
      4. Gere o documento final com a tabela completa.
   
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
        // Use essas tags em um espaço reservado de linha de tabela dentro do seu modelo
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // Defina o caminho para o arquivo de modelo
        String template = "table_template.xlsx";

        // Carregue dados da sua fonte escolhida
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // Salve o arquivo de saída com a tabela preenchida
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Crie documentos com tabelas preenchidas com dados"
  description: "GroupDocs.Assembly for Java torna simples a automação da criação de tabelas em seus documentos. Ele também suporta a adição de elementos como gráficos, listas e imagens usando modelos."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "Principais Recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Gere relatórios a partir de múltiplos formatos de dados"
      content: "A API opera de forma integrada com JSON, XML, CSV e outros formatos para preencher tabelas em seus documentos com dados organizados."

    # feature loop
    - title: "Apresente informações visualmente"
      content: "GroupDocs.Assembly ajuda a construir tabelas, listas e gráficos profissionais, além de inserir links, textos e imagens, para um visual refinado."

    # feature loop
    - title: "Coloque o conteúdo da tabela com precisão"
      content: "Use uma sintaxe flexível baseada em LINQ para adicionar linhas e colunas dinamicamente. Personalize a aparência, como estilos e cores de fonte, programaticamente."

    # feature loop
    - title: "Compatível com múltiplos formatos"
      content: "Trabalhe com MS Office, OpenOffice, PDF, HTML e mais. Mescle tabelas em qualquer formato de arquivo suportado sem esforço."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crie dinamicamente uma tabela preenchida com dados"
      content: |
        Este exemplo mostra como preencher uma tabela em um documento XLSX usando dados de entrada dinâmicos.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Desenhe um modelo com um espaço reservado para a tabela
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // Defina a localização do arquivo de modelo
          String template = "table_template.xlsx";

          // Carregue dados da sua fonte preferida
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Prepare um objeto de dados contendo os campos necessários
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Crie uma instância de DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o documento com a tabela preenchida
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
            link: "/examples/assembly/formats/assembly_table.xlsx"
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
    title: "Principais recursos em um relance"
    exclude: "table"
    description: "Nossa API simplifica a criação de documentos profissionais, automatizando o preenchimento de tabelas juntamente com outros componentes poderosos."
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
    title: "Produza tabelas detalhadas em vários formatos"
    exclude: "XLSX"
    description: "Com Java, você pode preencher modelos com dados e gerar relatórios detalhados em mais de 50 tipos de arquivos."
    items: 
          
        # format loop 1
        - name: "Adicionar uma tabela a um PDF"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Adicionar uma tabela a um DOCX"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Adicionar uma tabela a um PPTX"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Adicionar uma tabela a um XLSX"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---