



---
############################# Static ############################
layout: "format"
date:  2025-01-13T15:11:17
draft: false
lang: zh
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
    link_title: "了解更多"
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
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/assembly/assembly_all.pdf"
      result_title: "示例文档"
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
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/assembly/nodejs-java/"
          
      content: |
        ```java {style=abap}
        // {examples.comment_1}
        // Orders Prices by months<<y [Sum(c => c.Price)]>><<size [Count()]>>

        // {examples.comment_2}
        String template = "chart_template.docx";

        // {examples.comment_3}
        DataSourceInfo data 
            = new DataSourceInfo(GetChartData(), "orders");

        // {examples.comment_4}
        DocumentAssembler asm = new DocumentAssembler();
        asm.assembleDocument(template, "result.docx", data);
        ```           

############################# More features ############################
more_features:
  enable: true
  title: "{more_features.title}"
  description: "{more_features.description}"
  image: "/img/assembly/features_chart.webp" # 500x500 px
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
          // Total Contract Price<<y [m.Total_Contract_Price]>>
          // <<seriesColor [color]>>

          // {code_1.comment_2}
          String template = "table_template.docx";

          // {code_1.comment_3}
          JsonDataSource data_json = 
            new JsonDataSource("Items.json");

          // {code_1.comment_4}
          DataSourceInfo data 
              = new DataSourceInfo(data_json, "items");

          // {code_1.comment_5}
          DataSourceInfo design 
              = new DataSourceInfo("red", "color");

          // {code_1.comment_6}
          DocumentAssembler asm = new DocumentAssembler();

          // {code_1.comment_7}
          asm.assembleDocument(template, "result.docx", data, design);
          ```
        platform: "java"
        copy_title: "复制"
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
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/assembly/formats/assembly_chart.docx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-assembly/GroupDocs.Assembly-for-Node.js-via-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/assembly/nodejs-java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费探索GroupDocs.Assembly的功能或请求许可证"
  items:
    #  loop
    - title: "从NPM下载"
      link: "https://releases.groupdocs.com/assembly/nodejs-java/"
      color: "red"
        #  loop
    - title: "了解许可证信息"
      link: "https://purchase.groupdocs.com/pricing/assembly/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: ""
    exclude: "chart"
    description: ""
    items: 
          
        # operation loop 1
        - name: "生成条形码"
          operation: "barcode"
          link: "/assembly/nodejs-java/barcode/docx/"
          description: "动态创建并添加条形码到文档中"

        # operation loop 2
        - name: "用图表可视化数据"
          operation: "chart"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "用数据填充各种图表类型"

        # operation loop 3
        - name: "合并文档"
          operation: "document"
          link: "/assembly/nodejs-java/document/docx/"
          description: "将一个文档的内容合并到另一个文档中"

        # operation loop 4
        - name: "使用列表展示数据"
          operation: "list"
          link: "/assembly/nodejs-java/list/docx/"
          description: "使用特定数据在文档中生成列表"

        # operation loop 5
        - name: "在表格中组织数据"
          operation: "table"
          link: "/assembly/nodejs-java/table/docx/"
          description: "从任何来源获取数据并填充表格"
         
          
############################# More Formats ########################
more_formats:
    enable: true
    title: ""
    exclude: "DOCX"
    description: ""
    items: 
          
        # format loop 1
        - name: "在PDF中插入图表"
          format: "PDF"
          link: "/assembly/nodejs-java/chart/pdf/"
          description: "Adobe可移植文档格式"
          
        # format loop 2
        - name: "在DOCX中插入图表"
          format: "DOCX"
          link: "/assembly/nodejs-java/chart/docx/"
          description: "Microsoft Word开放XML文档"
          
        # format loop 3
        - name: "在PPTX中插入图表"
          format: "PPTX"
          link: "/assembly/nodejs-java/chart/pptx/"
          description: "PowerPoint开放XML演示文稿"
          
        # format loop 4
        - name: "在XLSX中插入图表"
          format: "XLSX"
          link: "/assembly/nodejs-java/chart/xlsx/"
          description: "Microsoft Excel开放XML电子表格"


          

---