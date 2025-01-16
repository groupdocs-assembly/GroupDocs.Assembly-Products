



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:03
draft: false
lang: ko
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript로 PPTX에서 동적 목록 생성하기"
head_description: "GroupDocs.Assembly for Node.js via Java API를 사용해 PPTX 템플릿에 목록을 디자인하고 삽입하는 과정을 간소화합니다."

############################# Header ############################
title: "Node.js로 PPTX 파일에 데이터 기반 목록 삽입하기" 
description: "GroupDocs.Assembly for Node.js via Java는 PPTX 문서에 유연하며 데이터 중심의 목록을 추가할 수 있는 강력한 도구를 제공합니다."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료로 시작하기"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java 소개"
    link: "/assembly/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)는 다양한 소스에서 데이터를 불러와 템플릿에 내장하여 문서 생성 과정을 단순화합니다. 목록, 표, 차트 및 기타 요소를 정확한 위치와 서식 옵션으로 구축할 수 있습니다. PDF, MS Office, 이메일 등 50개 이상의 형식을 지원하여 문서 생성 프로세스를 자동화합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 파일에 목록을 삽입하는 단계"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)을 사용하면 PPTX 템플릿에 세부적이고 데이터 기반 목록을 추가하는 과정이 간편합니다.
      
      1. PPTX 템플릿을 생성하고 목록에 대한 자리 표시자를 정의합니다.
      2. 템플릿의 파일 경로를 제공합니다.
      3. JSON 또는 XML과 같은 지원되는 소스에서 데이터를 로드합니다.
      4. 생성된 목록과 함께 문서를 저장합니다.
   
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
        // 템플릿에 이 태그를 배치하여 목록이 들어갈 위치를 표시합니다.
        // <<foreach [in customers]>><<[CustomerName]>><</foreach>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 템플릿의 파일 경로를 설정하세요.
        const template = "list_template.pptx";

        // 사용하려는 소스에서 데이터를 가져옵니다.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // 내장 목록과 함께 파일을 저장합니다.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "통합 데이터로 문서 생성하기"
  description: "GroupDocs.Assembly for Node.js via Java를 사용하면 목록, 표, 차트 및 기타 요소를 템플릿에 삽입하여 시간과 노력을 절약할 수 있습니다."
  image: "/img/assembly/features_list.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "다양한 데이터 소스로부터 보고서 생성"
      content: "JSON, XML, CSV 등에서 데이터를 가져와 목록 및 기타 요소를 효율적으로 채울 수 있습니다."

    # feature loop
    - title: "목록 및 기타 시각적 요소 추가"
      content: "GroupDocs.Assembly를 사용하면 텍스트, 이미지 및 링크와 함께 목록, 표, 차트를 매끄럽게 삽입할 수 있어 품질 높은 결과를 얻을 수 있습니다."

    # feature loop
    - title: "데이터의 위치와 스타일을 정밀하게 조정"
      content: "LINQ 기반 템플릿을 통해 목록 및 기타 데이터의 위치를 정확히 제어하고 반복 항목을 위한 루프를 사용하며 스타일을 맞춤 설정할 수 있습니다."

    # feature loop
    - title: "다양한 형식에서 작동"
      content: "MS Office, PDF, OpenOffice, HTML 및 이메일 등 다양한 형식으로 문서를 생성할 수 있으며, 여러 소스의 내용을 하나의 파일로 통합할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서 내에서 목록을 프로그래밍 방식으로 생성하기"
      content: |
        이 예제는 GroupDocs.Assembly를 사용하여 PPTX 문서에 동적으로 목록을 추가하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 템플릿에 목록용 자리 표시자를 추가합니다.
          // <<foreach [in products]>><<[NumberOf()]>>. <<[ProductName]>>
          // <</foreach>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 템플릿의 파일 경로를 지정합니다.
          const template = "numlist_template.pptx";

          // 목록을 채울 데이터를 로드합니다.
          const data_xml =
              new assemblyLib.XmlDataSource("products.xml");

          // 필요한 세부정보로 데이터 소스를 준비합니다.
          const data 
              = new assemblyLib.DataSourceInfo(data_xml, "products");

          // DocumentAssembler를 초기화합니다.
          const asm = new assemblyLib.DocumentAssembler();

          // 목록이 포함된 최종 문서를 저장합니다.
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
            link: "/examples/assembly/formats/assembly_list.pptx"
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
    title: "GroupDocs.Assembly의 기능 탐색하기"
    exclude: "list"
    description: "강력한 통합 도구를 사용하여 데이터가 풍부한 문서를 간편하게 디자인하고 생성하세요."
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
    title: "다양한 형식으로 문서 생성하기"
    exclude: "PPTX"
    description: "Node.js via Java는 50개 이상의 파일 형식을 지원하여 템플릿과 데이터를 통합하여 전문적인 결과를 쉽게 만들어 냅니다."
    items: 
          
        # format loop 1
        - name: "PDF에 목록 작성"
          format: "PDF"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 목록 작성"
          format: "DOCX"
          link: "/assembly/nodejs-java/list/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 목록 작성"
          format: "PPTX"
          link: "/assembly/nodejs-java/list/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 목록 작성"
          format: "XLSX"
          link: "/assembly/nodejs-java/list/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---