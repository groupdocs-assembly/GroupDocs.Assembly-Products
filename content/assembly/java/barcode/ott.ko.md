---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/assembly/java/barcode/ott/"
otherformats: DOC DOCX DOCM DOT DOTX DOTM RTF ODT 

############################# Head ############################
head_title: "Java를 통한 워드 프로세싱 문서의 바코드 생성 및 편집"
head_description: "GroupDocs.Assembly Java API를 사용하면 프로그래머가 Word(DOC, DOCX, DOCM, DOT, DOTX, RTF 및 ODT) 문서 내에서 바코드 이미지를 생성, 추가 및 편집할 수 있습니다."

############################# Header ############################
title: "Java API를 통해 Word OTT 문서에서 바코드 이미지 생성"
description: "GroupDocs.Assembly Java API를 사용하면 소프트웨어 개발자가 Java 애플리케이션 내부의 Word OTT 문서 내에서 바코드 이미지를 동적으로 만들고 수정할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "워드 프로세싱 문서에서 바코드를 만들고 편집하는 방법은 무엇입니까?"
    content: |
     바코드는 인기를 얻고 있으며 오늘날 모든 곳에서 사용됩니다. 1970년대 중반에 식료품점에 나타나기 시작했으며 오늘날에는 책, 티켓, 의약품 추적을 위한 병원, 자동차 부품점 등에서 찾을 수 있습니다. 이 웹 페이지에서는 Java 애플리케이션 내에서 다양한 유형의 문서 및 이메일에 바코드 이미지를 동적으로 생성하고 추가하는 방법을 설명합니다. Java용 GroupDocs.Assembly는 소프트웨어 개발자가 강력한 문서 자동화 및 보고 응용 프로그램을 만드는 데 도움이 되는 매우 유용한 API입니다. PDF, HTML, XPS, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook 전자 메일 등과 같은 많은 인기 있는 문서 형식을 처리하기 위한 지원을 제공합니다. Java API를 사용하면 몇 줄의 코드로 문서와 이메일 메시지에 바코드 이미지를 쉽게 만들고 삽입할 수 있습니다. 또한 바코드 이미지 크기 조정, 앞뒤 색상 변경, 바코드 이미지 해상도 변경, 바코드 텍스트 배치, 글꼴 변경 등과 같은 바코드 이미지 속성 수정을 지원합니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "OTT 문서에서 바코드 이미지 생성"
      content_left: |
       다음 자바 코드 예제는 Microsoft Word OTT 문서 내에서 바코드 이미지의 동적 생성 및 삽입을 보여줍니다. 개발자는 몇 줄의 Java 코드를 사용하여 작업을 수행할 수 있습니다.

      title_right: "Java를 통해 OTT 파일에 바코드 추가"
      content_right: |
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler) 의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.DataSourceInfo...-) 다음 매개변수가 있는 메서드 를 호출합니다,
           * 템플릿 문서를 읽을 스트림.
           * 결과 문서를 작성하는 스트림.
           * 문서 로드 및 저장 옵션.
           * Details 사용할 데이터 소스 개체에 대한 정보입니다.

     
      gisthash: "eaf50ed48706b66730933fc4b57cdd87"
      gistfile: "barcodes_creation_in_word_documents.java"

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