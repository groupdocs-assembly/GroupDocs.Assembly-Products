---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/assembly/net/text/pptx/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "PPTX 문서에 하이퍼링크를 동적으로 삽입하는 .NET API"
head_description: "GroupDocs.Assembly .NET API를 사용하면 개발자가 이메일, 보고서 또는 PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG 등과 같은 문서에 대한 하이퍼링크를 동적으로 삽입할 수 있습니다."

############################# Header ############################
title: ".NET API를 통해 PPTX 문서 및 보고서에 대한 하이퍼링크를 동적으로 삽입"
description: "GroupDocs.Assembly .NET API를 사용하면 프로그래머가 PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, EML, HTML, MSG 등과 같은 보고서, 이메일 및 Office 문서에 대한 하이퍼링크를 동적으로 삽입할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "보고서, 이메일 및 다양한 문서에 하이퍼링크를 동적으로 삽입하는 방법은 무엇입니까?"
    content: |
       이 웹 페이지에서는 사용자가 자신의 .NET 응용 프로그램 내에서 보고서, 전자 메일 메시지 및 다양한 문서 유형에 대한 하이퍼링크를 동적으로 삽입하는 방법을 설명합니다. 하이퍼링크는 World Wide Web의 중추이며 다른 페이지, 문서를 연결하는 데 사용하거나 을 클릭하여 현재 문서 내의 새 섹션으로 이동할 수 있습니다. GroupDocs.Assembly .NET은 소프트웨어 개발자가 단 몇 줄의 코드로 문서 또는 보고서 내부에 하이퍼링크를 동적으로 추가할 수 있도록 하는 매우 강력한 API입니다. PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션 등과 같은 매우 인기 있는 문서 유형에 대한 지원이 포함되어 있습니다. 문서 페이지에 링크 삽입, 셀에 링크 삽입, 하이퍼링크 편집, 하이퍼링크 대신 텍스트 표시, 책갈피에서 동적으로 링크 삽입, 프레젠테이션 슬라이드에 하이퍼링크 삽입 등과 같은 여러 고급 기능을 지원했습니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET을 통한 워드 프로세싱 문서에 대한 하이퍼링크 삽입"
      content_left: |
       GroupDocs.Assembly .NET API는 다양한 유형의 문서 내 하이퍼링크 삽입 및 편집을 완벽하게 지원합니다. 다음 C# .NET 코드 예제에서는 Word 문서 내에 하이퍼링크를 쉽게 추가하는 방법을 보여줍니다. 

      title_right: "Word 파일에 하이퍼링크를 추가하는 방법"
      content_right: |
        * 소스 및 대상 문서 설정
        * Uri 표현식 설정 및 디스플레이 텍스트 표현식
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 클래스의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 메서드를 호출하여 문서를 어셈블합니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "f4a8031406d44941d400088b718f7730"
      gistfile: "insert_hyperlinks_to_word_document.cs"

    - title_left: ".NET을 통해 스프레드시트에 하이퍼링크를 동적으로 삽입"
      content_left: |
       GroupDocs.Assembly .NET API는 스프레드시트 파일 내의 하이퍼링크 추가 및 처리를 완벽하게 지원합니다. 위치를 쉽게 편집하거나 새 위치로 바꿀 수 있습니다. 다음 C# 코드는 사용자가 자신의 .NET 앱 내 스프레드시트 파일에 하이퍼링크를 얼마나 쉽게 삽입할 수 있는지 보여줍니다. 

      title_right: "스프레드시트 문서에 하이퍼링크 추가"
      content_right: |
        * 소스 및 대상 문서 설정
        * Uri 표현식 설정 및 디스플레이 텍스트 표현식
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 클래스의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 메서드를 호출하여 문서를 어셈블합니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다. 

      gisthash: "c2f9cd8bb06f9a7a2c444621ebf82696"
      gistfile: "insert_hyperlinks_in_spreadsheet_documents.cs"

    - title_left: ".NET API를 통해 PowerPoint 프레젠테이션에 하이퍼링크 추가"
      content_left: |
       .NET용 GroupDocs.Assembly는 소프트웨어 전문가가 다양한 유형의 문서를 관리하기 위한 응용 프로그램을 구축하는 데 도움이 됩니다. 다음 코드 예제는 소프트웨어 개발자가 PowerPoint 프레젠테이션 문서 내에 하이퍼링크를 추가할 수 있는 방법을 보여줍니다.

      title_right: "프레젠테이션에 하이퍼링크를 추가하는 방법"
      content_right: |
        * 소스 및 대상 프리젠테이션 파일 설정
        * Uri 설정 및 텍스트 표현식 표시
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 클래스의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 메서드를 호출하여 문서를 어셈블합니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "49e1ca9eccc41942372c23c14f98ecef"
      gistfile: "insert_hyperlinks_in_presentation_documents.cs"

    - title_left: "이메일에 하이퍼링크를 삽입하는 .NET API"
      content_left: |
       GroupDocs.Assembly .NET API를 사용하면 소프트웨어 전문가가 이메일 문서에 하이퍼링크를 삽입할 수 있습니다. 다음 .NET 코드는 프로그래머가 얼마나 쉽게 이메일 메시지에 하이퍼링크를 추가하고 자신의 .NET 앱 내에서 다른 사용자에게 보낼 수 있는지 보여줍니다. 

      title_right: "이메일 문서에 하이퍼링크 추가"
      content_right: |
        * 소스 및 대상 프리젠테이션 파일 설정
        * Uri 설정 및 텍스트 표현식 표시
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 클래스의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/1) 메서드를 호출하여 문서를 어셈블합니다. 그것은 지원
          * 템플릿 문서를 읽는 스트림.
          * 결과 문서를 작성하는 스트림.
          * 문서 로드 및 저장을 위한 추가 옵션.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "8c119b4faa0334179854e164d87d3e7b"
      gistfile: "insert_hyperlinks_in_email_documents.cs"  

    - title_left: "시스템 요구 사항"
      content_left: |
       GroupDocs.Assembly .NET API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 전체 시스템 요구 사항 가이드를 보려면 [시스템 요구 사항](https://docs.groupdocs.com/assembly/net/system-requirements/)을 방문하십시오. 아래 코드를 실행하기 전에 다음 전제 조건이 컴퓨터에 설치되어 있는지 확인하십시오. 체계:
        * 운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
        * 개발 환경: Visual Studio, Xamarin, MonoDevelop 등
        * 프레임워크: .NET Framework, .NET Standard, .NET Core, Mono
        * [NuGet](https://www.nuget.org/packages/GroupDocs.Assembly/)에서 최신 버전의 GroupDocs.Assembly .NET API를 가져옵니다.
        
      title_right: "GroupDocs.Assembly를 사용하는 이유"
      content_right: |
       * 사용자가 템플릿에서 사용자 정의 문서를 만들 수 있습니다.
       * 문서 생성 및 자동화를 위해 추가 소프트웨어가 필요하지 않습니다.
       * 데이터 소스를 기반으로 출력 문서를 생성하는 기능
       * 보고서에 문서 내용을 동적으로 삽입
       * 동적으로 이메일 첨부 파일 첨부 및 보고서에 하이퍼링크 삽입
       * 빈 단락 자동 제거
       * 여러 데이터 형식에 대한 완벽한 지원
       * 동적 이메일 첨부 파일 지원

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---