



---
############################# Static ############################
layout: "format"
date:  2024-12-13T10:30:53
draft: false
lang: ko
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java를 사용하여 PPTX 문서에 차트 생성하기"
head_description: "GroupDocs.Assembly for Java API는 개발자가 문서에 동적 차트나 그래프를 라이브 데이터로 원활하게 생성하고 삽입할 수 있도록 합니다."

############################# Header ############################
title: "Java API로 PPTX 문서에 차트 추가하기" 
description: "GroupDocs.Assembly for Java은 실시간 데이터를 활용하여 PPTX 문서에 차트를 통합하는 과정을 간소화합니다."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료로 시작하기"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java 소개"
    link: "/assembly/java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)는 문서 및 보고서 생성을 자동화하기 위한 다목적 솔루션입니다. 차트, 테이블, 목록, 바코드 및 이미지를 파일에 직접 추가할 수 있으며, 정밀한 형식 지정 및 데이터 통합을 위한 고급 도구를 제공합니다. 이 플랫폼은 PDF, Microsoft Office 파일 및 이메일 등 50개 이상의 형식을 지원합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 문서에 차트를 삽입하는 단계"
    content: |
      [GroupDocs.Assembly](/assembly/java/)은 PPTX 템플릿에 차트를 삽입하는 과정을 간소화합니다. 바, 파이 및 선 그래프 등 다양한 차트 스타일 중에서 선택하십시오.
      
      1. PPTX 템플릿을 생성하되 차트를 위한 자리 표시자를 포함합니다.
      2. 호환 가능한 출처에서 데이터를 로드합니다.
      3. 차트 옵션(유형, 레이블, 색상 등)을 설정합니다.
      4. 차트가 포함된 문서를 저장합니다.
   
    code:
      platform: "java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "예제 문서"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-assembly</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "복사하려면 클릭"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/assembly/java/"
          
      content: |
        ```java {style=abap}
        // 차트를 포함하려면 템플릿에 이 태그를 추가하세요.
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // 템플릿의 파일 경로를 제공합니다.
        String template = "chart_template.pptx";

        // 소스에서 필요한 데이터를 추출합니다.
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // 차트가 포함된 최종 문서를 저장합니다.
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "문서에 동적 차트를 손쉽게 삽입하기"
  description: "GroupDocs.Assembly for Java은 인기 있는 형식으로 데이터가 풍부한 문서를 구축하는 간편한 방법을 제공합니다. 템플릿을 사용하여 차트, 테이블, 바코드, 목록, 링크 및 이미지를 데이터의 동적 업데이트와 함께 삽입할 수 있습니다."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "데이터를 차트로 변환"
      content: "API를 사용하여 JSON, XML, CSV 또는 기타 출처의 데이터를 문서용으로 깔끔하고 전문적인 차트로 변환합니다."

    # feature loop
    - title: "시각적으로 임팩트 있는 콘텐츠 생성"
      content: "GroupDocs.Assembly은 바 그래프, 파이 차트, 선 그래프 등 다양한 시각적 형식을 지원하며, 테이블, 바코드, 이미지와 결합하여 향상된 보고서를 제공합니다."

    # feature loop
    - title: "차트 배치 및 스타일 사용자 정의"
      content: "LINQ 기반의 문법을 통해 문서 내에서 동적으로 차트를 생성하고 배치할 수 있으며, 디자인 요구에 맞게 스타일, 색상 및 레이아웃을 쉽게 조정할 수 있습니다."

    # feature loop
    - title: "다양한 문서 형식 지원"
      content: "MS Office, PDF, OpenOffice, HTML 등의 형식으로 문서를 생성하십시오. 차트는 모든 지원 형식에 원활하게 통합되어 전문적인 결과를 제공합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "프로그래밍적으로 차트를 생성하고 삽입하기"
      content: |
        이 예제에서는 차트를 PPTX 문서에 프로그램matically 생성하고 삽입하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 차트를 위한 자리 표시자가 있는 템플릿을 준비합니다.
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // 템플릿의 파일 경로를 지정합니다.
          String template = "table_template.pptx";

          // 선택한 출처에서 데이터를 로드합니다.
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 관련 정보를 포함한 데이터 개체를 생성합니다.
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // 차트의 유형 및 모양을 구성합니다.
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // DocumentAssembler 초기화합니다.
          DocumentAssembler asm = new DocumentAssembler();

          // 차트가 삽입된 완료된 문서를 저장합니다.
          asm.assembleDocument(template, "result.pptx", data, design);
          ```
        platform: "java"
        copy_title: "복사"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-assembly</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "복사하려면 클릭"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.pptx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/assembly/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Assembly의 기능을 무료로 탐색하거나 라이센스를 요청하세요"
  items:
    #  loop
    - title: "Maven에서 다운로드"
      link: "https://releases.groupdocs.com/assembly/java/"
      color: "red"
        #  loop
    - title: "라이센스에 대해 알아보세요"
      link: "https://purchase.groupdocs.com/pricing/assembly/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "강력한 기능 탐색"
    exclude: "chart"
    description: "이 플랫폼은 데이터 중심의 시각적으로 매력적인 문서를 설계하는 과정을 간소화합니다."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/java/barcode/pptx/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/java/chart/pptx/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/java/document/pptx/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/java/list/pptx/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/java/table/pptx/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식으로 포괄적인 보고서 생성"
    exclude: "PPTX"
    description: "Java는 50개 이상의 파일 형식에 걸쳐 통합된 차트가 포함된 문서를 생성할 수 있도록 하여 템플릿과 데이터의 원활한 병합을 보장합니다."
    items: 
          
        # format loop 1
        - name: "PDF의 차트"
          format: "PDF"
          link: "/assembly/java/chart/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX의 차트"
          format: "DOCX"
          link: "/assembly/java/chart/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX의 차트"
          format: "PPTX"
          link: "/assembly/java/chart/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX의 차트"
          format: "XLSX"
          link: "/assembly/java/chart/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---