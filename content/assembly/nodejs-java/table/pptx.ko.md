



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:12
draft: false
lang: ko
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript을 사용하여 PPTX 문서에 테이블 삽입하기"
head_description: "GroupDocs.Assembly for Node.js via Java를 사용하여 다양한 출처에서 데이터를 가져와 문서나 이메일에 테이블을 빠르게 삽입하세요."

############################# Header ############################
title: "Node.js에서 PPTX 파일에 테이블 추가하기" 
description: "GroupDocs.Assembly for Node.js via Java을 사용하면 여러 출처의 데이터를 이용해 PPTX 문서에 테이블을 쉽게 채울 수 있습니다."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험 시작하기"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java 소개"
    link: "/assembly/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)는 문서 생성 자동화를 위한 강력한 도구입니다. 테이블, 차트, 리스트, 이미지를 템플릿에 정밀하게 삽입할 수 있습니다. PDF, Word, 이메일을 포함해 50개 이상의 파일 형식을 지원하며, 보고서 생성 및 기타 작업을 간소화합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX에서 테이블에 데이터 추가하기"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)은 동적 데이터 소스를 사용하여 PPTX 파일의 테이블 템플릿을 빠르게 채울 수 있도록 합니다.
      
      1. PPTX 템플릿을 생성하고 테이블 행 및 열을 위한 자리 표시자를 추가합니다.
      2. JSON 또는 CSV와 같은 지원되는 출처에서 데이터를 로드합니다.
      3. 필요에 따라 데이터를 정리하고 형식을 지정합니다.
      4. 완성된 테이블이 포함된 문서를 생성합니다.
   
    code:
      platform: "java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "예제 문서"
      install:
        command: "npm i @groupdocs/groupdocs.assembly"
        copy_tip: "복사하려면 클릭"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        // 템플릿의 테이블 행 자리 표시자에 이러한 태그를 포함하세요.
        // <<foreach [c in ds]>>
        // <<[c.Client]>><<[c.Manager]>><<[c.Price]>>
        // <</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 템플릿 파일 경로를 지정하세요.
        const template = "table_template.pptx";

        // 선택한 출처에서 데이터를 로드하세요.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "ds");

        // 완성된 테이블이 포함된 최종 문서를 저장하세요.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "데이터 기반 테이블을 문서에 추가하기"
  description: "GroupDocs.Assembly for Node.js via Java을 통해 사용자는 테이블을 자동으로 생성할 수 있을 뿐만 아니라, 템플릿 기반 워크플로우를 사용하여 차트, 이미지 및 리스트를 삽입할 수 있습니다."
  image: "/img/assembly/features_table.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "구조화된 데이터로부터 테이블 생성"
      content: "JSON, XML, CSV 등 다양한 형식에서 데이터를 가져와 문서 테이블을 자동으로 채울 수 있습니다."

    # feature loop
    - title: "세련된 시각적 콘텐츠 생성"
      content: "GroupDocs.Assembly을 사용하여 전문적인 테이블, 차트 및 리스트를 디자인하고, 링크, 이미지 및 텍스트를 추가하여 다듬어진 문서의 외관을 제공합니다."

    # feature loop
    - title: "동적 테이블 내용 배치"
      content: "LINQ 기반 템플릿을 사용하여 프로그래밍적으로 행과 열을 추가하고, 글꼴, 색상 및 정렬과 같은 스타일을 사용자 정의할 수 있습니다."

    # feature loop
    - title: "다양한 형식에서 원활하게 작동"
      content: "MS Office, OpenOffice, PDF, HTML 등에서 테이블을 쉽게 생성하거나 편집하고, 필요에 따라 파일에 병합할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "프로그램적으로 테이블 채우기"
      content: |
        이 예시는 외부 출처의 데이터를 사용하여 PPTX 문서의 테이블을 채우는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 테이블을 위한 자리 표시자가 포함된 템플릿을 디자인합니다.
          // <<foreach [c in items]>> <<[c.Client]>><<[c.Manager]>>
          //  <<[c.Price]>> <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 템플릿의 파일 경로를 지정합니다.
          const template = "table_template.pptx";

          // 필요한 데이터를 출처에서 로드합니다.
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // 데이터를 필요한 구조로 구성합니다.
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // DocumentAssembler 초기화하기.
          const asm = new assemblyLib.DocumentAssembler();

          // 완성된 테이블이 포함된 출력 문서를 저장합니다.
          asm.assembleDocument(template, "result.pptx", data);
          ```
        platform: "java"
        copy_title: "복사"
        install:
          command: "npm i @groupdocs/groupdocs.assembly"
          copy_tip: "복사하려면 클릭"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/assembly/formats/assembly_table.pptx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Assembly의 기능을 무료로 탐색하거나 라이센스를 요청하세요"
  items:
    #  loop
    - title: "NPM에서 다운로드"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "라이센스에 대해 알아보세요"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "핵심 기능 한눈에 보기"
    exclude: "table"
    description: "우리의 API는 테이블 생성 자동화 및 다양화된 도구와 템플릿으로 문서 생성을 향상합니다."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식으로 테이블 생성하기"
    exclude: "PPTX"
    description: "Node.js via Java을 사용하여 템플릿을 채우고 50개 이상의 지원되는 파일 형식에서 포괄적인 테이블을 생성합니다."
    items: 
          
        # format loop 1
        - name: "PDF에 표 추가"
          format: "PDF"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 표 추가"
          format: "DOCX"
          link: "/assembly/nodejs-java/table/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 표 추가"
          format: "PPTX"
          link: "/assembly/nodejs-java/table/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 표 추가"
          format: "XLSX"
          link: "/assembly/nodejs-java/table/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---