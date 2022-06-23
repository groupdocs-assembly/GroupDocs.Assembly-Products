---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

head_title: "Java 문서 자동화 어셈블리 및 동적 보고서 생성기 API"
head_description: "문서 자동화, 어셈블리 및 보고를 위한 Java API. 사용자 지정 템플릿에서 보고서를 만듭니다. DB, JSON, OData 및 XML 데이터 소스에서 PDF Word Excel PPTX HTML 조합."

title: "문서 및 보고서를 자동화하는 Java API"
description: "데이터를 가져오기 위한 문서 자동화 애플리케이션 구축 사용자 정의 가능한 템플릿에 넣고 Java API를 통해 동적 보고서 생성."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
        product: "GroupDocs.Assembly"
        platform: "Java"

    middle:
        button:
            - link: "#overview"
              text: "개요"

            - link: "#features"
              text: "특징"

            - link: "#support"
              text: "지원하다"

            - link: "https://products.groupdocs.app/assembly"
              text: "라이브 데모"

            - link: "https://purchase.groupdocs.com/pricing/assembly/java"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      Java API용 GroupDocs.Assembly를 사용하면 외부 소프트웨어를 설치하지 않고도 템플릿에서 사용자 정의 보고서를 생성할 수 있도록 Java로 문서 자동화 및 보고 응용 프로그램을 신속하게 개발할 수 있습니다. 보고서 생성 엔진은 템플릿 문서에서 데이터를 가져와서 조합하고 정의된 구문에 따라 지정된 출력 형식으로 보고서를 생성합니다. 템플릿 요소의 서식 속성을 동적으로 구성 및 삽입할 수 있으며 데이터를 검색할 다양한 데이터 소스(JSON, XML, OData, 데이터베이스, CSV, 데이터 테이블로 스프레드시트, 데이터 및 데이터베이스 테이블로 워드 프로세싱 테이블)를 지원합니다.  

      문서 어셈블리 라이브러리는 여러 문서 형식을 인식하고 PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션 및 텍스트와 같이 지원되는 모든 파일 형식으로 템플릿을 만들 수 있습니다. LINQ 기반 템플릿 구문을 지원하며 사용자는 템플릿 요소의 서식 속성을 동적으로 구성하고 삽입할 수도 있습니다.  

      Java용 GroupDocs.Assembly는 신규 또는 기존 Java 애플리케이션과 쉽게 통합됩니다. 모든 Java 버전과 매우 호환되며 Java 런타임을 실행할 수 있는 널리 사용되는 운영 체제(Windows, Linux, MacOS)를 지원합니다.
    tabs:
      enable: true     
      
      tab_one:
        description: |
          다음은 Java용 GroupDocs.Assembly의 개요입니다.

        right:
          enable: true
          icon: "fab fa-html5"
          title: "개요"
          content: |
            * 데이터 공식화
            * 데이터 포맷
            * 데이터 자동화
            * 템플릿 만들기
            * 템플릿 요소 서식
            * 보고서 생성
      
      tab_two:
        description: |
          Java 문서 생성 API에 지원되는 [문서 파일 형식](https://docs.groupdocs.com/assembly/java/supported-document-formats/)은 다음과 같습니다.

        left:
          enable: true
          table:
            - title: "마이크로소프트 오피스 형식"
              content: |
                * **워드**: DOC, DOCX, DOT, DOTX, DOTM, DOCM, RTF, WordprocessingML(XML)
                * **엑셀**: XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX, SpreadsheetML(XML)
                * **파워포인트**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM
                * **전망**: EML, EMLX, MSG, MHT

            - title: "지원되는 데이터 소스"
              content: |
                * 데이터베이스
                * XML
                * 오데이터
                * JSON
                * CSV
                * 사용자 정의 .NET 개체
                * 데이터 테이블로서의 스프레드시트
                * 데이터 테이블로서의 워드 프로세싱 테이블

        right:
          enable: true
          table:
            - title: "기타 형식"
              content: |
                * **오픈오피스 문서 형식**: ODT, OTT, ODS, ODP
                * **이메일**: MHT, MHTML
                * **웹**: HTML
                * **마크다운 문서 파일**: MD
                * **기타**: TXT

            - title: "형식 간 어셈블리 지원"
              content: |
                * 워드 프로세싱 **TO** 워드 프로세싱, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * 스프레드시트 **TO** 스프레드시트, HTML, PDF, XPS, TIFF, MHTML
                * 프레젠테이션 **TO** 프레젠테이션, HTML, PDF, XPS, TIFF
                * 이메일 **TO** 워드 프로세싱, 이메일, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL
                * HTML 및 TXT **TO** 워드 프로세싱, HTML, PDF, XPS, TIFF, MHTML, Markdown, TXT, XAML, OpenXPS, EPUB, SVG, PS, PCL

      tab_three:
        description: |
          Java용 GroupDocs.Assembly는 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다.
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * 마이크로소프트 윈도우 데스크탑
                * 마이크로소프트 윈도우 서버
                * 리눅스
                * 맥 OS

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * 자바 7(1.7) 이상

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "개발 환경"
              content: |
                * 넷빈
                * IntelliJ 아이디어
                * 이클립스
            - icon: "fas fa-tools"
              title: "빌드 자동화 도구"
              content: |
                * 메이븐

features:
    enable: true
    title: "Java 기능을 위한 GroupDocs.Assembly"

    feature:
      - icon: "fas fa-copy"
        content: "이미지 비율을 유지하면서 Word, Excel, 프레젠테이션 및 이메일의 텍스트 상자에서 이미지 조정"

      - icon: "fas fa-eye"
        content: "수식 사용 및 순차적 데이터 작업 수행 - 스프레드시트 조립 중 수식 적용"

      - icon: "fas fa-bolt"
        content: "템플릿 구문의 문자열에 Upper, Lower, Capital, FirstCap 서식 적용"
      
      - icon: "fas fa-file-powerpoint"
        content: "템플릿 구문 지원 Ordinal, Cardinal, Alphabetic Numeric Nature의 서식 지정"

      - icon: "fas fa-code"
        content: "템플릿 구문 태그 내에서 사용자 정의 변수 및 텍스트 주석이 있는 템플릿 문서 지원"

      - icon: "fas fa-cloud"
        content: "보고서에 문서 내용을 동적으로 삽입"

      - icon: "fas fa-remove-format"
        content: "HTML 문서의 배경색을 동적으로 구성하고 보고서에서 바코드 생성"

      - icon: "fas fa-comment-slash"
        content: "보고서에 동적으로 하이퍼링크 삽입 및 이메일 메시지 본문에 속성 적용"

      - icon: "fas fa-location-arrow"
        content: "워드 프로세싱 문서 어셈블리 중 이메일 첨부 파일을 동적으로 첨부하고 필드 업데이트"

      - icon: "fas fa-border-all"
        content: "Microsoft Word의 NEXT Field Analogue 지원"

      - icon: "fas fa-wrench"
        content: "문서 형식에 링크 및 책갈피를 동적으로 추가하고 Excel 스프레드시트의 셀 범위 이름 지정"

      - icon: "fas fa-columns"
        content: "조립된 POT 및 OTP 프레젠테이션 문서 형식 로드 및 저장"

      - icon: "fas fa-file-word"
        content: "숫자, 텍스트, 이미지, 날짜-시간, 차트 요소에 대한 템플릿 서식 지정"

      - icon: "fas fa-envelope"
        content: "Base64로 인코딩된 바이트에서 이미지 및 문서를 동적으로 삽입"

      - icon: "fas fa-print"
        content: "LINQ 기반 템플릿 구문"

      - icon: "fas fa-file-archive"
        content: "명시적 사양 또는 파일 확장자를 사용하여 어셈블된 파일의 형식 변경"

      - icon: "fas fa-lock"
        content: "Markdown 지원되는 주문 목록 - Markdown에 새로 조립된 이메일 및 Word 문서 저장"

      - icon: "fas fa-file-code"
        content: "차트, 이미지, 테이블, 목록 등 다양한 보고서 유형 생성"
      
      - icon: "fas fa-fill-drip"
        content: "예외 발생 대신 생성된 문서의 인라인 템플릿 구문 오류"

      - icon: "fas fa-file-excel"
        content: "HTML 및 RTF 본문이 포함된 이메일은 물론 Word 문서의 번호 매기기 목록을 동적으로 다시 시작"

      - icon: "fas fa-heading"
        content: "조립된 마크다운 문서에 대한 테이블, 자동 링크, 인라인 링크 및 이미지 지원"

      - icon: "fas fa-project-diagram"
        content: "동적으로 바코드 생성(GS1-128 AI 8102 쿠폰 확장 및 UPCA 및 GS1 데이터바 쿠폰"

      - icon: "fas fa-cube"
        content: "리소스가 포함된 HTML에서 템플릿 문서 로드 및 리소스가 포함된 HTML에 조립된 Word, Excel, PowerPoint 및 이메일 저장"

    more_feature:
      - title: "템플릿 요소 조작"
        content: |
          Java API용 GroupDocs.Assembly로 수많은 템플릿 요소를 조작합니다. 작업할 수 있는 템플릿 요소에는 텍스트 블록, 이미지, 하이퍼링크, HTML 블록, 바코드(바코드 글꼴 사용) 및 차트가 있습니다. 목록 항목 및 테이블 행에 대해 반복 블록 및 조건부 블록을 적용할 수도 있습니다. HTML 및 RTF 본문이 있는 문서, 프리젠테이션, 스프레드시트 및 이메일에 대한 템플릿 표현식을 기반으로 동일한 텍스트를 포함하는 테이블 셀의 동적 병합.
      
      - title: "목록 보고서 조작"
        content: |
          Java API용 GroupDocs.Assembly를 사용하여 다음 유형의 목록 보고서를 지원합니다.  

          * 글머리 기호 목록
          * 번호 매기기 목록
          * 컬러 번호 매기기 목록

      - title: "차트 보고서 조작"
        content: |
          Java용 GroupDocs.Assembly는 다음 유형의 차트 보고서를 지원합니다.

          * 3차원 데이터를 표시하는 거품형 차트
          * 기둥형 차트
          * 파이 차트
          * 분산형 차트
          * 시리즈 차트(컬러)

      - title: "테이블 보고서 조작"
        content: |
          Java용 GroupDocs.Assembly는 다음 유형의 테이블 보고서를 지원합니다.  

          * 마스터-디테일 테이블
          * 강조 표시된 행이 있는 표
          * 대체 콘텐츠가 있는 표
          * 필터링, 그룹화 및 정렬이 포함된 테이블  

          테이블 행에서 단면정보 테이블을 사용할 수도 있습니다.

      - title: "차트 보고서 조작"
        content: |
          Java API용 GroupDocs.Assembly를 Java 애플리케이션과 통합하는 것은 매우 쉽습니다. 다음은 Java를 사용하여 OpenDocument 형식으로 보고서를 생성하는 예제 코드 블록입니다.  

          ```java
          // DocumentAssembler 클래스 인스턴스화
          DocumentAssembler assembler = new DocumentAssembler();
          //AssembleDocument를 호출하여 보고서 생성
          assembler.assembleDocument("D:\\WordTemplates\\Nested External Document.docx", "D:\\WordReports\\Nested External Document.docx", 
          new DataSourceInfo( new DataStorage(), null));
          //(https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java에서 새로운 DataStorage() 메서드 세부 정보 참조)
          ```

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Assembly는 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        - img_alt: "GroupDocs.Assembly for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
          product: "GroupDocs.Assembly"
          platform: ".NET"
          link: "/assembly/net/"

back_to_top:
  enable: true
---
