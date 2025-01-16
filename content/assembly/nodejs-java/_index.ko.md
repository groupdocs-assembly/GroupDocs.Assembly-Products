---
############################# Static ############################
layout: "landing"
date: 2025-01-16T13:04:06
draft: false

lang: ko
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
head_title: "Node.js 문서 생성, 자동화 및 사용자 정의를 위한 툴킷"
head_description: "Node.js 문서 워크플로우 자동화를 위한 라이브러리입니다. 템플릿에서 PDF, Word, Excel, PowerPoint, HTML 및 이메일 파일을 생성합니다."

############################# Header ############################
title: "Node.js API를 통한 문서 및 보고서 자동화 간소화"
description: "사전 구축된 템플릿과 데이터를 병합하여 JavaScript 보고서 생성을 간소화합니다."
words:
  for: "용"

actions:
  main: "NPM에서 무료 평가판 시작"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.assembly"
  alt: "라이선스 관리"
  alt_link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Assembly의 기능을 무료로 사용해 보거나 라이선스를 요청하세요."

release:
  title: "버전 {0} 출시"
  notes: "새로운 사항 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/assembly/nodejs-java/"

code:
  title: "Node.js를 사용하여 Word 문서에 차트 만들기"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.assembly"
  content: |
    ```javascript {style=abap}
    const assemblyLib = require('@groupdocs/groupdocs.assembly');

    // 주 템플릿의 경로
    const template = "chart_template.docx";

    // 소스에서 관리자 생산성 데이터 검색
    const data_table = 
        new assemblyLib.DocumentTable("Managers.json", 1);

    // DataSourceInfo의 인스턴스를 데이터로 생성
    const data 
        = new assemblyLib.DataSourceInfo(data_table, "managers");

    // 다른 DataSourceInfo를 사용하여 차트 색상 설정
    const design = 
        new assemblyLib.DataSourceInfo("red", "color");

    // 데이터로 템플릿 채우고 출력으로 저장
    const asm = new assemblyLib.DocumentAssembler();
    asm.assembleDocument(template, "result.docx", data, design);
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Assembly 개요"
  description: "데이터 처리가 통합된 프로그래밍 방식으로 문서를 생성하기 위해 구축된 Node.js 라이브러리입니다."
  features:
    # feature loop
    - title: "JavaScript로 템플릿에 비즈니스 데이터 통합"
      content: "GroupDocs.Assembly for Node.js via Java을 사용하여 JSON, XML 또는 기타 데이터를 템플릿에 삽입하여 세련된 보고서를 생성합니다."

    # feature loop
    - title: "임베디드 콘텐츠 관리"
      content: "외부 데이터를 사용하여 문서 내의 표, 차트 및 기타 시각적 요소를 자동으로 채웁니다."

    # feature loop
    - title: "사용자 정의 가능한 옵션"
      content: "GroupDocs.Assembly for Node.js via Java을 사용하면 바코드 추가, URL에서 데이터 가져오기, 다양한 형식으로 파일 내보내기와 같은 기능을 추가할 수 있습니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Assembly for Node.js via Java은 선도적인 운영 체제, 프레임워크 및 패키지 관리자와 원활하게 통합됩니다."
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
    GroupDocs.Assembly for Node.js via Java은 광범위한 [문서 형식](https://docs.groupdocs.com/assembly/nodejs-java/supported-document-formats/)을 지원합니다.
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
  title: "GroupDocs.Assembly의 핵심 기능"
  description: "강력한 데이터 관리 도구를 사용하여 동적 문서 및 보고서를 생성합니다."

  items:
    # feature loop
    - icon: "preview"
      title: "풍부한 데이터 시각화"
      content: "문서에 차트, 표, 이미지 및 목록을 완전히 사용자 정의하여 쉽게 삽입할 수 있습니다."

    # feature loop
    - icon: "manipulate"
      title: "데이터 변환"
      content: "공식 및 정렬과 같은 도구를 활용하여 정보를 효과적으로 구조화하고 표시합니다."

    # feature loop
    - icon: "two_pages"
      title: "광범위한 형식 호환성"
      content: "템플릿과 출력에 일반적으로 사용되는 파일 형식과 원활하게 작업합니다."

    # feature loop
    - icon: "document_settings"
      title: "고급 템플릿 사용자 정의"
      content: "숫자, 알파벳 및 기타 스타일링 옵션으로 템플릿을 포맷합니다."

    # feature loop
    - icon: "text"
      title: "동적으로 바코드 생성"
      content: "필요에 따라 문서에 바코드 이미지를 직접 생성하고 삽입합니다."

    # feature loop
    - icon: "add"
      title: "유연한 텍스트 스타일링"
      content: "템플릿에서 대문자화 또는 제목 형식과 같은 텍스트 스타일을 쉽게 적용합니다."

    # feature loop
    - icon: "manipulate"
      title: "동적 콘텐츠 삽입"
      content: "문서 생성 중 외부 파일의 콘텐츠를 동적으로 포함합니다."

    # feature loop
    - icon: "convert"
      title: "다양한 형식으로 내보내기"
      content: "지정한 구성으로 여러 형식으로 문서를 저장합니다."

    # feature loop
    - icon: "update"
      title: "동적으로 미디어 삽입"
      content: "문서를 생성할 때 Base64 데이터를 사용하여 이미지나 기타 요소를 삽입합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "GroupDocs.Assembly을 사용하여 일반 작업을 수행하는 방법에 대한 실용적인 예제를 발견하십시오."
  items:
    # code sample loop
    - title: "Word 문서에 글머리 목록 추가"
      content: |
        데이터를 효과적으로 정리하기 위해 Word 문서에서 [글머리 목록](https://docs.groupdocs.com/assembly/nodejs-java/bulleted-list-in-word-processing-document/)을 생성하는 방법을 확인하십시오. 이 예제는 GroupDocs.Assembly을 사용하여 글머리 목록을 생성하는 방법을 보여줍니다.
        {{< landing/code title="Word 문서에 글머리 목록 추가">}}
        ```javascript {style=abap}
        // 문서 페이지에 이 템플릿을 삽입하세요:
        // 관리자의 성과 지표
        // . <<foreach [in products]>><<[ProductName]>>
        // <</foreach>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 템플릿 경로 지정
        const template = "Bulleted List Template.docx";

        // 출력 파일 경로 설정
        const result = "Result Report.docx"

        // JSON 소스에서 관리자 데이터를 가져옵니다
        const dataSource = new assemblyLib.JsonDataSource("Report data.json");
        const data = new assemblyLib.DataSourceInfo(dataSource, "managers")

        // 채워진 데이터로 보고서를 생성합니다
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "PowerPoint에 원형 차트 삽입"
      content: |
        템플릿과 XML을 사용하여 프레젠테이션에 [원형 차트](https://docs.groupdocs.com/assembly/nodejs-java/pie-chart-in-presentation-document/)를 추가하는 방법을 배우십시오. 데이터를 시각적으로 명확하게 제시하기 위해 원형 차트를 사용하여 보고서를 향상시킵니다.
        {{< landing/code title="PowerPoint에 원형 차트 삽입">}}
        ```javascript {style=abap} 
        // 프레젠테이션에 차트 제목 템플릿 추가:
        // 고객 수익 <<foreach [in customers]>> 
        // <<x [CustomerName]>>

        // 차트 데이터 템플릿도 포함하세요:
        // Total Order Price<<foreach [in customers]>> 
        // <<x [CustomerName]>>

        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 차트 템플릿 경로 지정
        const template = "Pie Chart Template.pptx";

        // 출력 파일 경로 설정
        const result = "Result Report.pptx"

        // XML 소스에서 고객 데이터를 가져옵니다
        const dataSource = new assemblyLib.JsonDataSource("Chart data.xml");
        const data = new assemblyLib.DataSourceInfo(dataSource, "customers")

        // 차트를 생성하고 결과를 저장합니다
        const assembler = new assemblyLib.DocumentAssembler();
        assembler.assembleDocument(template, result, data);
        ```
        {{< /landing/code >}}

---