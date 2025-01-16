



---
############################# Static ############################
layout: "format"
date:  2025-01-16T13:04:00
draft: false
lang: ko
format: Pptx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript를 사용하여 PPTX 파일에 차트 삽입하기"
head_description: "GroupDocs.Assembly for Node.js via Java를 사용하면 개발자가 실시간 데이터 소스를 통해 문서에 동적 차트를 신속하게 생성하고 삽입할 수 있습니다."

############################# Header ############################
title: "Node.js를 사용하여 PPTX 파일에 차트 추가하기" 
description: "GroupDocs.Assembly for Node.js via Java는 실시간 데이터 입력으로 PPTX 문서에 차트를 통합하는 과정을 간소화합니다."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "지금 무료 시작하기"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java 개요"
    link: "/assembly/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)는 자동화된 문서 및 보고서를 생성하기 위한 강력한 솔루션입니다. 차트, 테이블, 이미지, 바코드 및 목록을 파일에 정밀하게 추가할 수 있습니다. 이 다목적 플랫폼은 PDF, Office 문서 및 이메일을 포함하여 50개 이상의 파일 형식을 지원합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 문서에 차트를 추가하는 단계"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)는 PPTX 파일에 차트를 추가하는 과정을 단순화합니다. 막대 차트, 선 차트 또는 파이 차트와 같은 차트 유형 중에서 선택하세요.
      
      1. PPTX 템플릿을 디자인하고 차트의 자리 표시자를 추가합니다.
      2. 지원되는 소스에서 데이터를 로드합니다.
      3. 차트 유형, 색상 및 레이블을 포함하여 차트 옵션을 구성합니다.
      4. 내장된 차트가 있는 문서를 내보냅니다.
   
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
        // 차트를 생성하기 위해 템플릿에 이 태그를 포함합니다.
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 템플릿 파일 경로를 지정합니다.
        const template = "chart_template.pptx";

        // 소스 시스템에서 데이터를 추출합니다.
        const data 
            = new assemblyLib.DataSourceInfo(GetChartData(), "orders");

        // 차트가 포함된 최종 문서를 저장합니다.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pptx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "문서에 차트를 손쉽게 삽입하기"
  description: "GroupDocs.Assembly for Node.js via Java는 인기 있는 파일 형식으로 기능이 풍부한 문서를 생성하는 것을 간편하게 해줍니다. 템플릿을 사용하여 차트, 테이블, 바코드, 목록, 이미지 등을 실시간 데이터 업데이트와 함께 추가하세요."
  image: "/img/assembly/features_chart.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 주요 기능"
  features:
    # feature loop
    - title: "데이터를 전문적인 차트로 변환하기"
      content: "JSON, XML 또는 CSV와 같은 소스의 데이터를 고품질 차트로 변환하여 문서에 직접 삽입할 수 있습니다."

    # feature loop
    - title: "눈에 띄는 시각 자료 생성하기"
      content: "다른 문서 요소(이미지, 테이블 및 바코드 등)와 원활하게 작동하는 막대 차트, 파이 그래프 및 선 차트를 생성합니다."

    # feature loop
    - title: "유연한 차트 스타일링 및 배치"
      content: "LINQ 템플릿을 사용하여 차트 위치 및 스타일을 제어할 수 있으며, 색상, 레이아웃 및 레이블을 설정하여 세련된 프레젠테이션을 구현합니다."

    # feature loop
    - title: "다양한 파일 형식 지원"
      content: "MS Office, PDF, OpenOffice 및 HTML 형식으로 문서를 생성할 수 있으며, 차트가 완벽하게 통합되어 전문적인 마무리를 제공합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "차트를 동적으로 생성하고 삽입하기"
      content: |
        이 예제는 PPTX 파일에 차트를 프로그래밍 방식으로 생성하고 삽입하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 차트의 자리 표시자를 포함한 템플릿을 설정합니다.
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 템플릿 파일 경로를 정의합니다.
          const template = "table_template.pptx";

          // 선택한 소스에서 데이터를 가져옵니다.
          const data_json = 
            new assemblyLib.JsonDataSource("Items.json");

          // 차트 정보를 포함한 데이터 객체를 준비합니다.
          const data 
              = new assemblyLib.DataSourceInfo(data_json, "items");

          // 차트 유형을 선택하고 외관을 사용자 정의합니다.
          const design 
              = new assemblyLib.DataSourceInfo("red", "color");

          // DocumentAssembler를 초기화합니다.
          const asm = new assemblyLib.DocumentAssembler();

          // 차트가 내장된 업데이트된 문서를 저장합니다.
          asm.assembleDocument(template, "result.pptx", data, design);
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
            link: "/examples/assembly/formats/assembly_chart.pptx"
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
    title: "첨단 기능 알아보기"
    exclude: "chart"
    description: "이 플랫폼은 데이터 시각화와 원활한 통합을 위한 도구로 문서 생성을 간소화합니다."
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
    title: "다양한 파일 형식으로 보고서 생성하기"
    exclude: "PPTX"
    description: "Node.js via Java는 50개 이상의 형트를 지원하여 데이터를 템플릿과 결합하여 세련된 문서를 생성하는 것이 쉽습니다."
    items: 
          
        # format loop 1
        - name: "PDF의 차트"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX의 차트"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX의 차트"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX의 차트"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---