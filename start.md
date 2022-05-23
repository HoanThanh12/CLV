# GitHub

    - git add : Add source push GitHub
    - git commit "" : Comment
    - git push :  Push to GitHub
    - ssh-keygen -t ed25519 : Create a new ssh key
    - $ git config --global user.name "Thanh"
    - $ git config --global user.email "hoanthanh410@gmail.com"
# Framework outline

    - OPUS Container system is an application base on Synapse Framework || Là ứng dụng dựa trên Synapse Framework
    - Channel : An area for processing requests from various users coming into the OPUS Container system || Xử lý yêu cầu của khách hàng đến hệ thống
    - Biz App : An area for processes and manages the business logic || Một khu vực dành cho các quy trình và logic nghiệp vụ trong kinh doanh || Có 39 module
    - Business commmon : An area where common business logic is located || Một khu vực nơi kinh doanh phổ biến được đặt
    - System common : A collection of common functions used by Biz App and Biz Common || Các chức năng phổ biến được Biz App và Business common sử dụng
    - Connector : An area that provides functions for transmitting data from an OPUS Container to an external system || Cung cấp chức năng cho cho OPUS Container để truyền ra bên ngoài
    - Synapse Framework : Provide core classes and common functionality for systematic processing used by Biz App and Biz Common || Cung cấp các lớp cốt lõi và xử lý có hệ thống cho Biz App and Biz Common sử dụng
    - WAS : An environment for running framework and application || Là môi trường để chạy ứng dụng và framework

## Presentation Layer
 - Nhận yêu cầu và tạo requests xử lý và truyển dữ liệu yêu cầu trên màn hình

## Control Layer
 - Nó đóng vai trò như một bộ chặn cho tất cả các quy trình kinh doanh và nó đóng vai trò quản lý phiên và vai trò bộ lọc, đồng thời xác định việc tiếp tục xử lý ứng dụng bằng chính sách đăng nhập của người dùng và thông tin quyền

## Business Layer
 - Nó thực hiện quy trình nghiệp vụ theo yêu cầu công việc của người dùng và yêu cầu xử lý dữ liệu

## Integration Layer
- Nó là một lớp để giao tiếp giữa cơ sở dữ liệu và hệ thống bên ngoài, và chịu trách nhiệm gọi các dịch vụ của các thành phần nghiệp vụ khác và hệ thống bên ngoài theo yêu cầu của lớp nghiệp vụ.

## Resource Layer
- Nó là một khu vực nền tảng cung cấp các tài nguyên vật lý của hệ thống, chẳng hạn như hệ thống tệp và cơ sở dữ liệu


# Service Comment
- Để biết request đó gửi là gì, yêu cầu là gì và trả ra kết quả như thế nào

# Business Components là lớp interface
- Khai báo phương thức
# BCImpl
- Dùng để implement các phương thức nằm trong BC đó
- Tương tác đến DBDAO hoặc EAIDAO
- DBDAO dùng để tưởng tác đến database để xóa sửa thêm, ......
- EAIDAO dùng để gửi mail, máy fax, upload file,...

# HtmlAction
- perform() : perform request
- doStart()
- doEnd()

# Event
- implement từ EventSupport
- signOnUserAccount() : sign on user account and authentication and authorization
- ConditionVO : Nhận request subject
- VO Collection : Trả data cho request đó
