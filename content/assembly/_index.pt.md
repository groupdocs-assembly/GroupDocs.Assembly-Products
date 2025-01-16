---
############################# Static ############################
layout: "family"
date:  2025-01-16T13:04:05
draft: false

product: "Assembly"
product_tag: "assembly"

lang: pt

############################# Head ############################
head_title: "APIs .NET, Java, Node.js e Aplicativos Online de Montagem de Documentos da GroupDocs"
head_description: "Obtenha uma solução completa para Automação de Documentos e Relatórios para aplicações .NET, Java e Node.js. Gere todos os documentos comuns a partir de templates personalizados e dados."

############################# Header ############################
title: "Solução de Automação e Relatórios de Documentos"
description:  |
  Crie relatórios detalhados utilizando templates e fontes de dados com nossos aplicativos e APIs multiplataforma.

  Gere relatórios em formatos como Word, Excel, Apresentações e muitos mais, utilizando templates com marcação flexível.

  Preencha gráficos, códigos de barra, tabelas e outros elementos com dados de fontes como JSON, XML, CSV, etc.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Escolha sua plataforma"
  title: "Independência de plataforma"
  description: "GroupDocs.Assembly é compatível com os seguintes sistemas operacionais e frameworks:"
  details_link_title: "Saiba mais"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualquer outro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Principais recursos do GroupDocs.Assembly"
  description: "Esta solução ajuda você a criar relatórios em formatos populares de documentos, automaticamente preenchidos com seus dados de negócios. Automatize suas tarefas de geração de documentos."

  items:
    # items loop
    - icon: "additional"
      title: "Preencher templates com dados"
      content: "Preencha relatórios usando dados de fontes suportadas."

    # items loop
    - icon: "manipulate"
      title: "Marcação flexível"
      content: "Adicione dados a documentos de uma forma personalizável."

    # items loop
    - icon: "structure"
      title: "Recursos nativos de documentos"
      content: "Exiba dados usando tabelas, gráficos e códigos de barra."

    # items loop
    - icon: "merge"
      title: "Todos os formatos populares"
      content: "Suporta todos os formatos de documentos comumente usados."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Gere relatórios bem personalizados"
  description: "Exemplos de código do GroupDocs.Assembly"
  items:
    # code sample loop
    - title: "Utilizando Códigos de Barras Gerados"
      content: |
       GroupDocs.Assembly permite a marcação de códigos de barras em templates de relatórios. Ao criar um relatório, um código de barras é gerado com base na marcação e nos dados fornecidos. Especifique o caminho para o template que contém o texto, os objetos de dados e a marcação. Além disso, especifique a fonte de dados para preencher o código de barras com conteúdo.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Crie uma instância da classe DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Especifique o caminho para o template
            var tmp_path = "barcode_template.docx";

            //Especifique o caminho para o documento de resultado
            var res_path = "result.docx";

            //Crie uma instância da fonte de dados
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Chame AssembleDocument para gerar o relatório
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Crie uma instância da classe DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Especifique o caminho para o template
            String tmp_path = "barcode_template.docx";

            //Especifique o caminho para o documento de resultado
            String res_path = "result.docx";

            //Crie uma instância da fonte de dados
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Chame AssembleDocument para gerar o relatório
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // Crie uma instância da classe DocumentAssembler
            const assembler = new assemblyLib.DocumentAssembler();
            
            //Especifique o caminho para o template
            const tmp_path = "barcode_template.docx";

            //Especifique o caminho para o documento de resultado
            const res_path = "result.docx";

            //Crie uma instância da fonte de dados
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // Chame AssembleDocument para gerar o relatório
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Suporta mais de 50 formatos de arquivo"
  description: "GroupDocs.Assembly trabalha com quase todos os formatos de arquivo populares"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Estatísticas do nosso produto"
  description: "Explore métricas do produto para obter insights sobre nosso progresso, impacto e crescimento."

  items:
    # items loop
    - number: "50+"
      title: "Formatos Suportados"
      content: "Suportamos mais de 50 dos formatos de documentos mais amplamente utilizados."

    # items loop
    - number: "650k"
      title: "Downloads do NuGet"
      content: "GroupDocs.Assembly para .NET é uma biblioteca popular com mais de 650.000 downloads no NuGet."

    # items loop
    - number: "18k"
      title: "Downloads do Maven"
      content: "Desenvolvedores Java baixaram GroupDocs.Assembly no Maven mais de 18.000 vezes."

    # items loop
    - number: "150+"
      title: "Clientes Satisfeitos"
      content: "Nossos produtos são confiáveis por desenvolvedores individuais e empresas líderes em todo o mundo para criar soluções inovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nossos Clientes Satisfeitos"
  description: "As bibliotecas GroupDocs são utilizadas por algumas das marcas mais renomadas e respeitadas em todo o mundo."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Pronto para Começar?"
  description: "Teste os recursos do GroupDocs.Assembly gratuitamente em sua plataforma."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Perguntas Frequentes"
  description: "Navegue pelas nossas Perguntas Frequentes."

  items:
    # items loop
    - question: "O GroupDocs.Assembly requer bibliotecas externas para a composição de documentos?"
      answer: "Não, o GroupDocs.Assembly funciona de forma independente e não requer bibliotecas de terceiros como Adobe Acrobat ou Microsoft Office."

    # items loop
    - question: "Posso testar os recursos do GroupDocs.Assembly antes de comprar?"
      answer: "Sim, você pode! O GroupDocs.Assembly oferece um teste gratuito. Instale-o e explore seus recursos. A versão de teste adiciona 'etiquetas de teste' aos seus documentos e processa apenas as primeiras 3 páginas. Para a experiência completa, obtenha uma licença temporária gratuita de 30 dias para acessar todos os recursos. Mais detalhes estão disponíveis em [licença temporária](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quais tipos de licenças estão disponíveis?"
      answer: "Procurando uma licença para o GroupDocs.Assembly? Oferecemos uma variedade de opções para atender às suas necessidades. Escolha com base no tamanho de sua equipe, local de implantação (um único escritório ou remoto), e se você precisa compartilhar o SDK/API com clientes para distribuição. Alternativamente, escolha uma licença de uso mensal com planos medidos — pague apenas pelo que você usa. Encontre a melhor opção para você em [preços](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "APIs de Baixo Código do GroupDocs.Assembly"
  description: "Gere documentos usando sua aplicação através da nossa API REST baseada em nuvem."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Use a API RESTful cURL para adicionar dados a Word, Excel, PowerPoint e muitos outros templates."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Melhore suas aplicações .NET gerando relatórios através do SDK Cloud. Exiba dados de negócios no seu formato personalizado."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "O SDK do GroupDocs.Assembly oferece diferentes opções para aplicações Java gerarem vários tipos de documentos."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Aplicativos Web do GroupDocs.Assembly"
  description: "GroupDocs.Assembly oferece um aplicativo web gratuito para gerar documentos. Você pode processar mais de 50 formatos de arquivo populares diretamente no seu navegador, GRÁTIS."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Gere relatórios em Excel, Word, PowerPoint e muitos outros tipos de arquivos diretamente do seu navegador."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Crie documentos do Microsoft Word a partir de templates e fontes de dados."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Carregue um template e uma fonte de dados para gerar relatórios Excel gratuitamente."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---