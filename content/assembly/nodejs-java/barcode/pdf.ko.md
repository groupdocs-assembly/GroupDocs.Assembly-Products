



---
############################# Static ############################
layout: "format"
date:  2025-02-24T17:52:05
draft: false
lang: ko
format: Pdf
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript를 사용하여 PDF 파일에 바코드 추가"
head_description: "GroupDocs.Assembly for Node.js via Java API로 문서 및 이메일에 바코드를 생성하고 삽입합니다."

############################# Header ############################
title: "Node.js를 사용하여 PDF 파일에 바코드 생성" 
description: "GroupDocs.Assembly for Node.js via Java를 사용하면 PDF 문서에 바코드를 동적으로 생성하고 사용자 지정하며 삽입할 수 있습니다."
subtitle: "GroupDocs.Assembly for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "시작하기"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Assembly for Node.js via Java 소개"
    link: "/assembly/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       [GroupDocs.Assembly for Node.js via Java](/assembly/nodejs-java/)는 여러 소스의 데이터를 결합하여 전문적인 문서를 만들 수 있게 해줍니다. 차트, 표, 목록, 이미지 및 바코드를 문서에 추가할 수 있습니다. 콘텐츠를 정확히 필요하는 곳에 정리할 수 있도록 템플릿을 사용하세요. PDF, Office 문서 및 이메일을 포함하여 50개 이상의 형식과 호환됩니다.

############################# Steps ############################
steps:
    enable: true
    title: "PDF 파일에 바코드 추가 단계"
    content: |
      [GroupDocs.Assembly](/assembly/nodejs-java/)는 PDF 문서에 바코드를 삽입하는 과정을 간소화합니다. 1D 및 2D 형식을 포함하여 60개 이상의 바코드 유형을 지원합니다.
      
      1. 바코드 자리 표시자를 포함한 템플릿을 디자인합니다 (PDF 템플릿은 지원되지 않습니다).
      2. 호환 가능한 소스에서 데이터를 검색합니다.
      3. 크기 및 해상도와 같은 바코드 옵션을 설정합니다.
      4. 바코드를 포함한 문서를 PDF 파일로 내보냅니다.
   
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
        // 출력 문서에 바코드를 포함하려면 템플릿에 이 태그를 사용하세요.
        // <<barcode [barcode_expression] -barcode_type>>
    
        const assemblyLib = require('@groupdocs/groupdocs.assembly');

        // 템플릿 파일의 경로를 지정하세요.
        // 참고: PDF 템플릿은 현재 지원되지 않습니다.
        const template = "barcode_template.docx";

        // 소스에서 필요한 데이터를 로드하세요.
        const data 
            = new assemblyLib.DataSourceInfo(GetData(), "label");

        // 바코드를 포함한 문서를 PDF 파일로 내보냅니다.
        const asm = new assemblyLib.DocumentAssembler();
        asm.assembleDocument(template, "result.pdf", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "데이터 기반 템플릿으로 문서 생성"
  description: "GroupDocs.Assembly for Node.js via Java을 사용하면 인기 있는 형식으로 전문적인 파일을 생성하면서 차트, 표, 목록, 링크, 이미지 및 바코드를 원활하게 삽입할 수 있습니다."
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Assembly의 핵심 기능"
  features:
    # feature loop
    - title: "비즈니스 데이터로 보고서 작성"
      content: "API를 사용하여 JSON, XML 및 CSV 형식의 데이터로 템플릿을 신속하고 정확하게 채울 수 있습니다."

    # feature loop
    - title: "시각적 요소 추가"
      content: "GroupDocs.Assembly는 실시간으로 차트, 표, 목록, 텍스트, 링크, 이미지 및 바코드와 같은 요소를 삽입할 수 있도록 지원합니다."

    # feature loop
    - title: "데이터 배치 제어"
      content: "LINQ 기반 템플릿으로 데이터를 정확하게 배치하고 배열을 순회하며 프로그래밍 방식으로 사용자 정의 형식을 적용할 수 있습니다."

    # feature loop
    - title: "다양한 형식과 호환"
      content: "MS Office 문서, PDF, HTML, OpenOffice 파일 및 이메일과 같은 파일에서 작업할 수 있습니다. 필요에 따라 여러 문서를 병합할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "예제: 프로그래밍 방식으로 바코드 생성"
      content: |
        이 예제에서는 PDF 문서에 바코드를 프로그래밍 방식으로 생성하고 삽입하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```javascript {style=abap}
          // 바코드 자리 표시자가 포함된 템플릿을 디자인합니다.
          // <<barcode [barcode_expression] -barcode_type>>
          
          const assemblyLib = require('@groupdocs/groupdocs.assembly');

          // 템플릿 파일의 경로를 지정합니다.
          // 참고: PDF 템플릿은 현재 지원되지 않습니다.
          const template = "barcode_template.docx";

          // 소스에서 데이터를 가져옵니다.
          const data_csv =
              new assemblyLib.CsvDataSource("Barcode Labels.csv", 
              new assemblyLib.CsvDataLoadOptions(true));

          // 필요한 세부정보로 데이터를 원본 객체를 생성합니다.
          const data 
              = new assemblyLib.DataSourceInfo(data_csv, "label");

          // DocumentAssembler의 인스턴스를 초기화합니다.
          const asm = new assemblyLib.DocumentAssembler();

          // 바코드 구성을 설정합니다.
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // 바코드가 포함된 문서를 저장합니다.
          asm.assembleDocument(template, "result.pdf", data);
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
            link: "/examples/assembly/formats/assembly_barcode.pdf"
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
    title: "핵심 기능 탐색"
    exclude: "barcode"
    description: "고급 도구와 자동화 기능을 활용하여 문서 처리 과정을 간소화합니다."
    items: 
          
        # operation loop 1
        - name: "바코드 생성"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "문서에 바코드를 동적으로 생성하고 추가"

        # operation loop 2
        - name: "다이어그램으로 데이터 시각화"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "다양한 다이어그램 유형에 데이터를 채우기"

        # operation loop 3
        - name: "문서 병합"
          operation: "document"
          link: "/assembly/nodejs-java/document/pdf/"
          description: "한 문서의 내용을 다른 문서에 결합"

        # operation loop 4
        - name: "목록으로 데이터 표시"
          operation: "list"
          link: "/assembly/nodejs-java/list/pdf/"
          description: "특정 데이터를 사용하여 문서에 목록 생성"

        # operation loop 5
        - name: "표로 데이터 정리"
          operation: "table"
          link: "/assembly/nodejs-java/table/pdf/"
          description: "모든 소스에서 데이터를 검색하고 표를 채우기"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "보고서 생성을 위한 지원 파일 형식"
    exclude: "PDF"
    description: "Node.js via Java는 50개 이상의 파일 형식을 처리하여 데이터 병합 및 템플릿 처리를 통해 고품질 결과를 얻는 것을 단순하게 만듭니다."
    items: 
          
        # format loop 1
        - name: "PDF에 바코드 추가"
          format: "PDF"
          link: "/assembly/nodejs-java/barcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 바코드 추가"
          format: "DOCX"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 3
        - name: "PPTX에 바코드 추가"
          format: "PPTX"
          link: "/assembly/nodejs-java/barcode/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에 바코드 추가"
          format: "XLSX"
          link: "/assembly/nodejs-java/barcode/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"


          

---