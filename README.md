# pre-program-package-2018
Tài liệu gửi trước chuẩn bị cho chương trình Trại hè Toán và Khoa học MaSSP 2018.
## Github
### 1. Cài đặt Git
Làm theo chỉ dẫn của phần Setting Up Git: https://help.github.com/articles/set-up-git/#setting-up-git
### 2. Kiểm tra
Từ command shell của Git, nhập lệnh clone repo của massp. Nếu thành công, một thư mục `pre-program-package-2018` sẽ được tạo ra
```
~/MaSSP $ git clone https://github.com/masspvn/pre-program-package-2018.git 
```
Đừng ngại hỏi mentor nếu bước này không thành công!

## Anaconda, Python
### 1. Cài đặt Anaconda

Tải file cài Anaconda cho Python 3 tại https://www.continuum.io/downloads, ví dụ Anaconda3-4.2.0-Windows-x86_64.exe, và cài đặt theo chỉ dẫn. Chọn "allow add to path and use Anaconda as default Python" nếu được hỏi.
### 2. Tạo môi trường

Với hệ điều hành Windows, khi cài xong, từ Start Menu mở chương trình Anaconda Prompt. Tiếp đó, tạo một thư mục để chứa tài liệu trong trại hè, ví dụ `~/MaSSP`:
```
~/ $ mkdir MaSSP
```
Chạy lệnh sau đây để tạo môi trường `datascience` với Python 3.5 và Jupyter notebook:
```
~/MaSSP $ conda create -n datascience python=3.5 jupyter
```
Gõ “y” và Enter nếu được hỏi `Proceed ([y]/n)?`

### 3. Kích hoạt môi trường
```
~/MaSSP $ activate datascience
```
Nếu lệnh trên không được, thử `source activate datascience`.

### 4. Cài các thư viện cần thiết vào môi trường

Để bắt đầu, chúng ta cần 2 thư viện matplotlib và numpy.
```
(datascience) ~/MaSSP $  conda install matplotlib
(datascience) ~/MaSSP $  conda install numpy
```
### 5. Khởi động Jupyter notebook

Tải repo sau từ GitHub của MaSSP
``` 
~/MaSSP $ git clone https://github.com/masspvn/pre-program-package-2018.git  
```
Từ Anaconda Prompt, khởi động Jupyter notebook
```
(datascience) ~/MaSSP$ cd pre-program-package-2018
(datascience) ~/MaSSP/pre-program-package-2018 $ jupyter notebook
```
Nếu một session của Jupyter notebook không tự động bắt đầu trên trình duyệt, copy đường link nhận được trong terminal và mở bằng trình duyệt. Đường link này thường bắt đầu với “http://localhost:XXXX”. Tại đường link này, bạn sẽ thấy một số tài liệu của chương trình. Trước khi đọc những tài liệu này, hãy kiểm tra xem các bước cài trên đã thành công chưa.

### 6. Kiểm tra cài đặt

Thử tạo một notebook mới: Nhấn nút “New” ở góc trên bên phải màn hình và chọn “Python 3” ở dưới “Notebooks” như hình ảnh sau. Một notebook có tên Untitled sẽ được tạo ra.

![tạo notebook](/images/create_new_notebook.png)
	
Thử numpy và matplotlib: trong notebook vừa tạo, gõ lệnh import sau và nhấn `Shift + Enter`. Nếu không thấy lỗi nào hiện ra thì quá trình cài đặt đã hoàn thành.

![thử numpy và matplotlib](/images/verify_numpy_matplotlib.png)

## Tutorials
### 1. Jupyter notebook, Python, Pandas
Các bạn hãy xem video hướng dẫn cách sử dụng Jupyter notebook: [phần 1](https://www.youtube.com/watch?v=6JeSric40N0) và [phần 2](https://www.youtube.com/watch?v=BY2V1wxGFy4).
Sau đó, các bạn hãy đọc và thử các lệnh trong notebook `Learn_Python.ipynb` để làm quen với Python.

Ngoài ra, còn rất nhiều tài liệu hay khác để bắt đầu với Python, ví dụ lớp miễn phí của ĐH KHTN HCM trên vnsigma (http://vnsigma.net/), lớp học online của University of Michigan subtitled bởi Kiến Học: Python ![cơ bản](http://study.kienhoc.vn/courses/course-v1:UMICH+CS101+2016_T3/about) và ![nâng cao](http://study.kienhoc.vn/courses/course-v1:UMICH+CS201+2016_T3/about). 

Mọi ý kiến/thắc mắc hãy post lên Facebook group hoặc gửi email cho mentor.
Nếu có sự cố khi cài đặt, hãy hỏi mentors và trong câu hỏi ghi rõ đang ở bước nào và kèm screenshot.

### 2. LaTEX (tự chọn)
Các bạn có thể tham khảo tài liệu `Intro to LaTEX.pdf` soạn thảo bởi anh Hồ Đức - mentor nhóm Toán để tìm hiểu cách sử dụng LaTEX trên trang https://www.overleaf.com/. Ngoài ra, còn rất nhiều tài liệu hay khác như http://math2it.com/tu-hoc-latex-bai-tong-hop/, và ![loạt video về LaTEX](https://www.youtube.com/watch?v=Qc82mJTDzt8&index=2&list=PLlsF2nDmyL7msihnebzII_KVWy6URxDfp) của anh Vũ Hữu Tiệp.


