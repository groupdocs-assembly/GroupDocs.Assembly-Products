



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: ko
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#를 사용하여 DOCX 문서에 표 만들기"
head_description: "GroupDocs.Assembly for .NET API를 통해 개발자는 동적 소스의 데이터를 사용하여 문서와 이메일에 표를 간편하게 추가하고 채울 수 있습니다."

############################# Header ############################
title: "우리의 .NET API를 사용하여 DOCX 문서에서 데이터 표 생성" 
description: "GroupDocs.Assembly for .NET는 다양한 소스에서 데이터로 DOCX 문서의 표를 동적으로 채우는 작업을 간소화합니다."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 평가판 다운로드"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET 개요"
    link: "/assembly/net/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)는 여러 출처의 데이터를 사용하여 문서 및 보고서를 생성하기 위해 설계되었습니다. 표, 목록 및 차트에 구조화된 데이터를 간편하게 삽입하거나 이미지를 동적으로 포함할 수 있습니다. 고급 문법을 통해 정확한 데이터 배치가 가능합니다. PDFs, MS Office 문서 및 이메일 파일을 포함한 50개 이상의 형식을 지원합니다.

############################# Steps ############################
steps:
    enable: true
    title: "DOCX 문서에 표를 채우는 방법"
    content: |
      [GroupDocs.Assembly](/assembly/net/)을 사용하면 DOCX와 같은 형식의 템플릿에 표를 동적으로 채울 수 있습니다. 다양한 소스에서 데이터를 표에 삽입하세요.
      
      1. DOCX 템플릿을 생성하고 표 자리 표시자를 추가합니다.
      2. 지원되는 소스에서 데이터를 가져옵니다.
      3. 필요한 정보만 포함되도록 데이터를 필터링합니다.
      4. 채워진 표와 함께 문서를 저장합니다.
   
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
        // 템플릿 테이블 행에 이 태그들을 추가하세요
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // 템플릿의 파일 경로를 설정하세요
        string template = "table_template.docx";

        // 지원되는 소스에서 데이터를 가져오세요
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // 데이터로 채워진 표와 함께 문서를 저장하세요
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.docx", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "동적 표로 문서 생성"
  description: "GroupDocs.Assembly for .NET는 문서 생성을 간소화하여 문서의 표를 자동으로 채우고, 템플릿과 고급 마크업을 통해 차트, 목록 및 이미지와 같은 추가 요소를 지원합니다."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "구조적 데이터로 보고서 생성"
      content: "API는 JSON, XML, CSV와 같은 소스의 데이터를 처리하여 오피스 문서의 표를 효과적이고 정확하게 채울 수 있습니다."

    # feature loop
    - title: "데이터를 시각적으로 표시"
      content: "GroupDocs.Assembly는 전문적인 문서 디자인을 위해 표, 목록 및 차트를 생성하고 텍스트, 링크 및 이미지를 포함하는 기능을 제공합니다."

    # feature loop
    - title: "표 데이터의 정확한 위치 지정"
      content: "LINQ 기반 문법을 사용하여 테이블 행과 열을 동적으로 추가합니다. 스타일, 색상 및 형식을 프로그래밍적으로 사용자 정의할 수 있습니다."

    # feature loop
    - title: "다양한 형식 지원"
      content: "MS Office, OpenOffice, PDF 및 HTML과 같은 인기 있는 파일 형식을 문제없이 처리할 수 있습니다. 지원되는 문서 형식에 채워진 표를 원활하게 포함할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "데이터 표를 동적으로 채우는 방법"
      content: |
        이 예제는 동적 데이터를 사용하여 DOCX 문서의 표를 채우는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 표를 위한 자리 표시자가 있는 템플릿을 준비합니다
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          // <<[c.Price]>> <</foreach>>

          // 템플릿의 파일 경로를 지정합니다
          string template = "table_template.docx";

          // 선택한 소스에서 데이터를 조회합니다
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 필요한 데이터를 가진 데이터 소스 개체를 생성합니다
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // DocumentAssembler 초기화
          DocumentAssembler asm = new DocumentAssembler();

          // 채워진 표가 포함된 완료된 문서를 저장합니다
          asm.AssembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_table.docx"
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
    exclude: "table"
    description: "우리 솔루션은 동적으로 채워진 표와 추가 요소가 포함된 전문 문서를 간편하게 생성할 수 있도록 돕습니다."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/net/barcode/docx/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/net/chart/docx/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/net/document/docx/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/net/list/docx/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/net/table/docx/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "상세한 표로 보고서 생성"
    exclude: "DOCX"
    description: ".NET는 50개 이상의 지원 형식에서 테이블과 기타 데이터 요소로 템플릿을 채워 포괄적인 보고서를 생성할 수 있게 해줍니다."
    items: 
          
        # format loop 1
        - name: "PDF에 표 추가"
          format: "PDF"
          link: "/assembly/net/table/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 표 추가"
          format: "DOCX"
          link: "/assembly/net/table/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 표 추가"
          format: "PPTX"
          link: "/assembly/net/table/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 표 추가"
          format: "XLSX"
          link: "/assembly/net/table/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---