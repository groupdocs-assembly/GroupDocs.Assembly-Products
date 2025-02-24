



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:09
draft: false
lang: ko
format: Xlsx
product: "Assembly"
product_tag: "assembly"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java로 XLSX 문서에서 목록 만들기"
head_description: "GroupDocs.Assembly for Java API를 사용하여 XLSX 템플릿에 동적 목록을 설계하고 삽입할 수 있습니다."

############################# Header ############################
title: "우리의 Java API로 XLSX 파일에 동적 목록 추가하기" 
description: "GroupDocs.Assembly for Java는 XLSX 문서에 데이터가 풍부한 목록을 생성하고 직접 삽입할 수 있는 유연한 도구를 제공합니다."
subtitle: "GroupDocs.Assembly for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험하기"
      link: "https://releases.groupdocs.com/assembly/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Java란?"
    link: "/assembly/java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Java](/assembly/java/)는 여러 출처로부터 데이터를 끌어와 전문적인 문서를 설계할 수 있게 해 줍니다. 목록, 표, 차트, 텍스트 등을 생성하고 이러한 요소들을 고급 템플릿 기능을 사용하여 필요한 위치에 배치할 수 있습니다. 50개 이상의 형식을 지원하며 PDF, MS Office 파일 및 이메일 문서가 포함되어 있어 워크플로우를 자동화하고 간소화하는 데 도움을 줍니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX 문서에 데이터 기반 목록 추가 방법"
    content: |
      [GroupDocs.Assembly](/assembly/java/)를 사용하면 XLSX 템플릿에 데이터가 풍부한 목록을 신속하게 삽입할 수 있습니다. 콘텐츠를 손쉽게 커스터마이즈하고 정리하세요.
      
      1. XLSX 템플릿을 만들고 목록에 대한 자리 표시자를 표시합니다.
      2. 템플릿에 대한 파일 경로를 설정합니다.
      3. JSON 또는 XML과 같은 지원 형식에서 데이터를 가져옵니다.
      4. 목록이 추가된 최종 문서를 저장합니다.
   
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
        // 목록이 나타나는 곳에 이 태그를 템플릿에 포함시킵니다.
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>

        // 템플릿의 파일 경로를 정의합니다.
        String template = "list_template.xlsx";

        // 선택한 소스에서 데이터를 가져옵니다.
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // 목록이 포함된 문서를 저장합니다.
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.xlsx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "데이터 통합으로 템플릿에서 문서 생성하기"
  description: "GroupDocs.Assembly for Java는 동적 목록, 표, 차트 및 기타 요소를 문서 템플릿에 쉽게 추가할 수 있도록 합니다."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 핵심 기능"
  features:
    # feature loop
    - title: "다양한 출처의 데이터를 사용하여 보고서 구축"
      content: "JSON, XML 및 CSV와 같은 형식의 데이터를 사용하여 목록 및 다른 구성 요소를 효율적으로 채울 수 있습니다."

    # feature loop
    - title: "목록 및 기타 데이터 요소를 원활하게 추가"
      content: "GroupDocs.Assembly는 텍스트, 이미지 및 링크 옆에 목록, 차트, 표 등을 통합하여 단정한 문서를 만들 수 있도록 지원합니다."

    # feature loop
    - title: "데이터가 나타나는 위치를 정확하게 제어"
      content: "LINQ 기반 템플릿을 사용하면 목록과 데이터의 정확한 위치를 정의할 수 있습니다. 루프를 사용하여 세부 목록을 자동으로 생성하고 사용자 지정 형식을 적용할 수 있습니다."

    # feature loop
    - title: "다양한 문서 형식 지원"
      content: "MS Office, PDF, OpenOffice, HTML 및 이메일 형식으로 파일을 생성하거나 편집할 수 있습니다. 필요에 따라 여러 문서의 내용을 병합할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "프로그래밍 방식으로 목록 생성하기"
      content: |
        이 예제는 GroupDocs.Assembly를 사용하여 XLSX 파일에 목록을 동적으로 추가하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 목록을 위한 자리 표시자 태그를 템플릿에 추가합니다.
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>

          // 템플릿에 대한 파일 경로를 제공합니다.
          String template = "numlist_template.xlsx";

          // 목록을 채우기 위한 필요한 데이터를 가져옵니다.
          XmlDataSource data_xml =
              new XmlDataSource("products.xml");

          // 필요한 세부 정보로 데이터 소스를 준비합니다.
          DataSourceInfo data 
              = new DataSourceInfo(data_xml, "products");

          // DocumentAssembler 초기화
          DocumentAssembler asm = new DocumentAssembler();

          // 완료된 목록과 함께 출력 문서를 저장합니다.
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
            link: "/examples/assembly/formats/assembly_list.xlsx"
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
    title: "GroupDocs.Assembly의 기능 알아보기"
    exclude: "list"
    description: "고급 데이터 통합 도구를 사용하여 콘텐츠가 풍부한 문서를 간편하게 설계하고 생성하세요."
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
    title: "다양한 형식의 문서 생성"
    exclude: "XLSX"
    description: "Java는 50개 이상의 형식을 지원하며, 데이터를 템플릿과 결합하여 구조화된 문서를 생성할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF에 목록 작성"
          format: "PDF"
          link: "/assembly/java/list/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 목록 작성"
          format: "DOCX"
          link: "/assembly/java/list/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 목록 작성"
          format: "PPTX"
          link: "/assembly/java/list/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 목록 작성"
          format: "XLSX"
          link: "/assembly/java/list/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---