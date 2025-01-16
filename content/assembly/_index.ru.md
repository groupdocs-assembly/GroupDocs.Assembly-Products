---
############################# Static ############################
layout: "family"
date:  2025-01-16T13:04:05
draft: false

product: "Assembly"
product_tag: "assembly"

lang: ru

############################# Head ############################
head_title: "APIs для .NET, Java, Node.js и онлайн-приложения для сборки документов от GroupDocs"
head_description: "Получите универсальное решение для автоматизации документов и отчетности для приложений на .NET, Java и Node.js. Генерируйте все стандартные документы из пользовательских шаблонов и данных."

############################# Header ############################
title: "Решение для автоматизации документов и отчетности"
description:  |
  Создавайте подробные отчеты, используя шаблоны и источники данных с помощью наших кроссплатформенных приложений и API.

  Генерируйте отчеты в форматах, таких как Word, Excel, Презентации и многих других, используя шаблоны с гибкой разметкой.

  Заполняйте диаграммы, штрих-коды, таблицы и другие элементы данными из источников, таких как JSON, XML, CSV и т.д.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Выберите вашу платформу"
  title: "Платформенная независимость"
  description: "GroupDocs.Assembly совместим с следующими операционными системами и фреймворками:"
  details_link_title: "Узнать больше"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Assembly .NET 
      color: "blue"
      tag: "net"
      link: "/assembly/net/"
      features_link: "https://docs.groupdocs.com/assembly/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 2.0 or higher <br> Mono Framework 1.2 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Microsoft Azure <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> Xamarin.Android <br> MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Assembly Java
      color: "red"
      tag: "java"
      link: "/assembly/java/"
      features_link: "https://docs.groupdocs.com/assembly/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 7 (1.7) or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Assembly "Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/assembly/nodejs-java/"
      features_link: "https://docs.groupdocs.com/assembly/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Любой другой текстовый редактор
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Ключевые функции GroupDocs.Assembly"
  description: "Это решение помогает вам создавать отчеты в популярных форматах документов, автоматически заполняя их вашими бизнес-данными. Автоматизируйте задачи генерации документации."

  items:
    # items loop
    - icon: "additional"
      title: "Заполнение шаблонов данными"
      content: "Заполняйте отчеты, используя данные из поддерживаемых источников."

    # items loop
    - icon: "manipulate"
      title: "Гибкая разметка"
      content: "Добавляйте данные в документы настраиваемым способом."

    # items loop
    - icon: "structure"
      title: "Нативные функции документа"
      content: "Отображайте данные, используя таблицы, диаграммы и штрих-коды."

    # items loop
    - icon: "merge"
      title: "Все популярные форматы"
      content: "Поддерживает все часто используемые форматы документов."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Генерация хорошо настроенных отчетов"
  description: "GroupDocs.Assembly примеры кода"
  items:
    # code sample loop
    - title: "Использование сгенерированных штрих-кодов"
      content: |
       GroupDocs.Assembly позволяет использовать разметку штрих-кодов в шаблонах отчетов. При создании отчета штрих-код генерируется на основе разметки и предоставленных данных. Укажите путь к шаблону, содержащему текст, объекты данных и разметку. Также укажите источник данных для заполнения штрих-кода содержимым.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Создайте экземпляр класса DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Укажите путь к шаблону
            var tmp_path = "barcode_template.docx";

            //Укажите путь для итогового документа
            var res_path = "result.docx";

            //Создайте экземпляр источника данных
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Вызовите AssembleDocument, чтобы сгенерировать отчет
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Создайте экземпляр класса DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Укажите путь к шаблону
            String tmp_path = "barcode_template.docx";

            //Укажите путь для итогового документа
            String res_path = "result.docx";

            //Создайте экземпляр источника данных
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Вызовите AssembleDocument, чтобы сгенерировать отчет
            assembler.assembleDocument(tmp_path, res_path, data);

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const assemblyLib = require('@groupdocs/groupdocs.assembly');

            // Создайте экземпляр класса DocumentAssembler
            const assembler = new assemblyLib.DocumentAssembler();
            
            //Укажите путь к шаблону
            const tmp_path = "barcode_template.docx";

            //Укажите путь для итогового документа
            const res_path = "result.docx";

            //Создайте экземпляр источника данных
            const data = new assemblyLib.DataSourceInfo(new assemblyLib.DataStorage(), null);

            // Вызовите AssembleDocument, чтобы сгенерировать отчет
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Поддержка более 50 форматов файлов"
  description: "GroupDocs.Assembly работает практически со всеми популярными форматами файлов"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Статистика нашего продукта"
  description: "Изучите показатели продукта, чтобы получить представление о нашем прогрессе, влиянии и росте."

  items:
    # items loop
    - number: "50+"
      title: "Поддерживаемые форматы"
      content: "Мы поддерживаем более 50 наиболее широко используемых форматов документов."

    # items loop
    - number: "650k"
      title: "Загрузки NuGet"
      content: "GroupDocs.Assembly для .NET является популярной библиотекой с более чем 650 000 загрузок на NuGet."

    # items loop
    - number: "18k"
      title: "Загрузки Maven"
      content: "Разработчики Java загрузили GroupDocs.Assembly на Maven более 18 000 раз."

    # items loop
    - number: "150+"
      title: "Счастливые клиенты"
      content: "Наши продукты пользуются доверием индивидуальных разработчиков и ведущих компаний по всему миру для создания инновационных решений."


############################# Customers ###############################
customers:
  enable: true
  title: "Наши довольные клиенты"
  description: "Библиотеки GroupDocs используются некоторыми из самых известных и уважаемых брендов по всему миру."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Готовы начать?"
  description: "Тестируйте функции GroupDocs.Assembly бесплатно на вашей платформе."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/assembly/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Часто задаваемые вопросы"
  description: "Просмотрите наши часто задаваемые вопросы."

  items:
    # items loop
    - question: "Требует ли GroupDocs.Assembly каких-либо внешних библиотек для составления документов?"
      answer: "Нет, GroupDocs.Assembly работает независимо и не требует сторонних библиотек, таких как Adobe Acrobat или Microsoft Office."

    # items loop
    - question: "Могу ли я протестировать функции GroupDocs.Assembly перед покупкой?"
      answer: "Да, вы можете! GroupDocs.Assembly предлагает бесплатную пробную версию. Установите его и исследуйте его функции. Пробная версия добавляет «значки пробной версии» в ваши документы и обрабатывает только первые 3 страницы. Для полного опыта получите бесплатную 30-дневную временную лицензию, чтобы получить доступ ко всем функциям. Дополнительные детали доступны в разделе [временная лицензия](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Какие типы лицензий доступны?"
      answer: "Ищете лицензию GroupDocs.Assembly? Мы предлагаем различные варианты, чтобы удовлетворить ваши потребности. Выберите в зависимости от размера вашей команды, места развертывания (один офис или удаленный) и необходимости делиться SDK/API с клиентами для распространения. В качестве альтернативы выберите лицензию на использование на месяц с метered планами — платите только за то, что используете. Найдите лучший вариант для вас в разделе [цены](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Assembly API с низким уровнем кода"
  description: "Генерируйте документы с помощью вашего приложения через наш облачный REST API."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Используйте cURL RESTful API, чтобы добавить данные в Word, Excel, PowerPoint и многие другие шаблоны."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Улучшите свои .NET приложения, создавая отчеты с помощью Cloud SDK. Отображайте бизнес-данные в вашем пользовательском формате."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK предлагает различные возможности для Java-приложений для генерации различных типов документов."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Assembly Веб-приложения"
  description: "GroupDocs.Assembly предлагает бесплатное веб-приложение для генерации документов. Вы можете обрабатывать более 50 популярных форматов файлов прямо в своем браузере, БЕСПЛАТНО."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Генерируйте отчеты в Excel, Word, PowerPoint и многих других форматах файла напрямую из вашего веб-браузера."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Создавайте документы Microsoft Word из шаблонов и источников данных."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Загрузите шаблон и источник данных, чтобы бесплатно создать отчеты Excel."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---