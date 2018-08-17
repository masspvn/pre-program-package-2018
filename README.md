# pre-program-package-2018
Tài liệu gửi trước chuẩn bị cho chương trình Trại hè Toán và Khoa học MaSSP 2018 được chuẩn bị bởi nhóm mentors môn Tin học MaSSP 2017 và 2018.

Chủ đề của môn Tin học năm 2018 là Giới thiệu bộ môn Khoa học Dữ liệu (Data Science) và Máy học (Machine Learning).

Chắc hẳn các ngành học này còn khá mới lạ với các bạn. Sau đây là những tài liệu có thể giúp bạn tìm hiểu sơ qua về những ứng dụng của các ngành học này.

1. [The best stats you've ever seen - Hans Rosling](https://www.ted.com/talks/hans_rosling_shows_the_best_stats_you_ve_ever_seen/transcript ) (có phụ đề tiếng Việt). Trang web tương tác đi kèm video này: http://www.shichaoji.com/home-page/
2. [Machine Learning là gì? | Vũ Hữu Tiệp](http://machinelearningcoban.com/2016/12/26/introduce/)
3. [How we teach computers to understand pictures - Fei Fei Li](https://www.ted.com/talks/fei_fei_li_how_we_re_teaching_computers_to_understand_pictures/transcript) (có phụ đề tiếng Việt).

Ngôn ngữ lập trình được dùng chủ yếu trong khoá học là Python 3, vì thế các bạn có thể tìm trong tài liệu gửi trước này tutorial giới thiệu ngôn ngữ Python. Ngoài ra, các bạn sẽ được làm quen với một số thư viện thông dụng trong Python: numpy, matplotlib, và pandas. Những thư viện này được sử dụng rộng rãi cho việc minh hoạ dữ liệu (data visualization) và thống kê mô tả (descriptive statistics) - những bước không thể thiếu khi khám phá một bộ dữ liệu lớn và phức tạp.

Nhưng trước hết, các bạn hãy làm theo hướng dẫn sau để cài đặt những công cụ cần thiết. Các bạn cần biết dùng [giao diện dòng lệnh](https://www.codehub.vn/Command-line-co-ban-cho-nguoi-moi-bat-dau) (Command Line Interface hay CLI) trên Terminal. Tuỳ hệ điều hành của máy tính của bạn mà các bước sau có thể khác nhau một chút. Vì vậy, đừng ngại hỏi mentor nếu có vướng mắc! Facebook group: [MaSSP Tin](https://www.facebook.com/groups/183191748970952/).

## 1. Github
### 1.1. Tìm hiểu về Git
Git là một trong những `hệ thống quản lý phiên bản code phân tán`, vốn được phát triển nhằm quản lý mã nguồn (source code). Một số bài giới thiệu về tham chiếu Git và Github bằng tiếng Việt: của [Mark Lodato & Hoat Le](http://marklodato.github.io/visual-git-guide/index-vi.html), blog của [Dỗ Minh Hải](https://dominhhai.github.io/vi/categories/git/), [Git-SCM](https://git-scm.com/book/vi/v1/Bắt-Đầu-Cơ-Bản-về-Git), etc.
### 1.2. Cài đặt Git
Làm theo chỉ dẫn của phần Setting Up Git: https://help.github.com/articles/set-up-git/#setting-up-git
### 1.3. Kiểm tra
Từ command shell của Git, nhập lệnh clone repo của massp. Nếu thành công, một thư mục `pre-program-package-2018` sẽ được tạo ra
```
~/MaSSP $ git clone https://github.com/masspvn/pre-program-package-2018.git
```
Nếu có sự cố khi cài đặt, hãy hỏi mentors và trong câu hỏi ghi rõ đang ở bước nào và kèm screenshot. Bạn có thể làm các bước 1-4 trong phần tiếp theo mà không cần đến Git.
## 2. Anaconda, Python
### 2.1. Cài đặt Anaconda

Tải file cài Anaconda cho Python 3 tại https://www.continuum.io/downloads, ví dụ Anaconda3-4.2.0-Windows-x86_64.exe, và cài đặt theo chỉ dẫn. Chọn "allow add to path and use Anaconda as default Python" nếu được hỏi.
### 2.2. Tạo môi trường

Với hệ điều hành Windows, khi cài xong, từ Start Menu mở chương trình Anaconda Prompt. Tiếp đó, tạo một thư mục để chứa tài liệu trong trại hè, ví dụ `~/MaSSP`:
```
~/ $ mkdir MaSSP
```
Chạy lệnh sau đây để tạo môi trường `datascience` với Python 3.5 và Jupyter notebook:
```
~/MaSSP $ conda create -n datascience python=3.5 jupyter
```
Gõ “y” và Enter nếu được hỏi `Proceed ([y]/n)?`

### 2.3. Kích hoạt môi trường
```
~/MaSSP $ activate datascience
```
Nếu lệnh trên không được, thử `source activate datascience`.

### 2.4. Cài các thư viện cần thiết vào môi trường

Để bắt đầu, chúng ta cần 2 thư viện matplotlib và numpy.
```
(datascience) ~/MaSSP $  conda install matplotlib
(datascience) ~/MaSSP $  conda install numpy
```
### 2.5. Khởi động Jupyter notebook

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

### 2.6. Kiểm tra cài đặt

Thử tạo một notebook mới: Nhấn nút “New” ở góc trên bên phải màn hình và chọn “Python 3” ở dưới “Notebooks” như hình ảnh sau. Một notebook có tên Untitled sẽ được tạo ra.

![tạo notebook](/images/create_new_notebook.png)

Thử numpy và matplotlib: trong notebook vừa tạo, gõ lệnh import sau và nhấn `Shift + Enter`. Nếu không thấy lỗi nào hiện ra thì quá trình cài đặt đã hoàn thành.

![thử numpy và matplotlib](/images/verify_numpy_matplotlib.png)

## 3. Tutorials
Mọi ý kiến/thắc mắc/phát hiện lỗi sai, hãy post lên Facebook group hoặc gửi email cho mentor!
### 3.1. Jupyter notebook
Các bạn hãy xem video hướng dẫn cách sử dụng Jupyter notebook: [phần 1](https://www.youtube.com/watch?v=vYAvS97jqN8&t=0s&list=PLqOu9En69v830W527rOX__3v23eZIqGCH) và [phần 2](https://www.youtube.com/watch?v=8zb0u782AsQ&t=4s&list=PLqOu9En69v830W527rOX__3v23eZIqGCH). Lúc này, kể cả khi bạn chưa biết sử dụng Python, hãy vẫn cố làm theo các thao tác trong video nhé!

### 3.2. Python
Nếu bạn chưa từng sử dụng Python, hãy đọc và thử các lệnh trong notebook `Learn_Python.ipynb` để làm quen với các câu lệnh đơn giản.

Ngoài ra, còn rất nhiều tài liệu hay khác để bắt đầu với Python, ví dụ lớp miễn phí của ĐH KHTN HCM trên vnsigma (http://vnsigma.net/), lớp học online của University of Michigan subtitled bởi Kiến Học: Python [cơ bản](http://study.kienhoc.vn/courses/course-v1:UMICH+CS101+2016_T3/about) và [nâng cao](http://study.kienhoc.vn/courses/course-v1:UMICH+CS201+2016_T3/about). Tutorials in English: [CS231](http://cs231n.github.io/python-numpy-tutorial/).

### 3.3. Pandas
Trong notebook `Learn_Pandas.ipynb`, các bạn sẽ học được một số câu lệnh thường dùng trong Pandas. Cuối mỗi phần thường có các `checkpoint`, đó là những bài tập nhỏ các bạn nên hoàn thiện trước khi đi tiếp các phần sau. Sau khi hoàn thành notebook, hãy thử vẽ một số đồ thị tuỳ thích dựa theo những số liệu có thật và chia sẻ lên Facebook group [MaSSP Tin](https://www.facebook.com/groups/183191748970952/) để mọi người cùng biết nhé!

Sau đây là một số những trang web có thể tìm thấy số liệu thống kê:
- https://www.kaggle.com/
- https://www.gso.gov.vn/
- https://www.data.gov/
- https://data.gov.uk/
- https://data.gov.sg/
- https://data.worldbank.org/
- http://data.go.id/

### 3.4. LaTEX (tự chọn)
Các bạn có thể tham khảo tài liệu `Intro to LaTEX.pdf` soạn thảo bởi anh Hồ Đức - mentor nhóm Toán để tìm hiểu cách sử dụng LaTEX trên trang https://www.overleaf.com/. Ngoài ra, còn rất nhiều tài liệu hay khác như http://math2it.com/tu-hoc-latex-bai-tong-hop/, và [loạt video về LaTEX](https://www.youtube.com/watch?v=Qc82mJTDzt8&index=2&list=PLlsF2nDmyL7msihnebzII_KVWy6URxDfp) của anh Vũ Hữu Tiệp (cùng source code trên [Github](https://github.com/tiepvupsu/LatexBasics)).
