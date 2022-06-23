---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

head_title: ".문서 자동화, 어셈블리 및 보고서 생성을 위한 NET API"
head_description: "C# .NET 문서 자동화, 어셈블리 및 보고서 생성 API. 사용자 정의 템플릿에서 PDF Word Excel PPTX HTML 및 이메일 문서 만들기."

title: ".NET 문서 자동화 및 보고 API"
description: "템플릿을 정의하고 데이터를 병합하여 .NET 애플리케이션에서 보고서 생성."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Assembly for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-net.png"
        product: "GroupDocs.Assembly"
        platform: ".NET"

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

            - link: "https://purchase.groupdocs.com/pricing/assembly/net"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/assembly"
        link_learn: "https://docs.groupdocs.com/assembly/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      .NET API용 GroupDocs.Assembly를 사용하면 C#, ASP.NET 및 기타 .NET 관련 응용 프로그램의 사용자 지정 템플릿에서 보고서를 생성할 수 있는 기능을 통해 강력한 문서 자동화 및 보고서 생성 응용 프로그램을 구축할 수 있습니다. 몇 줄의 코드로 .NET 보고 라이브러리는 정의된 문서 템플릿에서 주어진 데이터를 지능적으로 조합하고 다양한 데이터 소스(데이터베이스, XML, JSON, ODATA, CSV, 사용자 지정 .NET 개체).  

      LINQ 기반 템플릿 구문을 지원하며 사용자는 PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션 및 슬라이드와 같이 일반적으로 사용되는 모든 비즈니스 파일 형식으로 출력 문서를 쉽게 생성할 수 있습니다. 템플릿 요소의 서식 속성은 텍스트, HTML 및 조건부 블록, 이미지, 차트, 바코드, 하이퍼링크, 피벗 테이블 등을 조작하여 구성할 수도 있습니다.  

      .NET용 GroupDocs.Assembly는 .NET 플랫폼을 대상으로 하는 모든 개발 환경에서 응용 프로그램을 개발하는 데 사용할 수 있습니다. 모든 .NET 기반 언어와 호환되며 Mono 또는 .NET 프레임워크(.NET Core 포함)를 설치할 수 있는 인기 있는 운영 체제(Windows, Linux, MacOS)를 지원합니다.
    tabs:
      enable: true
      
      tab_one:
        description: |
          다음은 .NET용 GroupDocs.Assembly의 개요입니다.
      
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
          .NET 문서 생성 API에 지원되는 [문서 파일 형식](https://docs.groupdocs.com/assembly/net/supported-document-formats/)은 다음과 같습니다.

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
          .NET용 GroupDocs.Assembly는 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다.
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * 윈도우 데스크탑
                * 윈도우 서버
                * 윈도우 애저
                * 리눅스

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * .NET 프레임워크 2.0 이상
                * 모노 프레임워크 1.2 이상

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "패키지 관리자"
              content: |
                * 누겟

            - icon: "fas fa-tools"
              title: "개발 환경"
              content: |
                * 마이크로소프트 비주얼 스튜디오
                * 자마린.안드로이드
                * 자마린.IOS
                * 자마린.맥
                * 모노디벨롭

features:
    enable: true
    title: ".NET 기능을 위한 GroupDocs.Assembly"

    feature:
      - icon: "fas fa-copy"
        content: "여러 데이터 형식에서 작동"

      - icon: "fas fa-eye"
        content: "수식 및 순차 데이터 연산을 사용하여 데이터 조작 가능"

      - icon: "fas fa-bolt"
        content: "템플릿 구문의 문자열 형식을 Upper, Lower, Capital, FirstCap으로 지정"
      
      - icon: "fas fa-file-powerpoint"
        content: "템플릿 구문에서 서수, 기본, 알파벳 숫자 형식 지정 수행"

      - icon: "fas fa-code"
        content: "템플릿 문서에서 변수 정의 및 템플릿 구문 태그 내에서 텍스트 주석 지원"

      - icon: "fas fa-cloud"
        content: "보고서에 외부 문서의 내용을 동적으로 삽입"

      - icon: "fas fa-remove-format"
        content: "보고서에서 동적으로 바코드 이미지 생성 및 HTML 문서의 배경색 설정"

      - icon: "fas fa-comment-slash"
        content: "이메일 메시지 본문에 동적으로 속성 할당 및 보고서에 하이퍼링크 삽입"

      - icon: "fas fa-location-arrow"
        content: "동적으로 이메일 메시지 첨부 파일 작성"

      - icon: "fas fa-border-all"
        content: "Microsoft Word NEXT 필드의 아날로그 지원"

      - icon: "fas fa-wrench"
        content: "워드 프로세싱 문서를 어셈블하는 동안 필드 업데이트"

      - icon: "fas fa-columns"
        content: "스프레드시트 문서를 조합하는 동안 공식 계산"

      - icon: "fas fa-file-word"
        content: "서식 숫자, 텍스트, 이미지, 차트, 템플릿의 날짜-시간 요소"

      - icon: "fas fa-envelope"
        content: "조립된 POT 및 OTP 프레젠테이션 문서 형식 로드 및 저장"

      - icon: "fas fa-print"
        content: "템플릿에 LINQ 기반 구문 사용 및 템플릿 요소의 조건부 텍스트 서식 수행"

      - icon: "fas fa-file-archive"
        content: "파일 확장자 또는 명시적 사양을 사용하여 어셈블된 문서의 파일 형식 변경"

      - icon: "fas fa-lock"
        content: "Markdown 지원되는 주문 목록 - Markdown에 새로 조립된 이메일 및 Word 문서 저장"

      - icon: "fas fa-file-code"
        content: "차트, 목록, 표, 이미지 등 다양한 유형의 보고서 지원"
      
      - icon: "fas fa-fill-drip"
        content: "예외 발생 대신 생성된 문서의 인라인 템플릿 구문 오류"

      - icon: "fas fa-file-excel"
        content: "리소스가 포함된 HTML에서 템플릿 문서 로드 및 리소스가 포함된 HTML에 조립된 Word, Excel, PowerPoint 및 이메일 저장"

      - icon: "fas fa-heading"
        content: "HTML 및 RTF 본문을 사용하여 Word 문서 형식 및 이메일에 동적으로 다시 시작 목록 번호 매기기 추가"

      - icon: "fas fa-project-diagram"
        content: "Base64로 인코딩된 바이트에서 이미지 및 문서를 동적으로 삽입하고 Word 문서의 확인란 값 설정 조정"

      - icon: "fas fa-cube"
        content: "이미지 비율을 유지하면서 Word, Excel, 프레젠테이션 및 이메일의 텍스트 상자에서 이미지 늘이기"

      - icon: "fab fa-uncharted"
        content: "문서 형식에 링크 및 책갈피를 동적으로 추가하고 Excel 스프레드시트의 셀 범위 이름 지정"

    more_feature:
      - title: "템플릿 요소 지원"
        content: |
          .NET API용 GroupDocs.Assembly를 사용하면 수많은 템플릿 요소로 작업할 수 있습니다. 서식이 지정된 텍스트 블록, HTML 블록, 이미지, 차트, 하이퍼링크 및 바코드(바코드 글꼴을 통해)로 작업할 수 있습니다. 목록 항목 및 테이블 행을 포함하여 반복 블록 및 조건부 블록도 지원됩니다. HTML 및 RTF 본문이 있는 스프레드시트, 프리젠테이션, 문서 및 이메일에 대한 템플릿 표현식을 기반으로 동일한 텍스트가 포함된 테이블 셀을 동적으로 병합할 수도 있습니다.

      - title: "목록 보고서 작업"
        content: |
          .NET API용 GroupDocs.Assembly를 사용하여 다음 세 가지 유형의 목록 보고서로 작업할 수 있습니다.  

          * 글머리 기호 목록
          * 번호 매기기 목록
          * 컬러 번호 매기기 목록

      - title: "차트 보고서 작업"
        content: |
          .NET용 GroupDocs.Assembly는 다음 유형의 차트 보고서를 지원합니다.  

          * 3차원 데이터를 표시하는 거품형 차트
          * 기둥형 차트
          * 파이 차트
          * 분산형 차트
          * 시리즈 차트(컬러)

      - title: "테이블 보고서 작업"
        content: |
          .NET용 GroupDocs.Assembly는 다음 유형의 테이블 보고서를 지원합니다.  

          * 마스터-디테일 테이블
          * 강조 표시된 행이 있는 표
          * 대체 콘텐츠가 있는 표
          * 필터링, 그룹화 및 정렬이 포함된 테이블  
          
          테이블 행에서 단면정보 테이블을 사용할 수도 있습니다.

      - title: "쉬운 통합"
        content: |
          몇 줄의 코드를 사용하여 .NET API용 GroupDocs.Assembly를 .NET 애플리케이션과 쉽게 통합할 수 있습니다. 다음은 공개 문서 형식으로 보고서를 생성하기 위한 예제 코드입니다.

          ```cs
          // DocumentAssembler 클래스 인스턴스화
          DocumentAssembler assembler = new DocumentAssembler();
          //AssembleDocument를 호출하여 보고서 생성
          assembler.AssembleDocument("D:\\WordTemplates\\Barcode.docx", "D:\\WordReports\\Barcode.docx", new DataSourceInfo(DataLayer.GetCustomerData(), 
          "customer"));
          //(https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET에서 DataLayer.GetCustomerData() 메서드 세부 정보 참조)
          ```

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Assembly는 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        - img_alt: "GroupDocs.Assembly for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-assembly-java.png"
          product: "GroupDocs.Assembly"
          platform: "Java"
          link: "/assembly/java/"

back_to_top:
  enable: true
---
