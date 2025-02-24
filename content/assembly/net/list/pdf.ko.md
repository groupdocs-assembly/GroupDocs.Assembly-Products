



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:10
draft: false
lang: ko
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#를 사용하여 PDF 문서에 목록 생성"
head_description: "GroupDocs.Assembly for .NET API는 개발자가 데이터를 채운 목록을 문서와 템플릿에 동적으로 생성하고 삽입할 수 있도록 지원합니다."

############################# Header ############################
title: ".NET API를 사용하여 PDF 문서에 데이터 기반 목록 추가" 
description: "GroupDocs.Assembly for .NET는 PDF 문서에 목록을 동적으로 생성하고 삽입하기 위한 강력한 도구를 제공합니다."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험 다운로드"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET 개요"
    link: "/assembly/net/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)는 다양한 출처에서 데이터를 매끄럽게 통합하여 문서 및 보고서를 생성하는 과정을 간소화하도록 설계되었습니다. 템플릿을 목록, 차트, 표, 바코드 또는 텍스트로 채우고 고급 마크업을 사용하여 내용을 정확히 배치할 수 있습니다. 50개 이상의 형식을 지원하며 PDF, MS Office 파일 및 이메일을 포함하여 문서 워크플로우 자동화에 이상적입니다.

############################# Steps ############################
steps:
    enable: true
    title: "PDF 문서에 데이터가 채워진 목록을 추가하는 단계"
    content: |
      [GroupDocs.Assembly](/assembly/net/)는 PDF 템플릿에 데이터 중심 목록을 삽입하는 과정을 간소화합니다. 목록을 만들고 사용자 정의하는 작업이 수월합니다.
      
      1. 목록을 위한 지정된 자리를 가진 템플릿을 만드세요 (현재 PDF 템플릿은 지원되지 않습니다).
      2. 템플릿에 대한 경로를 설정하세요.
      3. JSON 또는 XML과 같은 지원되는 출처에서 데이터를 가져오세요.
      4. 목록이 포함된 완료된 문서를 PDF 파일로 내보내세요.
   
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
        // 목록이 나타날 위치를 표시하기 위해 템플릿에 이 태그를 추가하세요
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // 템플릿 파일의 경로를 지정하세요
        // 현재 PDF 템플릿에 대한 지원이 제공되지 않습니다.
        string template = "list_template.docx";

        // 선택한 출처에서 데이터를 가져오세요
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 생성된 목록이 포함된 문서를 저장하세요
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "구조화된 데이터로 템플릿을 채워 문서 생성"
  description: "GroupDocs.Assembly for .NET은 데이터 중심 문서를 쉽게 구축하도록 합니다. 고급 템플릿을 사용하여 동적으로 목록, 표, 바코드, 차트, 이미지 및 기타 요소를 추가할 수 있습니다."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly 기능"
  features:
    # feature loop
    - title: "비즈니스 데이터를 기반으로 보고서 생성"
      content: "이 API는 JSON, XML, CSV 등과 같은 출처의 데이터를 사용하여 인기 있는 형식의 문서를 정확하고 효율적으로 채웁니다."

    # feature loop
    - title: "데이터를 표시하기 위해 목록 및 기타 요소 사용"
      content: "GroupDocs.Assembly를 사용하면 텍스트, 바코드, 하이퍼링크 및 이미지를 포함하여 목록, 표 및 차트를 삽입하여 잘 구조화된 문서를 만들 수 있습니다."

    # feature loop
    - title: "필요한 곳에 데이터를 정확히 삽입"
      content: "LINQ 기반 구문을 활용하여 목록 및 기타 데이터 요소를 정확히 배치하세요. 루프를 사용하여 목록을 동적으로 채우고 프로그래밍 방식으로 사용자 정의 형식을 적용할 수 있습니다."

    # feature loop
    - title: "다양한 문서 형식 지원"
      content: "MS Office, OpenOffice, PDF, HTML 및 이메일 파일과 같은 다양한 형식으로 문서를 생성하고 관리하세요. 여러 문서를 하나로 쉽게 통합할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "목록을 동적으로 생성하는 방법"
      content: |
        이 예제는 PDF 문서에 동적으로 생성된 목록을 삽입하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 목록을 위한 자리 표시자 태그를 템플릿에 추가하세요
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // 템플릿 파일의 경로를 지정하세요
          // 현재 PDF 템플릿에 대한 지원이 제공되지 않습니다.
          string template = "numlist_template.docx";

          // 목록을 채우기 위한 데이터를 가져오세요
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // 필요한 정보를 가진 데이터 소스 객체를 생성하세요
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // DocumentAssembler를 초기화하세요
          DocumentAssembler asm = new DocumentAssembler();

          // 생성된 목록이 포함된 최종 문서를 저장하세요
          asm.AssembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_list.pdf"
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
    title: "주요 기능 탐색"
    exclude: "list"
    description: "우리의 플랫폼은 데이터 기반 문서 내용을 쉽게 생성하고 통합할 수 있도록 설계되었습니다."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/net/barcode/pdf/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/net/chart/pdf/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/net/document/pdf/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/net/list/pdf/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/net/table/pdf/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "인기 형식으로 구조화된 문서 생성"
    exclude: "PDF"
    description: ".NET는 50개 이상의 형식을 지원하며, 데이터를 템플릿과 매끄럽게 병합하여 세련되고 구조화된 결과를 생성할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF에 목록 작성"
          format: "PDF"
          link: "/assembly/net/list/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 목록 작성"
          format: "DOCX"
          link: "/assembly/net/list/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 목록 작성"
          format: "PPTX"
          link: "/assembly/net/list/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 목록 작성"
          format: "XLSX"
          link: "/assembly/net/list/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---