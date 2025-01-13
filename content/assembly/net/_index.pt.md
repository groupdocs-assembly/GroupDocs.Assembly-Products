---
############################# Static ############################
layout: "landing"
date: 2025-01-13T15:11:22
draft: false

lang: pt
product: "Assembly"
product_tag: "assembly"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "API .NET para Automação de Documentos, Montagem & Geração de Relatórios"
head_description: "API C# .NET para automação de documentos, montagem e geração de relatórios. Crie documentos PDF, Word, Excel, PPTX, HTML e email a partir de templates personalizados."

############################# Header ############################
title: "API .NET para Automação de Documentos & Relatórios"
description: "Gere relatórios em aplicações .NET definindo templates e mesclando dados."
words:
  for: "para"

actions:
  main: "Baixar Trial via Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "Pronto para Começar?"
  description: "Experimente os recursos do GroupDocs.Assembly gratuitamente ou solicite uma licença."

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "Preencher um Gráfico em DOCX Usando C#"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // Caminho para o template principal
    string template = "chart_template.docx";

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
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visão Geral do GroupDocs.Assembly"
  description: "Solução .NET para automação na criação de documentos com integração avançada de dados."
  features:
    # feature loop
    - title: "Adicionar Dados Comerciais a Templates de Documentos com C#"
      content: "Geração de relatórios facilitada: Com GroupDocs.Assembly for .NET, você pode inserir dados de fontes como JSON ou XML em templates predefinidos com facilidade."

    # feature loop
    - title: "Processar Objetos de Dados Nativos"
      content: "Tipos de documentos suportados incluem objetos incorporados como diagramas, gráficos, tabelas e listas que podem ser preenchidos automaticamente com dados."

    # feature loop
    - title: "Recursos Adicionais"
      content: "GroupDocs.Assembly for .NET fornece amplas opções de personalização. Projete programaticamente objetos de dados, gere códigos de barra, use fontes de dados online via URLs e salve a saída em vários formatos."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de plataforma"
  description: "GroupDocs.Assembly for .NET é compatível com os seguintes sistemas operacionais, frameworks e gerenciadores de pacotes."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Assembly for .NET pode processar os seguintes [formatos de arquivo](https://docs.groupdocs.com/assembly/net/supported-document-formats/).
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
  title: "Recursos do GroupDocs.Assembly"
  description: "Crie documentos e relatórios utilizando modelos de dados avançados."

  items:
    # feature loop
    - icon: "preview"
      title: "Representação Avançada de Dados"
      content: "Suporta uma ampla gama de objetos de dados como gráficos, listas, tabelas, imagens e mais."

    # feature loop
    - icon: "manipulate"
      title: "Manipulação de Dados"
      content: "Aplique fórmulas e operações sequenciais para formatar e exibir dados de forma eficaz."

    # feature loop
    - icon: "two_pages"
      title: "Ampla Variedade de Formatos Suportados"
      content: "Trabalhe sem problemas com todos os formatos de documentos comuns para templates ou arquivos de saída."

    # feature loop
    - icon: "document_settings"
      title: "Marcação Enriquecida de Templates"
      content: "Aproveite a formatação ordinal, cardinal e alfabética em templates."

    # feature loop
    - icon: "text"
      title: "Incorporar Códigos de Barra"
      content: "Gere imagens de código de barras dinamicamente e insira-as em seus documentos."

    # feature loop
    - icon: "add"
      title: "Formatação de Dados"
      content: "Formate strings em templates como maiúsculas, minúsculas, com capitalização ou estilos de primeira letra maiúscula."

    # feature loop
    - icon: "manipulate"
      title: "Manipulação do Conteúdo do Documento"
      content: "Insira dinamicamente conteúdo de documentos externos em seus relatórios."

    # feature loop
    - icon: "convert"
      title: "Salvar em Vários Formatos"
      content: "Especifique o formato de arquivo de saída usando extensões de arquivo ou configurações detalhadas."

    # feature loop
    - icon: "update"
      title: "Processamento de Dados Flexível"
      content: "Insira imagens e documentos dinamicamente usando bytes codificados em Base64."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemplos de código"
  description: "Trechos de código para operações típicas do GroupDocs.Assembly."
  items:
    # code sample loop
    - title: "Lista com Marcadores em um Documento Microsoft Word"
      content: |
        [Listas com marcadores](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/) são uma forma comum de apresentar dados comerciais. Aqui está um exemplo de como adicionar uma lista a um documento Word usando GroupDocs.Assembly.
        {{< landing/code title="Como Preencher uma Lista em Documentos">}}
        ```csharp {style=abap}
        // Insira este template em uma página do documento:
        // Indicadores de desempenho dos gerentes
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // Especifique o caminho do template
        string template = "Bulleted List Template.docx";

        // Defina o caminho do arquivo de saída
        string result = "Result Report.docx"

        // Recupere dados dos gerentes de uma fonte JSON
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // Gere o relatório com os dados preenchidos
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Gráficos de Pizza em Presentações PPTX"
      content: |
        Você pode criar [Gráficos de Pizza](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/) usando templates e dados XML. Melhore seus relatórios com representações de dados visualmente atraentes.
        {{< landing/code title="Como Representar Dados em um Gráfico de Pizza">}}
        ```csharp {style=abap}
        // Adicione o template do título do gráfico à apresentação:
        // Receita dos clientes <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Inclua também o template de dados do gráfico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Especifique o caminho do template do gráfico
        string template = "Pie Chart Template.pptx";

        // Defina o caminho do arquivo de saída
        string result = "Result Report.pptx"

        // Recupere os dados dos clientes de uma fonte XML
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // Gere o gráfico e salve o resultado
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---