---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: pt
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Kit de Ferramentas Node.js para Construir, Automatizar e Personalizar Documentos"
head_description: "Biblioteca Node.js para automatizar fluxos de trabalho de documentos. Gere arquivos PDF, Word, Excel, PowerPoint, HTML e e-mails a partir de seus templates."

############################# Header ############################
title: "API Node.js para Automatização Simplificada de Documentos e Relatórios"
description: "Otimize a geração de relatórios JavaScript combinando seus dados com templates pré-construídos."
words:
  for: "para"

actions:
  main: "Inicie seu Teste no NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "Pronto para Começar?"
  description: "Experimente os recursos do GroupDocs.Assembly gratuitamente ou solicite uma licença."

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Criar um Gráfico em um Documento Word Usando Node.js"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // Caminho para o template principal
    const template = "chart_template.docx";

    // Recuperar dados de produtividade dos gerentes a partir da fonte
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // Crie uma instância de DataSourceInfo com os dados
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // Defina as cores do gráfico utilizando outro DataSourceInfo
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // Preencha o template com dados e salve na saída
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visão Geral do GroupDocs.Assembly"
  description: "Uma biblioteca Node.js desenvolvida para criar documentos programaticamente com manuseio de dados integrado."
  features:
    # feature loop
    - title: "Integre Dados da Empresa nos Templates com JavaScript"
      content: "Gere relatórios sofisticados embutindo JSON, XML ou outros dados em templates com GroupDocs.Assembly for Node.js via Java."

    # feature loop
    - title: "Gerenciar Conteúdo Incorporado"
      content: "Preencha automaticamente tabelas, gráficos e outras visualizações em seus documentos usando dados externos."

    # feature loop
    - title: "Opções Customizáveis"
      content: "GroupDocs.Assembly for Node.js via Java permite adicionar recursos como códigos de barras, buscar dados de URLs e exportar arquivos em vários formatos."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de plataforma"
  description: "GroupDocs.Assembly for Node.js via Java integra-se suavemente com os principais sistemas operacionais, frameworks e gerenciadores de pacotes."
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
    GroupDocs.Assembly for Node.js via Java suporta uma ampla gama de [formatos de documento](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/).
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
  title: "Principais Recursos do GroupDocs.Assembly"
  description: "Crie documentos dinâmicos e relatórios com poderosas ferramentas de gerenciamento de dados."

  items:
    # feature loop
    - icon: "preview"
      title: "Visuais de Dados Ricos"
      content: "Insira gráficos, tabelas, imagens e listas em seus documentos com total personalização."

    # feature loop
    - icon: "manipulate"
      title: "Transforme Seus Dados"
      content: "Aproveite ferramentas como fórmulas e ordenação para estruturar e exibir informações de forma eficaz."

    # feature loop
    - icon: "two_pages"
      title: "Ampla Compatibilidade de Formatos"
      content: "Trabalhe de forma fluida com formatos de arquivo populares para templates e saídas."

    # feature loop
    - icon: "document_settings"
      title: "Customização Avançada de Templates"
      content: "Formate templates com opções de estilo numérico, alfabético e outras."

    # feature loop
    - icon: "text"
      title: "Gere Códigos de Barras Dinamicamente"
      content: "Crie e insira imagens de código de barras diretamente em seus documentos sob demanda."

    # feature loop
    - icon: "add"
      title: "Estilo de Texto Flexível"
      content: "Aplique facilmente estilos de texto como capitalização ou título em seus templates."

    # feature loop
    - icon: "manipulate"
      title: "Inserção Dinâmica de Conteúdo"
      content: "Inclua conteúdo de arquivos externos de forma dinâmica durante a geração de documentos."

    # feature loop
    - icon: "convert"
      title: "Exporte para Vários Formatos"
      content: "Salve documentos em múltiplos formatos com suas configurações especificadas."

    # feature loop
    - icon: "update"
      title: "Incorpore Mídia Dinamicamente"
      content: "Insira imagens ou outros elementos usando dados Base64 ao criar documentos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemplos de código"
  description: "Descubra exemplos práticos de como utilizar GroupDocs.Assembly para tarefas comuns."
  items:
    # code sample loop
    - title: "Adicionar uma Lista com Marcadores em Documentos Word"
      content: |
        Veja como criar [listas com marcadores](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/) em documentos Word para organizar dados de forma eficaz. Este exemplo demonstra como gerar uma lista com marcadores usando GroupDocs.Assembly.
        {{< landing/code title="Adicionar uma Lista com Marcadores em Documentos Word">}}
        ```javascript {style=abap}
        // Insira este template em uma página do documento:
        // Indicadores de desempenho dos gerentes
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifique o caminho do template
        const template = "Bulleted List Template.docx";

        // Defina o caminho do arquivo de saída
        const result = "Result Report.docx"

        // Recupere dados dos gerentes de uma fonte JSON
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // Gere o relatório com os dados preenchidos
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Inserir Gráficos de Pizza em PowerPoint"
      content: |
        Aprenda como usar templates e XML para adicionar [gráficos de pizza](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/) em suas apresentações. Melhore seus relatórios com gráficos de pizza para apresentar dados de forma visual e clara.
        {{< landing/code title="Inserir Gráficos de Pizza em PowerPoint">}}
        ```javascript {style=abap} 
        // Adicione o template do título do gráfico à apresentação:
        // Receita dos clientes <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // Inclua também o template de dados do gráfico:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // Especifique o caminho do template do gráfico
        const template = "Pie Chart Template.pptx";

        // Defina o caminho do arquivo de saída
        const result = "Result Report.pptx"

        // Recupere os dados dos clientes de uma fonte XML
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // Gere o gráfico e salve o resultado
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---