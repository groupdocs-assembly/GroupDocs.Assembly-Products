



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:54
draft: false
lang: ko
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# API로 XLSX 문서를 다른 문서에 삽입하기"
head_description: "C#을 사용하여 XLSX 문서를 손쉽게 병합하세요. GroupDocs.Assembly와 함께 몇 가지 단계로 파일을 원활하게 결합할 수 있습니다."

############################# Header ############################
title: "XLSX 형식의 문서 결합하기" 
description: "GroupDocs.Assembly for .NET을 사용하면 하나의 XLSX 문서를 다른 문서에 빠르게 삽입할 수 있습니다. 이 API는 정밀한 문서 병합을 위한 강력한 도구를 제공합니다."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET란?"
    link: "/assembly/net/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)은 문서 구성 및 조작을 위한 강력한 도구입니다. 사용자가 한 문서를 다른 문서에 삽입할 수 있어 콘텐츠를 원활하게 병합할 수 있습니다. 50개 이상의 형식—PDF, MS Office 파일 등—을 지원하며, 최종 출력물을 필요한 대로 구성, 편집, 맞춤 설정할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX 파일에 문서 병합하는 방법"
    content: |
      [GroupDocs.Assembly](/assembly/net/)로 다른 XLSX 파일에 하나의 문서를 원활하게 삽입하세요. 콘텐츠를 병합하고 맞춤 설정할 수 있습니다.
      
      1. XLSX 템플릿을 설계하고 삽입 문서를 위한 자리 표시자를 포함하세요.
      2. 템플릿을 위한 파일 경로를 정의하세요.
      3. 삽입할 문서의 파일 경로를 지정하세요.
      4. 삽입된 콘텐츠로 최종 파일을 저장하세요.
   
    code:
      platform: "net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "예제 문서"
      install:
        command: "dotnet add package GroupDocs.Assembly"
        copy_tip: "복사하려면 클릭"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/assembly/net/"
          
      content: |
        ```csharp {style=abap}
        // 삽입 지점을 표시하기 위해 템플릿에 이 태그를 추가하세요.
        // <<doc [doc_expression]>>

        // 템플릿의 파일 경로를 지정하세요.
        string template = "doc_template.xlsx";

        // 삽입할 문서의 경로를 제공하세요.
        DataSourceInfo data 
            = new DataSourceInfo("insert.xlsx", "doc_expression");

        // 병합된 문서를 저장하세요.
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.xlsx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 도구로 문서 병합 간소화하기"
  description: "GroupDocs.Assembly for .NET 라이브러리는 다양한 파일 형식을 지원하며 원활한 통합을 위한 맞춤 설정 기능을 제공하여 하나의 문서를 다른 문서에 쉽게 삽입할 수 있습니다."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "비즈니스 데이터에서 보고서 생성"
      content: "JSON, XML, CSV 또는 기타 소스의 데이터를 사용하여 문서를 자동으로 채워 정확하고 효율적인 워크플로를 보장합니다."

    # feature loop
    - title: "시각 요소로 문서 풍부하게 하기"
      content: "GroupDocs.Assembly는 테이블, 차트, 목록, 텍스트, 링크, 이미지 및 동적으로 생성된 바코드를 포함할 수 있게 해줍니다."

    # feature loop
    - title: "데이터의 위치와 형식 정확하게 지정"
      content: "LINQ 기반 템플릿을 통해 데이터 배치를 제어하고 배열을 위한 루프를 처리하며 색상 맞춤 설정과 같은 스타일링을 허용합니다."

    # feature loop
    - title: "다양한 파일 형식과 호환"
      content: "MS Office, PDF, HTML, OpenOffice 등 다양한 형식 간에 문서를 쉽게 삽입할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "프로그램matically 이미지를 문서에 삽입하는 방법"
      content: |
        이 예제에서는 GroupDocs.Assembly를 사용하여 XLSX 문서에 이미지를 삽입하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 템플릿에 자리 표시자 태그를 추가하세요.
          // <<image [expression]>>

          // 템플릿의 파일 경로를 지정하세요.
          string template = "template.xlsx";

          // 이미지 파일의 경로를 설정하세요.
          DataSourceInfo data =
              = new DataSourceInfo("logo.jpg", "expression");

          // DocumentAssembler의 인스턴스를 초기화하세요.
          DocumentAssembler asm = new DocumentAssembler();

          // 삽입된 이미지로 문서를 저장하세요.
          asm.AssembleDocument(template, "result.xlsx", data);
          ```
        platform: "net"
        copy_title: "복사"
        install:
          command: "dotnet add package GroupDocs.Assembly"
          copy_tip: "복사하려면 클릭"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/assembly/formats/assembly_document.xlsx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-.NET/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/assembly/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Assembly의 기능을 무료로 탐색하거나 라이센스를 요청하세요"
  items:
    #  loop
    - title: "Nuget에서 다운로드"
      link: "https://releases.groupdocs.com/assembly/net/"
      color: "red"
        #  loop
    - title: "라이센스에 대해 알아보세요"
      link: "https://purchase.groupdocs.com/pricing/assembly/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "강력한 도구 발견하기"
    exclude: "document"
    description: "GroupDocs.Assembly가 제공하는 문서 삽입 및 병합 기능을 탐색하십시오."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/net/barcode/xlsx/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/net/chart/xlsx/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/net/document/xlsx/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/net/list/xlsx/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/net/table/xlsx/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식의 문서 병합"
    exclude: "XLSX"
    description: ".NET API로 50개 이상의 지원 형식 간에 문서를 결합할 수 있습니다. 파일이나 섹션을 최종 문서에 손쉽게 삽입하세요."
    items: 
          
        # format loop 1
        - name: "PDF에 문서 삽입"
          format: "PDF"
          link: "/assembly/net/document/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 문서 삽입"
          format: "DOCX"
          link: "/assembly/net/document/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 문서 삽입"
          format: "PPTX"
          link: "/assembly/net/document/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 문서 삽입"
          format: "XLSX"
          link: "/assembly/net/document/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---