---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/assembly/net/document/xlsb/"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: ".NET API를 통해 이메일 및 XLSB 파일에 외부 문서 콘텐츠 삽입"
head_description: "GroupDocs.Assembly .NET API를 사용하면 프로그래머가 외부 문서의 내용을 PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG 및 기타 파일 형식에 동적으로 삽입할 수 있습니다."

############################# Header ############################
title: ".NET API를 통해 Office 파일 및 이메일 메시지에 외부 문서 콘텐츠 삽입"
description: "GroupDocs.Assembly .NET API는 PDF DOCX, XLSX, CSV, PPTX, MSG 등과 같은 보고서, 이메일 및 Office 문서에 외부 문서 콘텐츠의 동적 삽입을 완벽하게 지원합니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NET을 통해 외부 문서의 내용을 다른 파일, 보고서 및 이메일에 삽입하는 방법은 무엇입니까?"
    content: |
       문서 또는 문서 파일은 사용자가 나중에 검색할 수 있는 디지털 및 비디지털 정보 집합을 나타냅니다. 컴퓨터 또는 디지털 문서는 컴퓨터 시스템 내부에 저장할 수 있는 소프트웨어 응용 프로그램에서 만든 파일입니다. 일반적으로 워드 프로세서 또는 텍스트 편집기는 컴퓨터 시스템에서 전자 문서를 작성하는 데 사용됩니다. .NET용 GroupDocs.Assembly는 소프트웨어 개발자가 문서를 쉽게 만들고 관리하는 데 사용할 수 있는 강력한 응용 프로그램 소프트웨어를 만드는 데 도움이 되는 매우 유용한 API입니다. 소프트웨어 개발자는 외부 문서의 내용을 보고서, 이메일 및 Office 문서에 동적으로 삽입할 수 있습니다. PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션 등과 같이 매우 일반적으로 사용되는 일부 문서 유형에 대한 지원을 제공했습니다. 또한 문서 페이지에 콘텐츠 삽입, 스프레드시트 셀에 삽입, 콘텐츠 편집 또는 교체, 프레젠테이션 슬라이드에 콘텐츠 삽입 등과 같은 문서 콘텐츠 삽입 및 편집과 관련된 일부 고급 기능이 완벽하게 지원됩니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET을 통해 Word 파일에 외부 문서 내용 삽입"
      content_left: |
       GroupDocs.Assembly .NET API를 사용하면 소프트웨어 개발자가 외부 문서의 내용을 다양한 유형의 문서 및 이메일 메시지에 쉽게 삽입할 수 있습니다. 아래 .NET 코드 예제는 몇 줄의 코드로 외부 문서의 내용을 워드 프로세싱 문서에 삽입하는 방법을 보여줍니다. 

      title_right: "문서 콘텐츠를 XLSB 파일에 추가하는 방법"
      content_right: |
        * 소스 오픈 문서 템플릿 설정
        * 대상 오픈 문서 보고서 설정
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 클래스의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) 메서드를 호출하여 오픈 문서 형식으로 Report를 생성합니다. 그것은 지원
          * 지정된 소스 경로에서 템플릿 문서를 로드합니다.
          * 지정된 단일 또는 여러 소스의 데이터로 템플릿 문서를 채웁니다.
          * 주어진 LoadSaveOptions를 사용하여 결과 문서를 대상 경로에 저장합니다.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "c4dc0be4f8ab8c2ba4ee6a78673ca1cd"
      gistfile: "dynamic_documents_insertion_to_word_processing.cs"

    - title_left: ".NET을 통해 이메일에 외부 문서의 내용 삽입"
      content_left: |
       GroupDocs.Assembly .NET API를 사용하면 문서 내부에 다양한 종류의 문서 유형과 내용을 추가하고 관리할 수 있습니다. 외부 문서의 내용을 다양한 문서 유형 및 이메일 파일 형식에 동적으로 삽입할 수 있습니다. 다음 C# 코드는 사용자가 외부 문서의 콘텐츠를 자신의 .NET 앱 내부에 있는 문서 및 이메일 메시지에 얼마나 쉽게 삽입할 수 있는지 보여줍니다.

      title_right: "C#을 통해 이메일 메시지에 문서 내용 추가"
      content_right: |
        * 소스 오픈 문서 템플릿 설정
        * 대상 오픈 문서 보고서 설정
        * [DocumentAssembler](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly/documentassembler) 클래스의 인스턴스 생성
        * [AssembleDocument](https://apireference.groupdocs.com/assembly/net/groupdocs.assembly.documentassembler/assembledocument/methods/3) 메서드를 호출하여 오픈 문서 형식으로 Report를 생성합니다. 그것은 지원
          * 지정된 소스 경로에서 템플릿 문서를 로드합니다.
          * 지정된 단일 또는 여러 소스의 데이터로 템플릿 문서를 채웁니다.
          * 주어진 LoadSaveOptions를 사용하여 결과 문서를 대상 경로에 저장합니다.
          * 데이터 소스 개체에 대한 정보입니다.

      gisthash: "8fe014550c5f05467da6910a7ee16f18"
      gistfile: "dynamic_documents_insertion_to_emails_dotnet.cs"

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