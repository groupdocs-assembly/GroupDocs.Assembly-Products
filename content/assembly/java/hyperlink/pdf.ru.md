---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/assembly/java/hyperlink/pdf/"
otherformats: HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOCM DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Добавление гиперссылок в документы и отчеты Office PDF через Java API"
head_description: "GroupDocs.Assembl для Java поддерживает динамическую вставку гиперссылок на офисные документы и документы электронной почты, такие как PDF DOCX, RTF, XLSX, PPTX, EML, MSG и другие, внутри приложений Java."

############################# Header ############################
title: "Добавление гиперссылок в документы Office и сообщения электронной почты через Java API"
description: "GroupDocs.Assembly Java API позволяет профессионалам программного обеспечения программно добавлять гиперссылки в сообщения электронной почты и документы Office, такие как PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, MSG и другие."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Как использовать Java API для добавления гиперссылок в документы Office и электронные письма?"
    content: |
       Гиперссылка — это слово, фраза или изображение, по которым можно щелкнуть, чтобы перейти к новому документу или новому разделу в текущем документе. Гиперссылки являются основой всемирной паутины и используются для многих необходимых функций во всемирной паутине. GroupDocs.Assembly для Java — это API автоматизации документов и создания отчетов, который помогает разработчикам программного обеспечения динамически вставлять гиперссылки в свои документы или отчеты. API очень стабилен и полностью поддерживает несколько расширенных функций, связанных с управлением гиперссылками, таких как добавление гиперссылок на страницу документа, добавление ссылок на слайд презентации, добавление гиперссылок в ячейки электронной таблицы, изменение содержимого гиперссылок, динамическая вставка ссылок из закладок, удаление ненужных ссылок. ссылки, показывать текст вместо гиперссылки и многое другое. Некоторые из очень распространенных типов документов, такие как PDF, HTML, электронная почта Outlook, Microsoft Office Word, рабочие листы Excel, презентации PowerPoint и т. д., полностью поддерживаются.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Вставка гиперссылок на документы обработки текста через Java"
      content_left: |
       Java API GroupDocs.Assembly полностью поддерживает вставку и редактирование гиперссылок внутри различных широко используемых форматов документов. В приведенном ниже примере кода Java показано, как вставлять гиперссылки в документ Microsoft Word.

      title_right: "Вставка гиперссылок в документ PDF с помощью Java"
      content_right: |
        * Настройка исходных и целевых документов
        * Установить выражение Uri, а также отображать текстовое выражение
        * Создайте экземпляр класса [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler).
        * Вызовите [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) для сборки документа. Он поддерживает
          * Поток для чтения шаблона документа.
          * Поток для записи результирующего документа.
          * Дополнительные возможности загрузки и сохранения документа.
          * Информация об объектах источника данных.

      gisthash: "ecae8e7f8626f52f4dda03e76c96ff57"
      gistfile: "add_hyperlinks_to_word_documents.java"

    - title_left: "Добавить гиперссылки в электронные таблицы через Java"
      content_left: |
       Java API GroupDocs.Assembly позволяет программистам с легкостью вставлять и изменять гиперссылки внутри своих электронных таблиц. Они могут легко получить доступ, отредактировать его местоположение или заменить его новым. Следующий код Java демонстрирует, как легко программисты могут добавлять гиперссылки в свои электронные таблицы.

      title_right: "Как вставить гиперссылки в файл PDF"
      content_right: |
        * Настройка исходного и целевого файлов электронных таблиц
        * Установить выражение Uri, а также отображать текстовое выражение
        * Создайте экземпляр класса [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler).
        * Вызовите [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) для сборки документа. Он поддерживает
          * Поток для чтения шаблона документа.
          * Поток для записи результирующего документа.
          * Дополнительные возможности загрузки и сохранения документа.
          * Информация об объектах источника данных.

      gisthash: "92bbf74f1dd23e5f7c6e5b5db0ff2504"
      gistfile: "add_hyperlinks_in_ spreadsheet_documents.java"

    - title_left: "Вставка гиперссылок в презентацию PowerPoint через Java"
      content_left: |
       Java API GroupDocs.Assembly упрощает для программистов решение задач, связанных с управлением документами. Вот пример кода Java, который показывает, как легко программисты могут получить доступ к своим документам презентации PowerPoint и добавить в них гиперссылки.

      title_right: "Как вставлять гиперссылки в презентации"
      content_right: |
        * Настройка исходных и целевых файлов презентации
        * Установите Uri и отобразите текстовые выражения
        * Создайте экземпляр класса [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler).
        * Вызовите [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) для сборки документа. Он поддерживает
          * Поток для чтения шаблона документа.
          * Поток для записи результирующего документа.
          * Дополнительные возможности загрузки и сохранения документа.
          * Информация об объектах источника данных.

      gisthash: "06535fd50bfd353db586671a504d2783"
      gistfile: "add_hyperlinks_in_ presentation_documents.java"

    - title_left: "Используйте Java API для добавления гиперссылок в сообщения электронной почты"
      content_left: |
       GroupDocs.Assembly for Java позволяет разработчикам программного обеспечения легко добавлять гиперссылки в свои сообщения электронной почты с помощью всего нескольких строк кода Java. В следующем примере показано, как легко разработчики могут вставлять гиперссылки в свои документы электронной почты и отправлять их другим пользователям в своих собственных приложениях Java.

      title_right: "Как добавить гиперссылки в электронные письма"
      content_right: |
        * Настройка исходного и целевого файлов электронных таблиц
        * Установите Uri и отобразите текстовые выражения
        * Создайте экземпляр класса [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler).
        * Вызовите [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) для сборки документа. Он поддерживает
          * Поток для чтения шаблона документа.
          * Поток для записи результирующего документа.
          * Дополнительные возможности загрузки и сохранения документа.
          * Информация об объектах источника данных.

      gisthash: "551cef5d45d08caa851d483a705114bb"
      gistfile: "add_hyperlinks_in_email_documents.java"  

    - title_left: "Системные Требования"
      content_left: |
       API GroupDocs.Assembly Java поддерживаются на всех основных платформах и операционных системах. Он может создавать документы в Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice и более 50 других форматах. Полное руководство по системным требованиям см. на странице [системные требования](https://docs.groupdocs.com/assembly/java/system-requirements/). Перед выполнением приведенного ниже кода убедитесь, что на вашем компьютере установлены следующие предварительные компоненты. система:
         * Операционные системы: Microsoft Windows, Linux, MacOS
         * Поддержка версий Java: J2SE 7.0 (1.7), J2SE 8.0 (1.8) или выше
         * Получите последнюю версию Java API GroupDocs.Assembly от [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/)
        
      title_right: "Зачем использовать GroupDocs.Assembly"
      content_right: |
        * Создание пользовательских документов из шаблонов.
        * Динамически прикреплять вложения электронной почты.
        * Для создания и автоматизации документов не требуется никакого дополнительного программного обеспечения.
        * Создает выходной документ на основе источника данных.
        * Динамически вставлять содержимое документа в отчет
        * Применение формулы во время сборки электронной таблицы.
        * Обеспечивает поддержку нескольких форматов данных
        * Поддержка последовательных операций с данными.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---