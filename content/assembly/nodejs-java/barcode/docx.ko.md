



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:16
draft: false
lang: ko
format: Docx
product: "Assembly"
product_tag: "assembly"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: ""
head_description: ""

############################# Header ############################
title: "" 
description: ""
subtitle: "" 

header_actions:
  enable: true
  items:
    #  loop
    - title: ""
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: ""
    link: "/assembly/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_assembly.svg" # 480 X 400
    content: |
       

############################# Steps ############################
steps:
    enable: true
    title: "{steps.title}"
    content: |
      {steps.content.title}
      
      1. {steps.content.step_1}
      2. {steps.content.step_2}
      3. {steps.content.step_3}
      4. {steps.content.step_4}
   
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
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```java {style=abap}
        // {examples.comment_1}
        // <<barcode [barcode_expression] -barcode_type>>

        // {examples.comment_2}
        String template = "barcode_template.docx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetData(), "label");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_barcode.webp" # 500x500 px
  image_description: "{more_features.image_description}"
  features:
    # feature loop
    - title: "{more_features.feature_1.title}"
      content: "{more_features.feature_1.content}"

    # feature loop
    - title: "{more_features.feature_2.title}"
      content: "{more_features.feature_2.content}"

    # feature loop
    - title: "{more_features.feature_3.title}"
      content: "{more_features.feature_3.content}"

    # feature loop
    - title: "{more_features.feature_4.title}"
      content: "{more_features.feature_4.content}"
      
  code_samples_ext:
    # code sample ext loop
    - title: "{code_1.title}"
      content: |
        {code_1.content}
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // {code_1.comment_1}
          // <<barcode [barcode_expression] -barcode_type>>

          // {code_1.comment_2}
          String template = "barcode_template.docx";

          // {code_1.comment_3}
          CsvDataSource data_csv =
              new CsvDataSource("Barcode Labels.csv", 
              new CsvDataLoadOptions(true));

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_csv, "label");

          // {code_1.comment_5}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_6}
          asm.getBarcodeSettings().setResolution(1200);
          asm.getBarcodeSettings().setBaseYDimension(5f);

          // {code_1.comment_7}
          asm.assembleDocument(template, "result.docx", data);
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
            link: "/examples/assembly/formats/assembly_barcode.docx"
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
    title: ""
    exclude: "barcode"
    description: ""
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
    title: ""
    exclude: "DOCX"
    description: ""
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