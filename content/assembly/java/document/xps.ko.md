---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/assembly/java/document/xps"
otherformats: PDF HTML TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Java API: XPS 파일 형식에 외부 문서 콘텐츠 추가"
head_description: "GroupDocs.Assembly Java API를 사용하면 외부 문서의 콘텐츠를 PDF, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG 등과 같은 다양한 파일 형식으로 동적으로 삽입할 수 있습니다."

############################# Header ############################
title: "지원되는 다른 파일 형식에 외부 문서의 내용을 삽입하는 Java API"
description: "Java용 GroupDocs.Assembly는 보고서, 이메일 및 PDF, DOC, DOCX, XLSX, CSV, PPTX, EML, MSG 등과 같은 다양한 지원 파일 형식에 외부 문서의 내용을 삽입하는 기능을 제공합니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java를 통해 외부 문서의 내용을 다른 인기 있는 파일 형식에 삽입하는 방법은 무엇입니까?"
    content: |
       문서 또는 파일은 사용자가 나중에 검색할 수 있는 정보를 포함하는 전자 사본 또는 하드 카피입니다. Wikipedia에 따르면 문서는 표 형식의 문서, 목록, 형식 또는 과학 차트와 같이 구조화되거나 책이나 신문 기사와 같이 반구조화되거나 손으로 쓴 메모와 같이 구조화되지 않을 수 있습니다. Java용 GroupDocs.Assembly는 소프트웨어 개발자가 문서 자동화 및 보고를 위한 강력한 애플리케이션을 구축할 수 있도록 하는 매우 유용한 API입니다. PDF, Microsoft Word, Excel 워크시트, PowerPoint, HTML, Outlook 이메일 등과 같은 다양한 문서 형식을 식별하고 작업하는 것을 완벽하게 지원합니다. 템플릿 요소 조작, 목록 보고서, 차트 보고서, 테이블 보고서 등과 같은 보고서 작업을 위한 다양한 고급 기능을 지원합니다. 또한 API는 문서 페이지에 콘텐츠 추가, 스프레드시트 셀에 데이터 삽입, 콘텐츠 교체, 프레젠테이션 슬라이드에 콘텐츠 추가 등과 같은 문서 콘텐츠 추가 및 수정과 관련된 여러 고급 기능을 완벽하게 지원합니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java를 통해 Word 문서에 외부 파일 내용 추가"
      content_left: |
       GroupDocs.Assembly Java API는 컴퓨터 프로그래머가 자체 Java 앱 내에서 문서 조작 작업을 처리하는 데 도움이 됩니다. 다양한 문서 유형에 대한 외부 문서의 파일 내용을 완벽하게 지원합니다. 다음 Java 코드 예제는 몇 줄의 코드로 외부 파일의 내용을 워드 프로세싱 문서에 추가하는 방법을 보여줍니다.

      title_right: "문서 내용을 XPS 파일에 삽입하는 방법"
      content_right: |
        * 소스 문서 템플릿 설정
        * 대상 문서 보고서 설정
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 클래스의 인스턴스 생성
        * 호출 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 문서를 어셈블하는 메서드입니다. 그것은 지원
          * 템플릿 문서를 읽을 스트림입니다.
          * 결과 문서를 작성하기 위한 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션을 지정합니다.
          * 사용할 데이터 소스 개체에 대한 정보를 제공합니다.

      gisthash: "abb65f9e514add59870865121ed3c526"
      gistfile: "insert_documents_to_word_processing.java"

    - title_left: "Java를 통해 이메일 메시지에 외부 파일 내용 추가"
      content_left: |
       GroupDocs.Assembly Java API에는 여러 인기 있는 문서 파일 형식 및 전자 메일 메시지에 대한 동적 외부 문서 콘텐츠 삽입 기능이 포함되어 있습니다. 아래 자바 코드는 프로그래머가 외부 애플리케이션 없이 이메일 문서에 외부 문서의 내용을 추가할 수 있는 방법을 보여줍니다.

      title_right: "파일 내용을 XPS 문서에 추가하는 방법"
      content_right: |
        * 소스 문서 템플릿 설정
        * 대상 문서 보고서 설정
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 클래스의 인스턴스 생성
        * 호출 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 문서를 어셈블하는 메서드입니다. 그것은 지원
          * 템플릿 문서를 읽을 스트림입니다.
          * 결과 문서를 작성하기 위한 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션을 지정합니다.
          * 사용할 데이터 소스 개체에 대한 정보를 제공합니다.

      gisthash: "b72d7608548993ffbe62f97c798ba021"
      gistfile: "Insert_dynamic_documents_to_emails.java"

    - title_left: "시스템 요구 사항"
      content_left: |
        GroupDocs.Assembly Java API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice 및 50개 이상의 기타 형식으로 문서를 생성할 수 있습니다. 전체 시스템 요구 사항 가이드를 보려면 [시스템 요구 사항](https://docs.groupdocs.com/assembly/java/system-requirements/)을 방문하십시오. 아래 코드를 실행하기 전에 다음 전제 조건이 컴퓨터에 설치되어 있는지 확인하십시오. 체계:
         * 운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
         * 자바 버전 지원: J2SE 7.0(1.7), J2SE 8.0(1.8) 이상
         * [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/)에서 최신 버전의 GroupDocs.Assembly Java API 다운로드
        
      title_right: "GroupDocs.Assembly를 사용하는 이유"
      content_right: |
        * 템플릿에서 사용자 정의 문서를 만듭니다.
        * 이메일 첨부 파일을 동적으로 첨부합니다.
        * 문서를 만들고 자동화하는 데 추가 소프트웨어가 필요하지 않습니다.
        * 데이터 소스를 기반으로 출력 문서를 생성합니다.
        * 보고서에 문서 내용을 동적으로 삽입
        * 스프레드시트 조립 중에 수식을 적용합니다.
        * 여러 데이터 형식에 대한 지원 제공
        * 순차적 데이터 작업 지원.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---