



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: pt
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Gere gráficos em documentos XLSX usando Java"
head_description: "A API GroupDocs.Assembly for Java permite que desenvolvedores criem e insiram gráficos dinâmicos em documentos de maneira fluida, alimentados por dados ao vivo."

############################# Header ############################
title: "Adicione gráficos a documentos XLSX com a API Java" 
description: "GroupDocs.Assembly for Java simplifica o processo de incorporação de gráficos em documentos XLSX utilizando dados em tempo real."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comece Gratuitamente"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "Introdução ao GroupDocs.Assembly for Java"
    link: "/assembly/java/"
    link_title: "Saiba mais"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/) é uma solução versátil para automatizar a criação de documentos e relatórios. Permite adicionar gráficos, tabelas, listas, códigos de barras e imagens diretamente nos seus arquivos, com ferramentas avançadas para formatação precisa e integração de dados. A plataforma suporta mais de 50 formatos, incluindo PDF, arquivos do Microsoft Office e e-mails.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para incorporar um gráfico em um documento XLSX"
    content: |
      [GroupDocs.Assembly](/assembly/java/) simplifica o processo de inserção de gráficos em templates XLSX. Escolha entre uma variedade de estilos de gráfico, incluindo gráficos de barras, pizza e linhas.
      
      1. Crie um template XLSX com espaços reservados para o gráfico.
      2. Carregue seus dados de uma fonte compatível.
      3. Defina as opções do gráfico, como tipo, rótulos e cores.
      4. Salve o documento com o gráfico incluído.
   
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
        // Adicione esta tag ao seu template para incluir um gráfico
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // Forneça o caminho do arquivo para o seu template
        String template = "chart_template.xlsx";

        // Extraia os dados necessários da sua fonte
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // Salve o documento final com o gráfico embutido
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "Integre gráficos dinâmicos em seus documentos com facilidade"
  description: "GroupDocs.Assembly for Java oferece uma maneira prática de construir documentos ricos em dados em formatos populares. Use templates para inserir gráficos, tabelas, códigos de barras, listas, links e imagens com atualizações dinâmicas a partir de seus dados."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "Principais recursos do GroupDocs.Assembly"
  features:
    # feature loop
    - title: "Transforme dados em gráficos"
      content: "Utilize a API para transformar dados de JSON, XML, CSV ou outras fontes em gráficos profissionais e bem elaborados para seus documentos."

    # feature loop
    - title: "Crie conteúdo visual impactante"
      content: "GroupDocs.Assembly suporta vários formatos visuais, incluindo gráficos de barras, gráficos de pizza e gráficos de linhas, que podem ser combinados com tabelas, códigos de barras, imagens e muito mais para relatórios aprimorados."

    # feature loop
    - title: "Personalização na colocação e estilo dos gráficos"
      content: "Com uma sintaxe baseada em LINQ, você pode gerar e posicionar gráficos dinamicamente no documento, ajustando estilos, cores e layouts conforme suas necessidades de design."

    # feature loop
    - title: "Suporta múltiplos formatos de documento"
      content: "Gere documentos em formatos como MS Office, PDF, OpenOffice e HTML. Os gráficos se integram perfeitamente a qualquer formato suportado, garantindo resultados profissionais."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Gere e incorpore gráficos programaticamente"
      content: |
        Este exemplo demonstra como criar e incorporar um gráfico em um documento XLSX programaticamente.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Prepare um template com um espaço reservado para o gráfico
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // Especifique o caminho do arquivo para o template
          String template = "table_template.xlsx";

          // Carregue dados da sua fonte escolhida
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // Crie um objeto de dados com as informações relevantes
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // Configure o tipo e a aparência do gráfico
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // Inicialize DocumentAssembler
          DocumentAssembler asm = new DocumentAssembler();

          // Salve o documento final com o gráfico embutido
          asm.assembleDocument(template, "result.xlsx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.xlsx"
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
    title: "Explore capacidades poderosas"
    exclude: "chart"
    description: "Esta plataforma torna o processo de design de documentos focados em dados e visualmente atraentes mais simples, adaptando-se às suas necessidades."
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
    title: "Gere relatórios abrangentes em diversos formatos"
    exclude: "XLSX"
    description: "Java permite que você crie documentos com gráficos integrados em mais de 50 formatos de arquivo, garantindo a fusão contínua de templates e dados."
    items: 
          
        # format loop 1
        - name: "Gráficos em PDF"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "Formato de Documento Portátil da Adobe"
          
        # format loop 2
        - name: "Gráficos em DOCX"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "Documento Open XML do Microsoft Word"
          
        # format loop 3
        - name: "Gráficos em PPTX"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "Apresentação Open XML do PowerPoint"
          
        # format loop 4
        - name: "Gráficos em XLSX"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "Planilha Open XML do Microsoft Excel"


          

---