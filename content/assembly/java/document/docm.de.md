---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/assembly/java/document/docm"
otherformats: PDF HTML XPS TIFF MHTML TXT XAML EPUB SVG PS PCL XML OTT OXPS MD POT OTP DOC DOCX DOT DOTX DOTM RTF ODT OTT XLS XLT XLSX XLSM XLTX XLTM XLSB ODS PPT PPTX PPTM PPS PPSX PPSM  POTX POTM ODP EML EMLX MSG 

############################# Head ############################
head_title: "Java-API: Inhalte externer Dokumente zu DOCM-Dateiformaten hinzufügen"
head_description: "GroupDocs.Assembly Java API ermöglicht das dynamische Einfügen von Inhalten externer Dokumente in verschiedene Dateiformate wie PDF, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG und mehr."

############################# Header ############################
title: "Java-API zum Einfügen des Inhalts externer Dokumente in andere unterstützte Dateiformate"
description: "GroupDocs.Assembly für Java bietet Funktionen zum Einfügen des Inhalts externer Dokumente in Berichte, E-Mails und verschiedene unterstützte Dateiformate wie PDF, DOC, DOCX, XLSX, CSV, PPTX, EML, MSG und mehr."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Wie füge ich den Inhalt externer Dokumente über Java in andere gängige Dateiformate ein?"
    content: |
       Ein Dokument oder eine Datei ist eine elektronische Kopie oder Papierkopie, die Informationen enthält, die zu einem späteren Zeitpunkt vom Benutzer abgerufen werden können. Laut Wikipedia kann ein Dokument strukturiert sein wie tabellarische Dokumente, Listen, Formulare oder wissenschaftliche Diagramme, halbstrukturiert wie ein Buch oder ein Zeitungsartikel oder unstrukturiert wie eine handschriftliche Notiz. GroupDocs.Assembly für Java ist eine sehr nützliche API, die es Softwareentwicklern ermöglicht, leistungsstarke Anwendungen für die Dokumentenautomatisierung und Berichterstellung zu erstellen. Es unterstützt vollständig das Identifizieren und Arbeiten mit zahlreichen Dokumentformaten wie PDF, Microsoft Word, Excel-Arbeitsblättern, PowerPoint, HTML, Outlook-E-Mail und vielen mehr. Es unterstützt zahlreiche erweiterte Funktionen für die Arbeit mit Berichten, z. B. das Bearbeiten von Vorlagenelementen, Listenberichten, Diagrammberichten, Tabellenberichten usw. Darüber hinaus unterstützt die API auch mehrere erweiterte Funktionen in Bezug auf das Hinzufügen und Ändern von Dokumentinhalten, wie z. B. das Hinzufügen von Inhalten zu einer Dokumentseite, das Einfügen von Daten in Tabellenkalkulationszellen, das Ersetzen von Inhalten, das Hinzufügen von Inhalten zu einer Präsentationsfolie und vieles mehr.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Hinzufügen externer Dateiinhalte zu Word-Dokumenten über Java"
      content_left: |
       Die Java-API GroupDocs.Assembly hilft Computerprogrammierern, Aufgaben zur Manipulation von Dokumenten in ihren eigenen Java-Apps zu erledigen. Es unterstützt vollständig Dateiinhalte eines externen Dokuments für verschiedene Arten von Dokumenttypen. Das folgende Java-Codebeispiel zeigt, wie Sie den Inhalt einer äußeren Datei mit nur wenigen Codezeilen zu einem Textverarbeitungsdokument hinzufügen. 

      title_right: "So fügen Sie den Inhalt des Dokuments in die DOCM-Datei ein"
      content_right: |
        * Quelldokumentvorlage festlegen
        * Einstellen des Zieldokumentberichts
        * Erstellen Sie eine Instanz der Klasse [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler).
        * Rufen Sie [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-)  auf Methode zum Zusammenstellen des Dokuments. Es unterstützt
          * Der Stream, aus dem ein Vorlagendokument gelesen werden soll.
          * Der Stream zum Schreiben eines Ergebnisdokuments.
          * Gibt zusätzliche Optionen zum Laden und Speichern von Dokumenten an.
          * Stellt Informationen zu zu verwendenden Datenquellenobjekten bereit.

      gisthash: "abb65f9e514add59870865121ed3c526"
      gistfile: "insert_documents_to_word_processing.java"

    - title_left: "Fügen Sie den Inhalt externer Dateien per Java zu E-Mail-Nachrichten hinzu"
      content_left: |
       Die Java-API von GroupDocs.Assembly enthält Funktionen zum dynamischen Einfügen von Inhalten externer Dokumente in mehrere gängige Dokumentdateiformate und E-Mail-Nachrichten. Der folgende Java-Code zeigt, wie Programmierer den Inhalt des äußeren Dokuments ohne externe Anwendung zu ihren E-Mail-Dokumenten hinzufügen können.

      title_right: "So fügen Sie Dateiinhalte zu DOCM-Dokument hinzu"
      content_right: |
        * Quelldokumentvorlage festlegen
        * Einstellen des Zieldokumentberichts
        * Erstellen Sie eine Instanz der Klasse [DocumentAssembler](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler).
        * Rufen Sie [AssembleDocument](https://apireference.groupdocs.com/assembly/java/com.groupdocs.assembly/DocumentAssembler#assembleDocument-java.io.InputStream-java.io.OutputStream-com.groupdocs.assembly.LoadSaveOptions-com.groupdocs.assembly.DataSourceInfo...-) auf Methode zum Zusammenstellen des Dokuments. Es unterstützt
          * Der Stream, aus dem ein Vorlagendokument gelesen werden soll.
          * Der Stream zum Schreiben eines Ergebnisdokuments.
          * Gibt zusätzliche Optionen zum Laden und Speichern von Dokumenten an.
          * Stellt Informationen zu zu verwendenden Datenquellenobjekten bereit.

      gisthash: "b72d7608548993ffbe62f97c798ba021"
      gistfile: "Insert_dynamic_documents_to_emails.java"

    - title_left: "System Anforderungen"
      content_left: |
        GroupDocs.Assembly-Java-APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Es kann Dokumente in Microsoft Word, Excel, PowerPoint, Outlook, OpenOffice und über 50 anderen Formaten erstellen. Eine vollständige Anleitung zu den Systemanforderungen finden Sie unter [Systemanforderungen](https://docs.groupdocs.com/assembly/java/system-requirements/). Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem installiert sind System:
         * Betriebssysteme: Microsoft Windows, Linux, MacOS
         * Unterstützung für Java-Versionen: J2SE 7.0 (1.7), J2SE 8.0 (1.8) oder höher
         * Holen Sie sich die neueste Version der GroupDocs.Assembly-Java-APIs von [Maven](https://mvnrepository.com/artifact/com.groupdocs/groupdocs-assembly/)
        
      title_right: "Warum GroupDocs.Assembly verwenden"
      content_right: |
        * Erstellen Sie benutzerdefinierte Dokumente aus Vorlagen.
        * E-Mail-Anhänge dynamisch anhängen.
        * Zum Erstellen und Automatisieren von Dokumenten ist keine zusätzliche Software erforderlich.
        * Generiert ein Ausgabedokument basierend auf der Datenquelle.
        * Fügen Sie den Dokumentinhalt dynamisch in den Bericht ein
        * Wenden Sie die Formel während der Tabellenkalkulation an.
        * Bietet Unterstützung für mehrere Datenformate
        * Unterstützung für sequentielle Datenoperationen.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---