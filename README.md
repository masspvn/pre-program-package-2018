# pre-program-package-2018
Tài liệu gửi trước chuẩn bị cho chương trình Trại hè Toán và Khoa học MaSSP 2018.
## Github
Vào đây làm theo chỉ dẫn của phần Setting Up Git https://help.github.com/articles/set-up-git/#setting-up-git
Kiểm tra
Từ command shell của Git, nhập lệnh clone repo của massp. Nếu thành công, một thư mục "pre-program-package-2018" sẽ được tạo ra
D:\MaSSP\physics\$ git clone https://github.com/masspvn/pre-program-package-2018.git 
Hỏi mentor nếu bước này không thành công.

## Anaconda, Python
Vào trang https://www.continuum.io/downloads 
Download setup file Anaconda cho Python 3, 
Windows 64-bit (ví dụ Anaconda3-4.2.0-Windows-x86_64.exe)
Chạy setup file, allow add to path and use Anaconda as default Python
Khi cài xong, từ Start Menu nếu dùng Windows mở Anaconda Prompt
Tạo một thư mục để chứa tài liệu trong trại hè, ví dụ D:\MaSSP\
D:\ $ mkdir MaSSP
Chạy command sau đây để tạo environment “datascience” với Python 3.5 và Jupyter notebook được cài theo
D:\MaSSP\$ conda create -n datascience python=3.5 jupyter
Gõ “y” và Enter nếu được hỏi “Proceed ([y]/n)?”
Activate environment
D:\MaSSP\$ activate datascience
Nếu lệnh trên không được, thử “source activate datascience”
prompt sẽ trở thành “(datascience) D:\MaSSP$” - ta đang ở trong environment có tên “datascience”
Cài matplotlib package vào environment
(datascience) D:\MaSSP$  conda install -c conda-forge matplotlib=2.0.2
Clone repo từ GitHub  - Bỏ qua nếu đã clone pre-program-package từ lúc setup GitHub
D:\MaSSP\ $ git clone https://github.com/masspvn/pre-program-package-2018.git  
Từ Anaconda Prompt, khởi động Jupyter notebook
D:\MaSSP$ cd pre-program-package
D:\MaSSP\pre-program-package$ jupyter notebook
Nếu một session của Jupyter notebook không tự động bắt đầu trên trình duyệt, copy đường link nhận được trong terminal và mở bằng trình duyệt. Đường link này thường bắt đầu với “http://localhost:XXXX”. Bạn sẽ thấy một số tutorials trong này.
	
Thử tạo một notebook mới: Nhấn nút “New” ở góc trên bên phải màn hình và chọn “Python 3” ở dưới “Notebooks” như hình ảnh sau. Một notebook có tên Untitled sẽ được tạo ra.
	
Thử numpy và matplotlib: trong notebook vừa tạo, gõ lệnh import sau và nhấn Shift + Enter. Nếu không thấy lỗi nào hiện ra thì quá trình cài đặt đã hoàn thành.

Python tutorial
Các bạn hãy đọc và thử các lệnh trong notebook Learn_Python.ipynb trước khi trại hè diễn ra. Notebook Linear_Algebra.ipynb nói về định nghĩa của vector, ma trận, và các phương pháp biến đổi, nhưng không quá cần thiết cho chương trình năm nay. Tuy nhiên các bạn có thể làm thử một số bài tập để làm quen hơn với thư viện numpy.
Mọi ý kiến/thắc mắc hãy post lên fb hoặc gửi email cho mentor.
Nếu có sự cố khi cài đặt, hãy hỏi mentors và trong câu hỏi ghi rõ đang ở bước nào và kèm screenshot.


