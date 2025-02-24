



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:08
draft: false
lang: ko
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript로 DOCX 파일 병합하기"
head_description: "JavaScript를 사용하여 DOCX 파일을 간편하게 결합하세요. GroupDocs.Assembly는 문서 병합을 몇 가지 간단한 단계로 효율적으로 처리합니다."

############################# Header ############################
title: "DOCX 파일의 내용을 손쉽게 결합하기" 
description: "GroupDocs.Assembly for Node.js via Java을 사용하면 하나의 DOCX 파일을 다른 파일에 신속하고 정확하게 통합할 수 있습니다. 매끄러운 병합을 위한 유연하고 신뢰할 수 있는 도구를 즐기세요."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험하기"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java 개요"
    link: "/assembly/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)는 문서 관리를 위한 강력한 방법을 제공합니다. PDF 및 MS Office와 같은 50개 이상의 형식을 지원하며, 하나의 파일을 다른 파일에 결합하는 과정이 간편합니다. 레이아웃을 사용자 정의하고, 내용을 편집하며, 문서를 필요한 대로 정확하게 조직하세요.

############################# Steps ############################
steps:
    enable: true
    title: "DOCX 파일에 문서 병합하기"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)은 커스터마이즈 가능한 옵션으로 하나의 DOCX 파일을 다른 파일에 삽입하는 과정을 간소화합니다.
      
      1. DOCX 템플릿을 콘텐츠에 대한 플레이스홀더와 함께 디자인합니다.
      2. 템플릿에 대한 파일 경로를 설정합니다.
      3. 병합할 문서의 파일 경로를 제공합니다.
      4. 결합된 콘텐츠로 최종 파일을 내보냅니다.
   
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
        // 템플릿에 이 태그를 삽입하여 문서가 삽입될 위치를 정의합니다.
        // <<doc [doc_expression]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 주 템플릿의 파일 경로를 설정합니다.
        const template = "doc_template.docx";

        // 병합할 문서의 경로를 제공하세요.
        const data 
            = new assemblyLib.DataSourceInfo("insert.docx", "doc_expression");

        // 삽입된 문서와 함께 최종 출력을 저장합니다.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "문서 통합을 위한 강력한 도구"
  description: "GroupDocs.Assembly for Node.js via Java은 다양한 형식 간 파일 삽입을 쉽고 완전히 사용자 정의할 수 있도록 합니다. 매번 일관되고 전문적인 결과를 제공합니다."
  image: "/img/assembly/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "비즈니스 데이터로 보고서 생성"
      content: "JSON, XML 또는 CSV 소스에서 데이터를 추출하여 신속하고 정확하게 포괄적인 보고서와 문서를 작성할 수 있습니다."

    # feature loop
    - title: "풍부한 시각적 요소 추가"
      content: "GroupDocs.Assembly를 사용하면 테이블, 차트, 목록, 이미지 및 바코드를 텍스트와 하이퍼링크와 함께 포함할 수 있습니다."

    # feature loop
    - title: "정확한 데이터 배치"
      content: "LINQ 템플릿을 사용하여 데이터를 정확한 위치에 배치하고, 배열과 같은 반복 항목을 처리하며, 스타일을 간편하게 사용자 정의하세요."

    # feature loop
    - title: "다양한 형식 지원"
      content: "PDF, MS Office 파일, HTML, OpenOffice와 같은 형식 간 콘텐츠를 매끄럽게 병합하여 모든 프로젝트에 유연성을 제공합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "프로그램을 통해 문서에 이미지 삽입하기"
      content: |
        이 예제는 GroupDocs.Assembly를 사용하여 DOCX 파일에 이미지를 삽입하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 이미지를 위한 템플릿에 플레이스홀더를 추가합니다.
          // <<image [expression]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 템플릿 파일의 경로를 지정합니다.
          const template = "template.docx";

          // 삽입할 이미지의 경로를 설정합니다.
          const data =
              = new assemblyLib.DataSourceInfo("logo.jpg", "expression");

          // DocumentAssembler 객체를 초기화합니다.
          const asm = new assemblyLib.DocumentAssembler();

          // 이미지가 포함된 문서를 저장합니다.
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_document.docx"
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
    title: "핵심 기능 개요"
    exclude: "document"
    description: "GroupDocs.Assembly이 제공하는 효율적이고 원활한 문서 병합을 위한 종합 도구를 탐색하세요."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "여러 형식의 문서 결합"
    exclude: "DOCX"
    description: "Node.js via Java을 사용하여 50개 이상의 파일 형식 간 콘텐츠를 병합하여 전문적이고 세련된 결과를 보장하세요."
    items: 
          
        # format loop 1
        - name: "PDF에 문서 삽입"
          format: "PDF"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 문서 삽입"
          format: "DOCX"
          link: "/assembly/nodejs-java/document/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 문서 삽입"
          format: "PPTX"
          link: "/assembly/nodejs-java/document/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 문서 삽입"
          format: "XLSX"
          link: "/assembly/nodejs-java/document/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---