---
############################# Static ############################
layout: "family"
date:  2024-12-13T10:30:57
draft: false

product: "Assembly"
product_tag: "assembly"

lang: vi

############################# Head ############################
head_title: "APIs .NET, Java & Ứng dụng Tài liệu Trực tuyến của GroupDocs"
head_description: "Nhận Giải pháp Tự động hóa Tài liệu & Báo cáo toàn diện cho các ứng dụng .NET và Java. Tạo tất cả các tài liệu thông dụng từ các mẫu tùy chỉnh và dữ liệu."

############################# Header ############################
title: "Giải pháp Tự động hóa Tài liệu và Báo cáo"
description:  |
  Tạo báo cáo chi tiết bằng cách sử dụng mẫu và nguồn dữ liệu với các ứng dụng và API đa nền tảng của chúng tôi.

  Tạo báo cáo ở các định dạng như Word, Excel, Bản trình bày và nhiều hơn nữa bằng cách sử dụng các mẫu với cú pháp linh hoạt.

  Lấp đầy biểu đồ, mã vạch, bảng và các phần tử khác với dữ liệu từ các nguồn như JSON, XML, CSV, v.v.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Chọn nền tảng của bạn"
  title: "Tính độc lập của nền tảng"
  description: "GroupDocs.Assembly tương thích với các hệ điều hành và khung sau:"
  details_link_title: "Tìm hiểu thêm"

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
  title: "Các tính năng chính của GroupDocs.Assembly"
  description: "Giải pháp này giúp bạn tạo báo cáo ở các định dạng tài liệu phổ biến, tự động được lấp đầy bằng dữ liệu doanh nghiệp của bạn. Tự động hóa các nhiệm vụ tạo tài liệu của bạn."

  items:
    # items loop
    - icon: "additional"
      title: "Điền thông tin vào mẫu"
      content: "Lấp đầy báo cáo bằng dữ liệu từ các nguồn được hỗ trợ."

    # items loop
    - icon: "manipulate"
      title: "Cú pháp linh hoạt"
      content: "Thêm dữ liệu vào tài liệu một cách tùy biến."

    # items loop
    - icon: "structure"
      title: "Các tính năng tài liệu bản địa"
      content: "Hiển thị dữ liệu bằng cách sử dụng bảng, biểu đồ và mã vạch."

    # items loop
    - icon: "merge"
      title: "Tất cả các định dạng phổ biến"
      content: "Hỗ trợ tất cả các định dạng tài liệu được sử dụng phổ biến."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Tạo báo cáo tùy chỉnh tốt"
  description: "GroupDocs.Assembly ví dụ mã"
  items:
    # code sample loop
    - title: "Sử dụng Mã vạch Được Tạo"
      content: |
       GroupDocs.Assembly cho phép cú pháp mã vạch trong các mẫu báo cáo. Khi tạo báo cáo, một mã vạch được tạo dựa trên cú pháp và dữ liệu được cung cấp. Chỉ định đường dẫn đến mẫu chứa văn bản, đối tượng dữ liệu và cú pháp. Ngoài ra, hãy chỉ định nguồn dữ liệu để lấp đầy mã vạch với nội dung.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Tạo một thể hiện của lớp DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();

            //Chỉ định đường dẫn đến mẫu
            var tmp_path = "barcode_template.docx";

            //Chỉ định đường dẫn cho tài liệu kết quả
            var res_path = "result.docx";

            //Tạo một thể hiện của nguồn dữ liệu
            var data = new DataSourceInfo(DataLayer.GetCustomerData(), "customer");

            //Gọi AssembleDocument để tạo báo cáo
            assembler.AssembleDocument(tmp_path, res_path, data);

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Tạo một thể hiện của lớp DocumentAssembler
            DocumentAssembler assembler = new DocumentAssembler();
            
            //Chỉ định đường dẫn đến mẫu
            String tmp_path = "barcode_template.docx";

            //Chỉ định đường dẫn cho tài liệu kết quả
            String res_path = "result.docx";

            //Tạo một thể hiện của nguồn dữ liệu
            DataSourceInfo data = new DataSourceInfo(new DataStorage(), null);

            // Gọi AssembleDocument để tạo báo cáo
            assembler.assembleDocument(tmp_path, res_path, data);

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Hỗ trợ hơn 50 định dạng tệp"
  description: "GroupDocs.Assembly hoạt động với hầu hết tất cả các định dạng tệp phổ biến"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Thống kê sản phẩm của chúng tôi"
  description: "Khám phá các chỉ số sản phẩm để có cái nhìn sâu sắc về tiến trình, ảnh hưởng và sự phát triển của chúng tôi."

  items:
    # items loop
    - number: "50+"
      title: "Các định dạng được hỗ trợ"
      content: "Chúng tôi hỗ trợ hơn 50 định dạng tài liệu được sử dụng rộng rãi nhất."

    # items loop
    - number: "650k"
      title: "Tải xuống NuGet"
      content: "GroupDocs.Assembly cho .NET là thư viện phổ biến với hơn 650,000 lượt tải trên NuGet."

    # items loop
    - number: "18k"
      title: "Tải xuống Maven"
      content: "Các nhà phát triển Java đã tải GroupDocs.Assembly trên Maven hơn 18,000 lần."

    # items loop
    - number: "150+"
      title: "Khách hàng Hài lòng"
      content: "Các sản phẩm của chúng tôi được các nhà phát triển cá nhân và các công ty hàng đầu trên toàn thế giới tin tưởng để tạo ra các giải pháp đổi mới."


############################# Customers ###############################
customers:
  enable: true
  title: "Khách hàng Hài lòng của Chúng tôi"
  description: "Thư viện GroupDocs được sử dụng bởi một số thương hiệu danh tiếng và được tôn trọng nhất trên toàn cầu."

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
  title: "Bạn đã sẵn sàng bắt đầu chưa?"
  description: "Kiểm tra các tính năng của GroupDocs.Assembly miễn phí trên nền tảng của bạn."

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
  title: "Các câu hỏi thường gặp"
  description: "Duyệt qua các câu hỏi thường gặp."

  items:
    # items loop
    - question: "GroupDocs.Assembly có yêu cầu bất kỳ thư viện bên ngoài nào cho việc soạn thảo tài liệu không?"
      answer: "Không, GroupDocs.Assembly hoạt động độc lập và không yêu cầu các thư viện bên thứ ba như Adobe Acrobat hoặc Microsoft Office."

    # items loop
    - question: "Tôi có thể thử nghiệm các tính năng của GroupDocs.Assembly trước khi mua không?"
      answer: "Có, bạn có thể! GroupDocs.Assembly cung cấp bản dùng thử miễn phí. Cài đặt nó và khám phá các tính năng của nó. Phiên bản dùng thử thêm 'nhãn thử nghiệm' vào tài liệu của bạn và chỉ xử lý 3 trang đầu tiên. Để trải nghiệm đầy đủ, hãy nhận một giấy phép tạm thời miễn phí 30 ngày để truy cập tất cả các tính năng. Thông tin chi tiết có sẵn trong [giấy phép tạm thời](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Các loại giấy phép nào có sẵn?"
      answer: "Đang tìm giấy phép GroupDocs.Assembly? Chúng tôi cung cấp nhiều tùy chọn khác nhau để phù hợp với nhu cầu của bạn. Chọn dựa trên kích thước nhóm của bạn, vị trí triển khai (văn phòng riêng hoặc từ xa) và liệu bạn có cần chia sẻ SDK/API với khách hàng để phân phối hay không. Ngoài ra, hãy chọn giấy phép sử dụng hàng tháng với các kế hoạch theo mức sử dụng — chỉ trả tiền cho những gì bạn sử dụng. Tìm tùy chọn tốt nhất cho bạn trong phần [giá](https://purchase.groupdocs.com/pricing/assembly/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "API Low-Code của GroupDocs.Assembly"
  description: "Tạo tài liệu bằng cách sử dụng ứng dụng của bạn thông qua API REST dựa trên đám mây của chúng tôi."
  
  items:
    # items loop
    - title: "GroupDocs.Assembly Cloud for cURL"
      content: "Sử dụng API RESTful cURL để thêm dữ liệu vào Word, Excel, PowerPoint và nhiều mẫu khác."
      icon: "groupdocs_assembly-for-curl"
      link: "https://products.groupdocs.cloud/assembly/curl"

    # items loop
    - title: "GroupDocs.Assembly Cloud for .NET"
      content: "Nâng cao ứng dụng .NET của bạn bằng cách tạo báo cáo thông qua SDK Đám mây. Hiển thị dữ liệu doanh nghiệp theo định dạng tùy chỉnh của bạn."
      icon: "groupdocs_assembly-for-net"
      link: "https://products.groupdocs.cloud/assembly/net"

    # items loop
    - title: "GroupDocs.Assembly Cloud for Java"
      content: "SDK GroupDocs.Assembly cung cấp nhiều tùy chọn cho các ứng dụng Java để tạo nhiều loại tài liệu khác nhau."
      icon: "groupdocs_assembly-for-java"
      link: "https://products.groupdocs.cloud/assembly/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Ứng dụng Web GroupDocs.Assembly"
  description: "GroupDocs.Assembly cung cấp một ứng dụng web miễn phí để tạo tài liệu. Bạn có thể xử lý hơn 50 định dạng tệp phổ biến trực tiếp trong trình duyệt của mình, MIỄN PHÍ."

  items:
    # items loop
    - title: "GroupDocs.Assembly Total"
      content: "Tạo báo cáo trong Excel, Word, PowerPoint và nhiều loại tệp khác trực tiếp từ trình duyệt web của bạn."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/assembly/total"

    # items loop
    - title: "GroupDocs.Assembly Word"
      content: "Tạo tài liệu Microsoft Word từ các mẫu và nguồn dữ liệu."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/assembly/docx"

    # items loop
    - title: "GroupDocs.Assembly Excel"
      content: "Tải lên một mẫu và một nguồn dữ liệu để tạo báo cáo Excel miễn phí."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/assembly/xlsx"


      


---