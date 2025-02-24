



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:11
draft: false
lang: ko
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java를 사용하여 XLSX 문서에 테이블 추가하기"
head_description: "GroupDocs.Assembly for Java을(를) 사용하면 개발자가 동적 소스에서 데이터를 끌어와 문서와 이메일에 테이블을 신속하게 통합할 수 있습니다."

############################# Header ############################
title: "Java API로 XLSX 파일에 테이블을 채우기" 
description: "GroupDocs.Assembly for Java은(는) 다양한 입력 데이터로 XLSX 문서에 테이블을 채우는 과정을 간소화합니다."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 평가판 받기"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java란?"
    link: "/assembly/java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)은(는) 사전 설계된 템플릿에 데이터를 자동으로 삽입하여 문서와 보고서를 생성하는 도구입니다. 테이블, 리스트, 차트 및 이미지를 손쉽게 추가할 수 있습니다. 고급 기능을 통해 문서 내에서 콘텐츠를 정확하게 배치할 수 있습니다. PDF, MS Office 및 이메일 형식을 포함한 50개 이상의 파일 유형과 호환됩니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX 테이블에 데이터 삽입 단계"
    content: |
      [GroupDocs.Assembly](/assembly/java/)은(는) XLSX 및 기타 형식에 대한 테이블 템플릿을 채우는 데 도움을 줍니다. 소스의 동적 데이터를 사용하여 테이블을 생성하세요.
      
      1. XLSX 템플릿을 설정하고 테이블 행과 열에 대한 자리 표시자를 추가하세요.
      2. 지원되는 입력 소스에서 데이터를 끌어오세요.
      3. 필요에 맞게 데이터를 필터링하거나 전처리하세요.
      4. 완성된 테이블과 함께 최종 문서를 생성하세요.
   
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
        // 템플릿 내 테이블 행 자리 표시자에서 이러한 태그를 사용하세요
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>

        // 템플릿 파일의 경로를 정의하세요
        String template = "table_template.xlsx";

        // 선택한 소스에서 데이터를 로드하세요
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "ds");

        // 테이블이 채워진 출력 파일을 저장하세요
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "데이터가 채워진 테이블로 문서 생성하기"
  description: "GroupDocs.Assembly for Java은(는) 문서에서 테이블 생성을 자동화하는 것을 간편하게 만듭니다. 또한 템플릿을 사용하여 차트, 리스트 및 이미지를 추가하는 것도 지원합니다."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "여러 데이터 형식에서 보고서 생성하기"
      content: "이 API는 JSON, XML, CSV 및 기타 형식과 원활하게 작동하여 문서의 테이블에 구조화된 데이터를 채울 수 있게 합니다."

    # feature loop
    - title: "정보를 시각적으로 표현하기"
      content: "GroupDocs.Assembly은(는) 전문적인 테이블, 리스트 및 차트를 생성하며 링크, 텍스트 및 이미지를 삽입하여 매끄러운 외관을 제공합니다."

    # feature loop
    - title: "테이블 콘텐츠 정확하게 배치하기"
      content: "유연한 LINQ 기반 구문을 사용하여 동적으로 행과 열을 추가하세요. 프로그램적으로 글꼴 스타일과 색상을 사용자 정의할 수 있습니다."

    # feature loop
    - title: "여러 형식과 호환"
      content: "MS Office, OpenOffice, PDF, HTML 등 다양한 형식과 작업하십시오. 지원되는 파일 형식으로 테이블을 손쉽게 병합하세요."
      
  code_samples_ext:
    # code sample ext loop
    - title: "동적으로 데이터가 채워진 테이블 생성하기"
      content: |
        이 예제는 동적 입력 데이터를 사용해 XLSX 문서에서 테이블을 채우는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 테이블에 대한 자리 표시자가 포함된 템플릿을 설계하세요
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>

          // 템플릿 파일의 위치를 설정하세요
          String template = "table_template.xlsx";

          // 선호하는 소스에서 데이터 로드하기
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // 필요한 필드를 포함하는 데이터 객체를 준비하세요
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // DocumentAssembler의 인스턴스를 생성하세요
          DocumentAssembler asm = new DocumentAssembler();

          // 테이블이 채워진 문서를 저장하세요
          asm.assembleDocument(template, "result.xlsx", data);
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
            link: "/examples/assembly/formats/assembly_table.xlsx"
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
    title: "핵심 기능 요약"
    exclude: "table"
    description: "우리 API는 테이블 채우기를 자동화하여 전문 문서를 생성하는 과정을 간소화합니다."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/java/barcode/xlsx/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/java/chart/xlsx/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/java/document/xlsx/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/java/list/xlsx/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/java/table/xlsx/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식으로 상세한 테이블 생성하기"
    exclude: "XLSX"
    description: "Java을(를) 사용하면 데이터로 템플릿을 채우고 50개 이상의 파일 유형으로 상세한 보고서를 생성할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF에 표 추가"
          format: "PDF"
          link: "/assembly/java/table/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 표 추가"
          format: "DOCX"
          link: "/assembly/java/table/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 표 추가"
          format: "PPTX"
          link: "/assembly/java/table/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 표 추가"
          format: "XLSX"
          link: "/assembly/java/table/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---