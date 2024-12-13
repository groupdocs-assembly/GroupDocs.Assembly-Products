



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: pt
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Inserir um documento em outro no XLSX usando Java"
head_description: "Combine arquivos XLSX com Java. O GroupDocs.Assembly simplifica o processo de mesclagem de documentos em apenas algumas linhas de código."

############################# Header ############################
title: "Incorpore conteúdo em arquivos XLSX sem complicações" 
description: "Use o GroupDocs.Assembly for Java para inserir um documento XLSX em outro de forma integrada. Obtenha resultados precisos com ferramentas flexíveis e confiáveis."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenha gratuitamente"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é o GroupDocs.Assembly for Java?"
    link: "/assembly/java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) é uma solução versátil para o manuseio de documentos. Ele permite integrar um documento a outro de forma eficiente, com suporte a mais de 50 formatos, como PDFs e arquivos do MS Office. Personalize sua saída mesclando, editando e organizando o conteúdo exatamente como desejar.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para inserir um documento em um arquivo XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) torna a incorporação de um documento XLSX em outro simples e personalizável.
      
      1. Prepare um template XLSX com marcadores para o conteúdo incorporado.
      2. Especifique o caminho do arquivo para o template.
      3. Forneça o caminho do arquivo para o documento a ser incorporado.
      4. Salve o arquivo de saída com o conteúdo mesclado.
   
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
        // Use esta tag em seu template para marcar o local do documento incorporado
        // <<doc [doc_expression]>>

        // Defina o caminho do arquivo para o template principal
        String template = "doc_template.xlsx";

        // Forneça o caminho para o documento que deseja inserir
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // Salve o arquivo final com o conteúdo incorporado
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Ferramentas avançadas para simplificar a integração de documentos"
  description: "Com o GroupDocs.Assembly for Java, incorporar documentos é simples e personalizável, independentemente do tipo de arquivo. Alcance resultados limpos e consistentes em seus projetos."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "Destaques do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Crie relatórios usando dados de negócios"
      content: "Preencha documentos com dados de fontes como JSON, XML ou CSV de forma rápida e confiável, otimizando seus fluxos de trabalho."

    # feature loop
    - title: "Melhore documentos com conteúdo visual"
      content: "O GroupDocs.Assembly permite inserir tabelas, gráficos e listas ao lado de texto, hyperlinks, imagens e até mesmo códigos de barras dinâmicos."

    # feature loop
    - title: "Coloque os dados exatamente onde pertencem"
      content: "Os templates LINQ ajudam a posicionar seus dados com precisão, gerenciando elementos repetidos como arrays e aplicando estilos personalizados sem dificuldades."

    # feature loop
    - title: "Compatível com diversos formatos de arquivo"
      content: "Mescle documentos em vários formatos, incluindo PDFs, HTML, arquivos do MS Office e OpenOffice, garantindo flexibilidade para seus projetos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como inserir programaticamente uma imagem em um documento"
      content: |
        Este exemplo mostra como incorporar uma imagem em um arquivo XLSX usando o GroupDocs.Assembly.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Adicione uma tag de marcador no arquivo do template
          // <<image [expression]>>

          // Defina o caminho para o template
          String template = "template.xlsx";

          // Especifique o caminho para a imagem
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // Inicialize a instância do DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o arquivo com a imagem incorporada
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
            link: "/examples/assembly/formats/assembly_document.xlsx"
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
    title: "Principais capacidades de uma olhada"
    exclude: "document"
    description: "Descubra os amplos recursos que o GroupDocs.Assembly oferece para tornar a integração e combinação de documentos eficientes e sem complicações."
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
    title: "Mescle diferentes tipos de documentos"
    exclude: "XLSX"
    description: "Com Java, você pode incorporar e combinar conteúdos em mais de 50 formatos de arquivo. Adicione arquivos de forma integrada para criar resultados profissionais."
    items: 
          
        # format loop 1
        - name: "Incorporar um documento em um PDF"
          format: "PDF"
          link: "/assembly/java/document/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Incorporar um documento em um DOCX"
          format: "DOCX"
          link: "/assembly/java/document/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Incorporar um documento em um PPTX"
          format: "PPTX"
          link: "/assembly/java/document/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Incorporar um documento em um XLSX"
          format: "XLSX"
          link: "/assembly/java/document/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---