



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:06
draft: false
lang: ko
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#로 PDF 파일에 차트 생성하기"
head_description: "GroupDocs.Assembly for .NET API는 개발자가 실시간 데이터를 사용하여 문서에 차트나 그래프를 동적으로 생성하고 삽입할 수 있게 합니다."

############################# Header ############################
title: ".NET API를 사용하여 PDF 파일에 차트 삽입하기" 
description: "GroupDocs.Assembly for .NET는 PDF 파일에 동적 데이터를 채워 넣고 차트를 원활하게 통합할 수 있는 강력한 방법을 제공합니다."
subtitle: "GroupDocs.Assembly for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험"
      link: "https://releases.groupdocs.com/assembly/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for .NET란?"
    link: "/assembly/net/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for .NET](/assembly/net/)는 여러 소스의 데이터를 통합하여 문서와 보고서를 생성하는 과정을 간소화하기 위해 설계된 도구입니다. 차트, 표, 리스트, 바코드 및 이미지를 동적으로 생성할 수 있습니다. 고급 형식 옵션을 통해 콘텐츠의 정확한 배치 및 사용자 정의가 가능합니다. PDF, MS Office 문서, 이메일을 포함한 50종 이상의 파일 형식을 지원합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PDF 문서에 차트 추가하기"
    content: |
      [GroupDocs.Assembly](/assembly/net/)는 PDF 템플릿에 차트를 생성하고 삽입하는 과정을 간소화합니다. 막대 차트, 원형 차트, 꺾은선 차트와 같은 다양한 차트 유형을 지원합니다.
      
      1. 차트를 위한 지정된 자리를 포함하여 템플릿을 설계하세요 (PDF 템플릿은 지원되지 않습니다).
      2. 호환되는 소스에서 데이터를 가져옵니다.
      3. 차트 옵션을 정의하세요: 유형, 레이블 및 색상 구성표.
      4. 차트를 포함한 문서를 PDF 파일로 내보내세요.
   
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
        // 차트를 생성하기 위해 템플릿에 이 태그를 포함하세요
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // 템플릿의 파일 경로를 지정하세요
        // 현재 PDF 템플릿은 지원되지 않습니다.
        string template = "chart_template.docx";

        // 선호하는 소스에서 데이터를 불러오세요
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // 차트가 포함된 문서를 저장하세요
        DocumentAssembler asm = new DocumentAssembler();
        asm.AssembleDocument(template, "result.pdf", data);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서에 동적 차트 추가하기"
  description: "GroupDocs.Assembly for .NET은 널리 사용되는 형식으로 데이터 기반 문서 생성을 간편하게 합니다. 템플릿을 사용하여 차트, 표, 바코드, 리스트, 하이퍼링크 및 이미지를 고급 동적 데이터 통합으로 삽입할 수 있습니다."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "데이터를 전문가 수준의 차트로 변환"
      content: "JSON, XML, CSV 등 다양한 소스에서 데이터를 가져와 몇 가지 단계만으로 시각적으로 매력적인 차트로 변환할 수 있습니다."

    # feature loop
    - title: "시각적으로 매력적인 콘텐츠 생성"
      content: "GroupDocs.Assembly은 막대 그래프, 원형 차트, 꺾은선 그래프와 같은 다양한 차트 유형을 지원하며, 이를 표, 바코드, 이미지 및 기타 요소와 결합하여 전문적인 보고서를 작성할 수 있습니다."

    # feature loop
    - title: "차트를 정확하게 배치하고 사용자 정의"
      content: "LINQ 구문을 사용하여 필요에 따라 차트를 동적으로 생성하고 배치할 수 있습니다. 스타일, 색상 및 레이아웃을 손쉽게 사용자 정의하여 요구 사항에 맞출 수 있습니다."

    # feature loop
    - title: "다양한 파일 형식과 호환"
      content: "MS Office, PDF, OpenOffice 및 HTML과 같은 인기 있는 형식으로 문서를 생성할 수 있습니다. 모든 지원되는 형식에 차트를 원활하게 삽입할 수 있는 완벽한 호환성을 제공합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "프로그래밍으로 차트 생성하기"
      content: |
        이 예제는 PDF 문서에 차트를 동적으로 생성하고 삽입하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 차트를 위한 자리 표시자를 가진 템플릿을 준비하세요
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // 템플릿 파일에 대한 경로를 제공하세요
          // 현재 PDF 템플릿은 지원되지 않습니다.
          string template = "table_template.docx";

          // 소스에서 데이터를 가져오세요
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 필요한 정보를 가진 데이터 객체를 작성하세요
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // 유형 및 외관과 같은 차트 속성을 설정하세요
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // DocumentAssembler 초기화
          DocumentAssembler asm = new DocumentAssembler();

          // 차트가 포함된 문서를 내보내기
          asm.AssembleDocument(template, "result.pdf", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pdf"
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
    title: "주요 기능 발견하기"
    exclude: "chart"
    description: "우리 플랫폼은 귀하의 요구에 맞춘 데이터 기반 문서를 작성하는 데 도움을 줍니다."
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
    title: "다양한 형식으로 시각적으로 풍부한 보고서 생성하기"
    exclude: "PDF"
    description: ".NET는 50개 이상의 지원 형식에서 차트가 통합된 문서를 생성할 수 있도록 하며, 템플릿과 데이터를 매끄럽게 결합합니다."
    items: 
          
        # format loop 1
        - name: "PDF의 차트"
          format: "PDF"
          link: "/assembly/net/chart/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX의 차트"
          format: "DOCX"
          link: "/assembly/net/chart/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX의 차트"
          format: "PPTX"
          link: "/assembly/net/chart/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX의 차트"
          format: "XLSX"
          link: "/assembly/net/chart/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---