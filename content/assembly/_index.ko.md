---
############################# Static ############################
layout: "family"
date:  2025-01-16T13:04:05
draft: false

product: "Assembly"
product_tag: "assembly"

lang: ko

############################# Head ############################
head_title: "GroupDocs의 .NET, Java, Node.js API 및 온라인 문서 조립 애플리케이션"
head_description: ".NET, Java 및 Node.js 애플리케이션을 위한 올인원 문서 자동화 및 보고 솔루션을 받아보세요. 사용자 정의 템플릿과 데이터를 통해 모든 일반 문서를 생성합니다."

############################# Header ############################
title: "문서 자동화 및 보고 솔루션"
description:  |
  크로스 플랫폼 애플리케이션 및 API를 사용하여 템플릿 및 데이터 소스를 활용하여 상세한 보고서를 만듭니다.

  {{FileFormatUp}}와 같은 형식으로 Word, Excel, 프레젠테이션 및 기타 많은 문서를 생성합니다. 유연한 마크업이 있는 템플릿을 사용합니다.

  JSON, XML, CSV 등의 데이터 소스에서 데이터를 사용하여 차트, 바코드, 테이블 및 기타 요소를 채웁니다.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "플랫폼 선택"
  title: "플랫폼 독립성"
  description: "GroupDocs.Assembly는 다음 운영 체제 및 프레임워크와 호환됩니다:"
  details_link_title: "더 알아보기"

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
                    Atom <br> Visual Studio Code <br> 기타 텍스트 편집기
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Assembly 주요 기능"
  description: "이 솔루션은 인기 있는 문서 형식으로 비즈니스 데이터로 자동 채워진 보고서를 생성하는 데 도움이 됩니다. 문서 생성 작업을 자동화합니다."

  items:
    # items loop
    - icon: "additional"
      title: "데이터로 템플릿 채우기"
      content: "지원되는 소스의 데이터를 사용하여 보고서를 채웁니다."

    # items loop
    - icon: "manipulate"
      title: "유연한 마크업"
      content: "사용자 정의 방식으로 문서에 데이터를 추가합니다."

    # items loop
    - icon: "structure"
      title: "네이티브 문서 기능"
      content: "테이블, 차트 및 바코드를 사용하여 데이터를 표시합니다."

    # items loop
    - icon: "merge"
      title: "모든 유명한 형식"
      content: "모든 일반적으로 사용되는 문서 형식을 지원합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "잘 맞춤화된 보고서 생성"
  description: "GroupDocs.Assembly 코드 예제"
  items:
    # code sample loop
    - title: "생성된 바코드 사용하기"
      content: |
       GroupDocs.Assembly는 보고서 템플릿에 바코드 마크업을 허용합니다. 보고서를 생성할 때 마크업 및 제공된 데이터를 기반으로 바코드가 생성됩니다. 텍스트, 데이터 객체 및 마크업이 포함된 템플릿의 경로를 지정합니다. 또한 바코드에 내용을 채우기 위해 데이터 소스를 지정합니다.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // DocumentAssembler 클래스의 인스턴스 생성
            DocumentAssembler assembler = new DocumentAssembler();

            //템플릿 경로 지정
            var tmp_path = "barcode_template.docx";

            //결과 문서 경로 지정
            var res_path = "result.docx";

            //데이터 소스의 인스턴스 생성
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //AssembleDocument를 호출하여 보고서 생성
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // DocumentAssembler 클래스의 인스턴스 생성
            DocumentAssembler assembler = new DocumentAssembler();
            
            //템플릿 경로 지정
            String tmp_path = "barcode_template.docx";

            //결과 문서 경로 지정
            String res_path = "result.docx";

            //데이터 소스의 인스턴스 생성
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // AssembleDocument를 호출하여 보고서 생성
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // DocumentAssembler 클래스의 인스턴스 생성
            const assembler = new assemblyLib.DocumentAssembler();
            
            //템플릿 경로 지정
            const tmp_path = "barcode_template.docx";

            //결과 문서 경로 지정
            const res_path = "result.docx";

            //데이터 소스의 인스턴스 생성
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // AssembleDocument를 호출하여 보고서 생성
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "50개 이상의 파일 형식 지원"
  description: "GroupDocs.Assembly는 거의 모든 인기 있는 파일 형식으로 작업합니다."

############################# Metrics ###############################
metrics:
  enable: true
  title: "우리 제품 통계"
  description: "진행 상황, 영향 및 성장에 대한 통찰력을 얻기 위해 제품 메트릭을 탐색합니다."

  items:
    # items loop
    - number: "50+"
      title: "지원되는 형식"
      content: "우리는 50개 이상의 가장 널리 사용되는 문서 형식을 지원합니다."

    # items loop
    - number: "650k"
      title: "NuGet 다운로드"
      content: "GroupDocs.Assembly for .NET은 NuGet에서 650,000회 이상의 다운로드를 기록한 인기 있는 라이브러리입니다."

    # items loop
    - number: "18k"
      title: "Maven 다운로드"
      content: "Java 개발자들은 Maven에서 GroupDocs.Assembly를 18,000회 이상 다운로드했습니다."

    # items loop
    - number: "150+"
      title: "만족한 고객"
      content: "우리 제품은 개별 개발자 및 세계 유수의 기업들이 혁신적인 솔루션을 만들기 위해 신뢰하고 있습니다."


############################# Customers ###############################
customers:
  enable: true
  title: "우리의 행복한 고객"
  description: "GroupDocs 라이브러리는 전 세계에서 가장 유명하고 존경받는 브랜드들에 의해 사용되고 있습니다."

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
  title: "시작할 준비가 되셨나요?"
  description: "당신의 플랫폼에서 GroupDocs.Assembly의 기능을 무료로 시험해 보세요."

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
  title: "자주 묻는 질문"
  description: "자주 묻는 질문을 살펴보세요."

  items:
    # items loop
    - question: "GroupDocs.Assembly는 문서 생성에 외부 라이브러리를 필요로 하나요?"
      answer: "아니요, GroupDocs.Assembly는 독립적으로 작동하며 Adobe Acrobat이나 Microsoft Office와 같은 타사 라이브러리를 필요로 하지 않습니다."

    # items loop
    - question: "GroupDocs.Assembly 기능을 구매 전에 시험해 볼 수 있나요?"
      answer: "네, 가능합니다! GroupDocs.Assembly는 무료 체험을 제공합니다. 설치하고 기능을 탐색해보세요. 체험 버전은 문서에 '체험 배지'를 추가하고 처음 3페이지만 처리합니다. 완전한 경험을 위해 모든 기능에 접근할 수 있는 무료 30일 임시 라이선스를 얻으세요. 더 자세한 내용은 [임시 라이선스](https://purchase.groupdocs.com/temporary-license/)에서 확인할 수 있습니다."

    # items loop
    - question: "어떤 종류의 라이선스가 있나요?"
      answer: "GroupDocs.Assembly 라이선스를 찾고 계신가요? 필요에 맞추어 다양한 옵션을 제공합니다. 팀 규모, 배포 위치(단일 사무실 또는 원격) 및 고객과의 SDK/API 공유 여부에 따라 선택하세요. 또는 사용량에 따라 요금을 지불하는 월별 사용 라이선스를 선택할 수 있습니다. [가격 책정](https://purchase.groupdocs.com/pricing/assembly/net/)에서 최적의 옵션을 찾아보세요."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Assembly 저코드 API"
  description: "클라우드 기반 REST API를 통해 애플리케이션에서 문서를 생성합니다."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "cURL RESTful API를 사용하여 Word, Excel, PowerPoint 및 기타 많은 템플릿에 데이터를 추가합니다."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: ".NET 애플리케이션을 강화하여 Cloud SDK를 통해 보고서를 생성합니다. 비즈니스 데이터를 사용자 정의 형식으로 표시합니다."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK는 Java 애플리케이션이 다양한 유형의 문서를 생성할 수 있도록 다양한 옵션을 제공합니다."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Assembly 웹 앱"
  description: "GroupDocs.Assembly는 문서를 생성하기 위한 무료 웹 애플리케이션을 제공합니다. 브라우저에서 50개 이상의 인기 파일 형식을 무료로 처리할 수 있습니다."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "브라우저에서 직접 Excel, Word, PowerPoint 및 기타 여러 파일 유형의 보고서를 생성합니다."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "템플릿 및 데이터 소스를 사용하여 Microsoft Word 문서를 생성합니다."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "템플릿과 데이터 소스를 업로드하여 무료로 Excel 보고서를 생성합니다."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---