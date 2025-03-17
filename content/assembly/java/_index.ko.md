---
############################# Static ############################
layout: "landing"
date: 2025-03-17T13:11:11
draft: false

lang: ko
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
head_title: "문서 생성, 자동화 및 보고를 위한 Java 라이브러리"
head_description: "문서 생성을 자동화하고 보고서를 생성하기 위한 Java 라이브러리. 사용자 정의 템플릿을 사용하여 PDF, Word, Excel, PPTX, HTML 및 이메일 문서를 생성합니다."

############################# Header ############################
title: "보고서 및 문서 자동화를 위한 Java API"
description: "데이터와 템플릿을 병합하여 Java에서 보고서 생성을 간소화합니다."
words:
  for: "용"

actions:
  main: "Maven에서 무료 체험 받기"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-assembly/"
  alt: "라이선스 관리"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/java/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Assembly의 기능을 무료로 사용해 보거나 라이선스를 요청하세요."

release:
  title: "버전 {0} 출시"
  notes: "새로운 사항 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/assembly/java/"

code:
  title: "Java로 DOCX에서 차트 생성하기"
  more: "더 많은 예시"
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
    // 주 템플릿의 경로
    String template = "chart_template.docx";

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
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly 개요"
  description: "문서 생성을 자동화하고 원활한 데이터 통합을 위해 설계된 Java 라이브러리입니다."
  features:
    # feature loop
    - title: "Java로 템플릿에 비즈니스 데이터 병합하기"
      content: "GroupDocs.Assembly for Java를 사용하여 JSON, XML 또는 기타 소스의 데이터를 디자인된 템플릿에 쉽게 삽입하여 전문 보고서를 생성합니다."

    # feature loop
    - title: "포함된 객체 작업하기"
      content: "외부 소스의 데이터를 사용하여 문서의 테이블, 차트 및 다이어그램과 같은 요소를 자동으로 채웁니다."

    # feature loop
    - title: "고급 사용자 정의"
      content: "GroupDocs.Assembly for Java는 바코드 생성, URL을 통해 온라인 데이터 가져오기, 여러 형식으로 출력 내보내기와 같은 유연한 기능을 제공합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Assembly for Java는 인기 있는 운영 체제, 개발 프레임워크 및 패키지 관리자와 원활하게 작동합니다."
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
  title: "지원하는 파일 형식"
  description: |
    GroupDocs.Assembly for Java는 다양한 [문서 형식](https://docs.groupdocs.com/assembly/java/supported-document-formats/)을 지원합니다.
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
  title: "GroupDocs.Assembly의 주요 기능"
  description: "고급 데이터 핸들링으로 전문 문서 및 보고서를 생성합니다."

  items:
    # feature loop
    - icon: "preview"
      title: "시각적 데이터 요소"
      content: "문서에 차트, 테이블, 이미지 및 목록과 같은 요소를 추가하고 형식화합니다."

    # feature loop
    - icon: "manipulate"
      title: "데이터 변환"
      content: "효과적으로 데이터를 정리하고 표시하기 위해 수식, 정렬 및 기타 도구를 사용합니다."

    # feature loop
    - icon: "two_pages"
      title: "다양한 형식 지원"
      content: "템플릿과 출력 파일 모두 일반 파일 형식으로 쉽게 작업할 수 있습니다."

    # feature loop
    - icon: "document_settings"
      title: "향상된 템플릿 형식화"
      content: "서수, 기수 및 기타 고급 형식 옵션으로 템플릿을 사용자 정의합니다."

    # feature loop
    - icon: "text"
      title: "동적 바코드 생성"
      content: "필요에 따라 신속하게 바코드 이미지를 생성하고 문서에 삽입합니다."

    # feature loop
    - icon: "add"
      title: "유연한 텍스트 스타일링"
      content: "템플릿에서 대문자, 소문자, 제목 대문자 또는 기타 스타일을 적용합니다."

    # feature loop
    - icon: "manipulate"
      title: "외부 콘텐츠 가져오기"
      content: "문서를 생성하는 동안 외부 파일의 콘텐츠를 동적으로 삽입합니다."

    # feature loop
    - icon: "convert"
      title: "여러 형식으로 내보내기"
      content: "지정한 확장자 또는 구성을 사용하여 최종 문서를 다양한 파일 형식으로 저장합니다."

    # feature loop
    - icon: "update"
      title: "동적 미디어 삽입"
      content: "문서 생성 중에 Base64 인코딩된 데이터를 사용하여 이미지 또는 기타 콘텐츠를 삽입합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "GroupDocs.Assembly의 일반적인 작업을 위한 샘플 코드 탐색."
  items:
    # code sample loop
    - title: "Word에서 글머리 목록 만들기"
      content: |
        Word 문서에 조직적인 데이터 표현을 위해 [글머리 목록](https://docs.groupdocs.com/assembly/java/bulleted-list-in-word-processing-document/)을 추가하는 방법을 배웁니다. 이 예는 GroupDocs.Assembly를 사용하여 Word에 목록을 생성하는 방법을 보여줍니다.
        {{< landing/code title="Word에서 글머리 목록 만들기">}}
        ```java {style=abap}
        // 문서 페이지에 이 템플릿을 삽입하세요:
        // 관리자의 성과 지표
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        // 템플릿 경로 지정
        String template = "Bulleted List Template.docx";

        // 출력 파일 경로 설정
        String result = "Result Report.docx"

        // JSON 소스에서 관리자 데이터를 가져옵니다
        JsonDataSource dataSource = new JsonDataSource("Report data.json");
        DataSourceInfo data = new DataSourceInfo(dataSource, "managers")

        // 채워진 데이터로 보고서를 생성합니다
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "PPTX에서 원형 차트 생성하기"
      content: |
        템플릿과 XML을 사용하여 프레젠테이션에 [원형 차트](https://docs.groupdocs.com/assembly/java/pie-chart-in-presentation-document/)를 추가합니다. 데이터를 시각화하여 보고서를 더욱 매력적으로 만듭니다.
        {{< landing/code title="PPTX에서 원형 차트 생성하기">}}
        ```java {style=abap}   
        // 프레젠테이션에 차트 제목 템플릿 추가:
        // 고객 수익 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 차트 데이터 템플릿도 포함하세요:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 차트 템플릿 경로 지정
        String template = "Pie Chart Template.pptx";

        // 출력 파일 경로 설정
        String result = "Result Report.pptx"

        // XML 소스에서 고객 데이터를 가져옵니다
        JsonDataSource dataSource = new JsonDataSource("Chart data.xml");
        DataSourceInfo data = new DataSourceInfo(dataSource, "customers")

        // 차트를 생성하고 결과를 저장합니다
        DocumentAssembler assembler = new DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---