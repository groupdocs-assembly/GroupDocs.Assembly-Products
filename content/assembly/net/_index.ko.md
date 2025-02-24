---
############################# Static ############################
layout: "landing"
date: 2025-02-24T17:52:13
draft: false

lang: ko
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
head_title: ".NET 문서 자동화, 조립 및 보고 생성 API"
head_description: "문서 자동화, 조립 및 보고 생성을 위한 C# .NET API. 사용자 정의 템플릿에서 PDF, Word, Excel, PPTX, HTML 및 이메일 문서를 생성합니다."

############################# Header ############################
title: ".NET 문서 자동화 및 보고 API"
description: ".NET 애플리케이션에서 템플릿을 정의하고 데이터를 병합하여 보고서를 생성합니다."
words:
  for: "용"

actions:
  main: "Nuget에서 무료 체험 다운로드"
  main_link: "https://www.nuget.org/packages/GroupDocs.Assembly"
  alt: "라이선스 관리"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/net/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Assembly의 기능을 무료로 사용해 보거나 라이선스를 요청하세요."

release:
  title: "버전 {0} 출시"
  notes: "새로운 사항 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/assembly/net/"

code:
  title: "C#를 사용한 DOCX의 차트 채우기"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
  install: "dotnet add package GroupDocs.Assembly"
  content: |
    ```csharp {style=abap}   
    // 주 템플릿의 경로
    string template = "chart_template.docx";

    // 소스에서 관리자 생산성 데이터 검색
    DocumentTable data_table = 
        new DocumentTable("Managers.json", 1);

    // DataSourceInfo의 인스턴스를 데이터로 생성
    DataSourceInfo data 
        = new DataSourceInfo(data_table, "managers");

    // 다른 DataSourceInfo를 사용하여 차트 색상 설정
    DataSourceInfo design = 
        new DataSourceInfo("red", "color");

    // 데이터로 템플릿 채우고 출력으로 저장
    DocumentAssembler asm = new DocumentAssembler();
    asm.AssembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly 개요"
  description: ".NET 솔루션으로 고급 데이터 통합과 함께 문서 생성을 자동화합니다."
  features:
    # feature loop
    - title: "C#로 문서 템플릿에 비즈니스 데이터 추가"
      content: "보고서 생성: GroupDocs.Assembly for .NET를 사용하여 JSON 또는 XML과 같은 소스에서 데이터를 쉽게 삽입할 수 있습니다."

    # feature loop
    - title: "네이티브 데이터 객체 처리"
      content: "지원되는 문서 유형에는 데이터로 자동 채울 수 있는 다이어그램, 차트, 테이블 및 목록과 같은 포함된 객체가 포함됩니다."

    # feature loop
    - title: "추가 기능"
      content: "GroupDocs.Assembly for .NET는 광범위한 사용자 정의 옵션을 제공합니다. 데이터 객체를 프로그래밍 방식으로 디자인하고, 바코드를 생성하며, URL을 통해 온라인 데이터 소스를 사용하고, 다양한 형식으로 출력을 저장합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Assembly for .NET는 다음 운영 체제, 프레임워크 및 패키지 관리자와 호환됩니다."
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
  title: "지원하는 파일 형식"
  description: |
    GroupDocs.Assembly for .NET는 다음 [파일 형식](https://docs.groupdocs.com/assembly/net/supported-document-formats/)을 처리할 수 있습니다.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 형식
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF, WordprocessingML
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTM, POTX
    # group loop
    - color: "blue"
      content: |
        ### 이미지 및 기타 형식
        * **휴대용:** PDF
        * **이미지:** SVG, TIFF
        * **기타 오피스 형식:** ODT, OTT, OTS, ODS, ODP, OTP
      # group loop
    - color: "red"
      content: |
        ### 기타 형식
        * **웹:** HTML, MHTML
        * **이메일:** EML, MSG, EMLX
        * **기타:** EPUB, MD

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Assembly 기능"
  description: "고급 데이터 모델을 사용하여 문서 및 보고서를 생성합니다."

  items:
    # feature loop
    - icon: "preview"
      title: "고급 데이터 표현"
      content: "차트, 목록, 테이블, 이미지 등 다양한 데이터 객체를 지원합니다."

    # feature loop
    - icon: "manipulate"
      title: "데이터 조작"
      content: "데이터를 효과적으로 형식화하고 표시하기 위해 수식 및 순차 작업을 적용합니다."

    # feature loop
    - icon: "two_pages"
      title: "지원되는 형식의 폭넓은 범위"
      content: "템플릿 또는 출력 파일을 위해 모든 일반 문서 형식과 원활하게 작업합니다."

    # feature loop
    - icon: "document_settings"
      title: "풍부한 템플릿 마크업"
      content: "템플릿에 서수, 기수 및 알파벳 숫자 형식을 활용합니다."

    # feature loop
    - icon: "text"
      title: "바코드 삽입"
      content: "바코드 이미지를 동적으로 생성하고 문서에 삽입합니다."

    # feature loop
    - icon: "add"
      title: "데이터 형식 지정"
      content: "템플릿에서 대문자, 소문자, 대문자 첫 글자 등의 스타일로 문자열을 형식화합니다."

    # feature loop
    - icon: "manipulate"
      title: "문서 콘텐츠 조작"
      content: "외부 문서에서 콘텐츠를 동적으로 삽입하여 보고서를 생성합니다."

    # feature loop
    - icon: "convert"
      title: "여러 형식으로 저장"
      content: "파일 확장자나 자세한 구성 설정을 사용하여 출력 파일 형식을 지정합니다."

    # feature loop
    - icon: "update"
      title: "유연한 데이터 처리"
      content: "Base64 인코딩된 바이트를 사용하여 동적으로 이미지 및 문서를 삽입합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "일반적인 GroupDocs.Assembly 작업을 위한 코드 스니펫."
  items:
    # code sample loop
    - title: "Microsoft Word 문서의 글머리 목록"
      content: |
        [글머리 목록](https://docs.groupdocs.com/assembly/net/bulleted-list-in-word-processing-document/)은 비즈니스 데이터를 제공하는 일반적인 방법입니다. 다음은 GroupDocs.Assembly를 사용하여 Word 문서에 목록을 추가하는 예입니다.
        {{< landing/code title="문서에 목록 채우기">}}
        ```csharp {style=abap}
        // 문서 페이지에 이 템플릿을 삽입하세요:
        // 관리자의 성과 지표
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // 템플릿 경로 지정
        string template = "Bulleted List Template.docx";

        // 출력 파일 경로 설정
        string result = "Result Report.docx"

        // JSON 소스에서 관리자 데이터를 가져옵니다
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // 채워진 데이터로 보고서를 생성합니다
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "PPTX 프리젠테이션의 원형 차트"
      content: |
        템플릿과 XML 데이터를 사용하여 [원형 차트](https://docs.groupdocs.com/assembly/net/pie-chart-in-presentation-document/)를 생성할 수 있습니다. 시각적으로 매력적인 데이터 표현으로 보고서를 더욱 향상시킵니다.
        {{< landing/code title="원형 차트로 데이터 표현하기">}}
        ```csharp {style=abap}
        // 프레젠테이션에 차트 제목 템플릿 추가:
        // 고객 수익 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 차트 데이터 템플릿도 포함하세요:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 차트 템플릿 경로 지정
        string template = "Pie Chart Template.pptx";

        // 출력 파일 경로 설정
        string result = "Result Report.pptx"

        // XML 소스에서 고객 데이터를 가져옵니다
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // 차트를 생성하고 결과를 저장합니다
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.AssembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---