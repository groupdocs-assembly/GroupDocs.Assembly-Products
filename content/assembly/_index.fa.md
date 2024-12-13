---
############################# Static ############################
layout: "family"
date:  2024-12-13T10:30:57
draft: false

product: "Assembly"
product_tag: "assembly"

lang: fa

############################# Head ############################
head_title: "APIهای .NET و Java و برنامه‌های آنلاین تجزیه و تحلیل مستندات توسط GroupDocs"
head_description: "راه حل اتوماسیون و گزارش‌دهی مستندات یکپارچه برای برنامه‌های .NET و Java. تولید همه مستندات رایج از الگوهای سفارشی و داده‌ها."

############################# Header ############################
title: "راه حل اتوماسیون و گزارش‌دهی مستندات"
description:  |
  گزارش‌های دقیق را با استفاده از الگوها و منابع داده با برنامه‌ها و APIهای چندسکویی ما ایجاد کنید.

  گزارش‌هایی با فرمت‌هایی مانند Word، Excel، ارائه، و بسیاری دیگر تولید کنید که با استفاده از الگوهای با نشانه‌گذاری انعطاف‌پذیر ایجاد شوند.

  نمودارها، بارکدها، جداول و عناصر دیگر را با داده‌هایی از منابعی مانند JSON، XML، CSV و غیره پر کنید.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "پلتفرم خود را انتخاب کنید"
  title: "عدم وابستگی به پلتفرم"
  description: "GroupDocs.Assembly با سیستم‌عامل‌ها و فریم‌ورک‌های زیر سازگار است:"
  details_link_title: "بیشتر بدانید"

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


############################# Features ###############################
features:
  enable: true
  title: "ویژگی‌های کلیدی GroupDocs.Assembly"
  description: "این راه حل به شما کمک می‌کند تا گزارش‌هایی در فرمت‌های مستندات محبوب ایجاد کنید که به‌طور خودکار با داده‌های تجاری شما پر شوند. کارهای تولید مستندات خود را به‌طور خودکار کنید."

  items:
    # items loop
    - icon: "additional"
      title: "پر کردن الگوها با داده‌ها"
      content: "گزارش‌ها را با استفاده از داده‌های منابع پشتیبانی شده پر کنید."

    # items loop
    - icon: "manipulate"
      title: "نشانه گذاری انعطاف‌پذیر"
      content: "داده‌ها را در مستندات به طریقی سفارشی اضافه کنید."

    # items loop
    - icon: "structure"
      title: "ویژگی‌های مستندات بومی"
      content: "داده‌ها را با استفاده از جداول، نمودارها و بارکدها نمایش دهید."

    # items loop
    - icon: "merge"
      title: "همه فرمت‌های محبوب"
      content: "از همه فرمت‌های معمول مستندات پشتیبانی می‌کند."

############################# Code samples ############################
code_samples:
  enable: true
  title: "تولید گزارش‌های سفارشی‌شده به‌خوبی"
  description: "GroupDocs.Assembly نمونه‌های کد"
  items:
    # code sample loop
    - title: "استفاده از بارکدهای تولیدشده"
      content: |
       GroupDocs.Assembly نشانه‌گذاری بارکد را در الگوهای گزارش امکان‌پذیر می‌کند. هنگام ایجاد یک گزارش، بارکدی بر اساس نشانه‌گذاری و داده‌های ارائه‌شده تولید می‌شود. مسیر الگو را که شامل متن، اشیاء داده و نشانه‌گذاری است، مشخص کنید. همچنین، منبع داده‌ای که بارکد را با محتوا پر کند، مشخص کنید.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // یک نمونه از کلاس DocumentAssembler ایجاد کنید
            DocumentAssembler assembler = new DocumentAssembler();

            //مسیر الگو را مشخص کنید
            var tmp_path = "barcode_template.docx";

            //مسیر مستند خروجی را مشخص کنید
            var res_path = "result.docx";

            //یک نمونه از منبع داده ایجاد کنید
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //برای تولید گزارش AssembleDocument را فراخوانی کنید
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // یک نمونه از کلاس DocumentAssembler ایجاد کنید
            DocumentAssembler assembler = new DocumentAssembler();
            
            //مسیر الگو را مشخص کنید
            String tmp_path = "barcode_template.docx";

            //مسیر مستند خروجی را مشخص کنید
            String res_path = "result.docx";

            //یک نمونه از منبع داده ایجاد کنید
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // برای تولید گزارش AssembleDocument را فراخوانی کنید
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "پشتیبانی از 50+ فرمت فایل"
  description: "GroupDocs.Assembly با تقریباً تمامی فرمت‌های محبوب فایل کار می‌کند"

############################# Metrics ###############################
metrics:
  enable: true
  title: "آمار محصول ما"
  description: "آمار محصول را بررسی کنید تا از پیشرفت، تأثیر و رشد ما مطلع شوید."

  items:
    # items loop
    - number: "50+"
      title: "فرمت‌های پشتیبانی شده"
      content: "ما از بیش از 50 فرمت مستندات به‌طور گسترده استفاده می‌کنیم."

    # items loop
    - number: "650k"
      title: "دانلودهای NuGet"
      content: "GroupDocs.Assembly برای .NET یک کتابخانه محبوب با بیش از 650000 دانلود در NuGet است."

    # items loop
    - number: "18k"
      title: "دانلودهای Maven"
      content: "توسعه‌دهندگان Java بیش از 18000 بار GroupDocs.Assembly را در Maven دانلود کرده‌اند."

    # items loop
    - number: "150+"
      title: "مشتریان راضی"
      content: "محصولات ما به‌عنوان راه‌حل‌های نوآورانه توسط توسعه‌دهندگان مستقل و شرکت‌های پیشرو در سراسر جهان اعتماد شده‌اند."


############################# Customers ###############################
customers:
  enable: true
  title: "مشتریان راضی ما"
  description: "کتابخانه‌های GroupDocs توسط برخی از معروف‌ترین و معتبرترین برندهای جهان استفاده می‌شوند."

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
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Assembly را به‌صورت رایگان در پلتفرم خود آزمایش کنید."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/assembly/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/assembly/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "سوالات متداول"
  description: "سوالات متداول ما را مرور کنید."

  items:
    # items loop
    - question: "آیا GroupDocs.Assembly به هیچ کتابخانه خارجی برای ترکیب مستندات نیاز دارد؟"
      answer: "خیر، GroupDocs.Assembly به‌صورت مستقل کار می‌کند و نیازی به کتابخانه‌های شخص ثالث مانند Adobe Acrobat یا Microsoft Office ندارد."

    # items loop
    - question: "آیا می‌توانم قبل از خرید امکانات GroupDocs.Assembly را آزمایش کنم؟"
      answer: "بله، می‌توانید! GroupDocs.Assembly یک دوره آزمایشی رایگان ارائه می‌دهد. آن را نصب کرده و امکانات آن را بررسی کنید. نسخه آزمایشی 'برچسب‌های آزمایشی' را به مستندات شما اضافه می‌کند و تنها صفحات اول را پردازش می‌کند. برای تجربه کامل، یک مجوز موقت 30 روزه رایگان را دریافت کنید تا به همه امکانات دسترسی پیدا کنید. جزئیات بیشتر در [مجوز موقت](https://purchase.groupdocs.com/temporary-license/) در دسترس است."

    # items loop
    - question: "چه نوع مجوزهایی موجود است؟"
      answer: "آیا به دنبال مجوز GroupDocs.Assembly هستید؟ ما گزینه‌های متنوعی را بسته به نیازهای شما ارائه می‌دهیم. بر اساس اندازه تیم، محل استقرار (یک دفتر یا دورکار) و اینکه آیا به‌دنبال اشتراک SDK/API با مشتریان برای توزیع هستید، انتخاب کنید. همچنین می‌توانید مجوز استفاده ماهانه با برنامه‌های مبتنی بر اندازه را انتخاب کنید—فقط برای آنچه که استفاده می‌کنید، هزینه پرداخت کنید. بهترین گزینه را در [قیمت‌گذاری](https://purchase.groupdocs.com/pricing/assembly/net/) پیدا کنید."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "APIهای کم‌کد GroupDocs.Assembly"
  description: "با استفاده از API REST مبتنی بر ابر ما، مستندات را از طریق برنامه خود تولید کنید."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "از API RESTful cURL برای افزودن داده به Word، Excel، PowerPoint و بسیاری از الگوها استفاده کنید."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "برنامه‌های .NET خود را با تولید گزارش از طریق SDK ابری بهبود دهید. داده‌های تجاری را در فرمت سفارشی خود نمایش دهید."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "GroupDocs.Assembly SDK گزینه‌های مختلفی را برای برنامه‌های Java برای تولید انواع مختلف مستندات ارائه می‌دهد."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "برنامه‌های وب GroupDocs.Assembly"
  description: "GroupDocs.Assembly یک برنامه وب رایگان برای تولید مستندات ارائه می‌دهد. می‌توانید بیش از 50 فرمت فایل محبوب را به‌طور مستقیم در مرورگر خود پردازش کنید، به‌صورت رایگان."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "گزارش‌ها را در Excel، Word، PowerPoint و بسیاری دیگر از نوع فایل‌ها به‌طور مستقیم از مرورگر وب خود تولید کنید."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "مستندات Microsoft Word را از الگوها و منابع داده ایجاد کنید."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "یک الگو و یک منبع داده را بارگذاری کنید تا به‌صورت رایگان گزارش‌های Excel تولید کنید."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---