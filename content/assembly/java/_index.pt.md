---
############################# Static ############################
layout: "landing"
date: 2024-12-13T10:30:57
draft: false

lang: pt
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"

############################# Head ############################
head_title: "Biblioteca Java para Criação, Automação & Relatórios de Documentos"
head_description: "Biblioteca Java para automação na criação de documentos e geração de relatórios. Crie documentos PDF, Word, Excel, PPTX, HTML e email utilizando templates personalizados."

############################# Header ############################
title: "API Java para Automação de Relatórios e Documentos"
description: "Simplifique a geração de relatórios em Java mesclando dados com templates."
words:
  for: "para"

actions:
  main: "Obtenha Trial via NuGet"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "Pronto para Começar?"
  description: "Experimente os recursos do GroupDocs.Assembly gratuitamente ou solicite uma licença."

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"

code:
  title: "Gerar um Gráfico em DOCX com Java"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-assembly</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}
    // Caminho para o template principal
    String template = "chart_template.docx";

    // Recuperar dados de produtividade dos gerentes a partir da fonte
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // Crie uma instância de DataSourceInfo com os dados
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // Defina as cores do gráfico utilizando outro DataSourceInfo
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // Preencha o template com dados e salve na saída
    DocumentAssembler asm = new DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visão Geral do GroupDocs.Assembly"
  description: "Uma biblioteca Java projetada para criação automatizada de documentos e integração de dados sem costura."
  features:
    # feature loop
    - title: "Mesclar Dados Comerciais em Templates com Java"
      content: "Crie relatórios profissionais facilmente incorporando dados de JSON, XML ou outras fontes em templates pré-projetados usando GroupDocs.Assembly for Java."

    # feature loop
    - title: "Trabalhar com Objetos Incorporados"
      content: "Preencha automaticamente elementos como tabelas, gráficos e diagramas em documentos utilizando dados de fontes externas."

    # feature loop
    - title: "Personalização Avançada"
      content: "GroupDocs.Assembly for Java oferece recursos flexíveis, como geração de códigos de barras, recuperação de dados online por meio de URLs e exportação de saída em diferentes formatos."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de plataforma"
  description: "GroupDocs.Assembly for Java funciona perfeitamente com sistemas operacionais, frameworks de desenvolvimento e gerenciadores de pacotes populares."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Assembly for Java suporta uma ampla gama de [formatos de documentos](https://docs.groupdocs.com/assembly/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos do Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### Imagens & Outros Formatos
        * **Portátil:** PDF
        * **Imagens:** SVG, TIFF
        * **Outros formatos de office:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### Outros formatos
        * **Web:** HTML, MHTML
        * **Emails:** EML, MSG, EMLX
        * **Outro:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "Principais Capacidades do GroupDocs.Assembly"
  description: "Crie documentos e relatórios profissionais com manipulação avançada de dados."

  items:
    # feature loop
    - icon: "preview"
      title: "Elementos de Dados Visuais"
      content: "Adicione e formate elementos como gráficos, tabelas, imagens e listas diretamente em seus documentos."

    # feature loop
    - icon: "manipulate"
      title: "Transformação de Dados"
      content: "Use fórmulas, ordenação e outras ferramentas para organizar e apresentar seus dados de forma eficaz."

    # feature loop
    - icon: "two_pages"
      title: "Suporte para Vários Formatos"
      content: "Trabalhe facilmente com tipos de arquivos comuns para templates e arquivos de saída."

    # feature loop
    - icon: "document_settings"
      title: "Formatação Avançada de Templates"
      content: "Personalize templates com opções de formatação numérica, alfabética e outras opções avançadas."

    # feature loop
    - icon: "text"
      title: "Geração Dinâmica de Códigos de Barras"
      content: "Crie rapidamente e insira imagens de códigos de barras nos documentos conforme necessário."

    # feature loop
    - icon: "add"
      title: "Estilização de Texto Flexível"
      content: "Aplique transformações de texto como maiúsculas, minúsculas ou capitalização em templates."

    # feature loop
    - icon: "manipulate"
      title: "Importação de Conteúdo Externo"
      content: "Incorpore conteúdo de arquivos externos dinamicamente durante a geração de documentos."

    # feature loop
    - icon: "convert"
      title: "Exportar em Múltiplos Formatos"
      content: "Salve documentos finais em vários formatos de arquivo usando extensões ou configurações especificadas."

    # feature loop
    - icon: "update"
      title: "Incorporação Dinâmica de Mídia"
      content: "Insira imagens ou outros conteúdos utilizando dados codificados em Base64 ao criar documentos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemplos de código"
  description: "Explore exemplos de código para tarefas comuns com GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Crie uma Lista com Marcadores em Word"
      content: |
        Saiba como adicionar [listas com marcadores](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/) aos documentos Word para uma representação organizada de dados. Este exemplo mostra como gerar uma lista em Word usando GroupDocs.Assembly.
        {{< landing/code title="Crie uma Lista com Marcadores em Word">}}
        ```java {style=abap}
        // Insira este template em uma página do documento:
        // Indicadores de desempenho dos gerentes
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Especifique o caminho do template
        String template = "Bulleted List Template.docx";

        // Defina o caminho do arquivo de saída
        String result = "Result Report.docx"

        // Recupere dados dos gerentes de uma fonte JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Gere o relatório com os dados preenchidos
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Crie Gráficos de Pizza em PPTX"
      content: |
        Use templates e XML para adicionar [gráficos de pizza](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/) às suas apresentações. Torne seus relatórios mais envolventes ao incluir gráficos de pizza para visualizar dados.
        {{< landing/code title="Crie Gráficos de Pizza em PPTX">}}
        ```java {style=abap}   
        // Adicione o template do título do gráfico à apresentação:
        // Receita dos clientes <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Inclua também o template de dados do gráfico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Especifique o caminho do template do gráfico
        String template = "Pie Chart Template.pptx";

        // Defina o caminho do arquivo de saída
        String result = "Result Report.pptx"

        // Recupere os dados dos clientes de uma fonte XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Gere o gráfico e salve o resultado
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---