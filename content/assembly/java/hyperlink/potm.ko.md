---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/assembly/java/hyperlink/potm/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX ODP EML EMLX MSG 

############################# Head ############################
head_title: "Java API를 통해 Office POTM 문서 및 보고서에 하이퍼링크 추가"
head_description: "Java용 GroupDocs.Assembl은 PDF DOCX, RTF, XLSX, PPTX, EML, MSG 등과 같은 사무실 및 이메일 문서에 대한 하이퍼링크의 동적 삽입을 Java 앱 내에서 지원합니다."

############################# Header ############################
title: "Java API를 통해 Office 문서 및 이메일에 하이퍼링크 추가"
description: "GroupDocs.Assembly Java API를 사용하면 소프트웨어 전문가가 PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, MSG 등과 같은 전자 메일 메시지 및 Office 문서에 대한 하이퍼링크를 프로그래밍 방식으로 추가할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java API를 사용하여 Office 및 이메일 문서에 하이퍼링크를 추가하는 방법은 무엇입니까?"
    content: |
       하이퍼링크는 클릭하여 새 문서나 현재 문서 내의 새 섹션으로 이동할 수 있는 단어, 구 또는 이미지입니다. 하이퍼링크는 월드 와이드 웹의 백본이며 월드 와이드 웹에서 필요한 많은 기능에 사용됩니다. Java용 GroupDocs.Assembly는 소프트웨어 개발자가 문서 또는 보고서 내부에 하이퍼링크를 쉽게 동적으로 삽입할 수 있도록 도와주는 문서 자동화 및 보고서 생성 API입니다. API는 매우 안정적이며 문서 페이지에 하이퍼링크 추가, 프레젠테이션 슬라이드에 링크 추가, 스프레드시트 셀에 하이퍼링크 추가, 하이퍼링크 내용 수정, 책갈피에서 동적으로 링크 삽입, 원치 않는 삭제와 같은 하이퍼링크 관리와 관련된 여러 고급 기능을 완벽하게 지원합니다. 링크, 하이퍼링크 대신 텍스트 표시 등. PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션 등과 같은 매우 일반적인 문서 유형 중 일부가 완벽하게 지원됩니다. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java를 통해 워드 프로세싱 문서에 하이퍼링크 삽입"
      content_left: |
       GroupDocs.Assembly Java API는 일반적으로 사용되는 다양한 문서 형식 내에서 하이퍼링크의 삽입 및 편집을 완벽하게 지원합니다. 아래 Java 코드 예제는 Microsoft Word 문서 내부에 하이퍼링크를 삽입하는 방법을 보여줍니다.

      title_right: "Java를 통해 POTM 문서에 하이퍼링크 삽입"
      content_right: |
        * 소스 및 대상 문서 설정
        * Uri 표현식을 설정하고 텍스트 표현식을 표시합니다.
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 클래스의 인스턴스 생성
        * 호출 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 문서를 어셈블하는 메서드입니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "Java를 통해 스프레드시트에 하이퍼링크 추가"
      content_left: |
       GroupDocs.Assembly Java API를 사용하면 컴퓨터 프로그래머가 스프레드시트 문서 내부에 하이퍼링크를 쉽게 삽입하고 수정할 수 있습니다. 쉽게 액세스하거나 위치를 편집하거나 새 위치로 교체할 수 있습니다. 다음 Java 코드는 프로그래머가 스프레드시트 내부에 하이퍼링크를 얼마나 쉽게 추가할 수 있는지 보여줍니다.

      title_right: "POTM 파일에 하이퍼링크를 삽입하는 방법"
      content_right: |
        * 소스 및 대상 스프레드시트 파일 설정
        * Uri 표현식을 설정하고 텍스트 표현식을 표시합니다.
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 클래스의 인스턴스 생성
        * 호출 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 문서를 어셈블하는 메서드입니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "Java를 통해 PowerPoint 프레젠테이션에 하이퍼링크 삽입"
      content_left: |
       GroupDocs.Assembly Java API를 사용하면 프로그래머가 문서 관리 관련 작업을 쉽게 처리할 수 있습니다. 다음은 소프트웨어 프로그래머가 PowerPoint 프레젠테이션 문서에 액세스하고 그 안에 하이퍼링크를 추가할 수 있는 방법을 보여주는 Java 코드 예제입니다.

      title_right: "프레젠테이션에 하이퍼링크를 삽입하는 방법"
      content_right: |
        * 소스 및 대상 프리젠테이션 파일 설정
        * Uri 설정 및 텍스트 표현식 표시
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 클래스의 인스턴스 생성
        * 호출 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 문서를 어셈블하는 메서드입니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "Java API를 사용하여 이메일에 하이퍼링크 추가"
      content_left: |
       Java용 GroupDocs.Assembly를 사용하면 소프트웨어 개발자가 몇 줄의 Java 코드로 전자 메일 메시지에 하이퍼링크를 쉽게 추가할 수 있습니다. 다음 예제는 개발자가 얼마나 쉽게 이메일 문서에 하이퍼링크를 삽입하고 자신의 Java 앱 내에서 다른 사용자에게 보낼 수 있는지 보여줍니다.

      title_right: "이메일에 하이퍼링크를 추가하는 방법"
      content_right: |
        * 소스 및 대상 스프레드시트 파일 설정
        * Uri 설정 및 텍스트 표현식 표시
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 클래스의 인스턴스 생성
        * 호출 [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) 문서를 어셈블하는 메서드입니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

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