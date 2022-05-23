# GitHub

    - git add : Add source push GitHub
    - git commit "" : Comment
    - git push :  Push to GitHub
    - ssh-keygen -t ed25519 : Create a new ssh key
    - $ git config --global user.name "Thanh"
    - $ git config --global user.email "hoanthanh410@gmail.com"
# Framework outline

    - OPUS Container system is an application base on Synapse Framework || Là ứng dụng dựa trên Synapse Framework
    - Channel : An area for processing requests from various users coming into the OPUS Container system || Sử lý yêu cầu của khách hàng đến hệ thống
    - Biz App : An area for processes and manages the business logic || Một khu vực dành cho các quy trình và logic nghiệp vụ trong kinh doanh
    - Business commmon : An area where common business logic is located || Một khu vực nơi kinh doanh phổ biến được đặt
    - System common : A collection of common functions used by Biz App and Biz Common || Các chức năng phổ biến được Biz App và Business common sử dụng
    - Connector : An area that provides functions for transmitting data from an OPUS Container to an external system || Cung cấp chức năng cho cho OPUS Container để truyền ra bên ngoài
    - Synapse Framework : Provide core classes and common functionality for systematic processing used by Biz App and Biz Common || Cung cấp các lớp cốt lõi và xử lý có hệ thống cho Biz App and Biz Common sử dụng
    - WAS : An environment for running framework and application || Là môi trường để chạy ứng dụng và framework
