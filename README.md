
# Cách kích hoạt PhysBots

-Sử dụng terminal trong Visual Code Studio để kích hoạt app.py
-Website sử dụng Flask, một Web Framework, khi đó ta truy cập vào trang web qua đường dẫn này http://127.0.0.1:5000
-Sau khi giải nén tệp tin, để có thể sử dụng được PhysBots ta phải làm theo các bước sau:

## Change directory (cd) vào thư mục PhysBots

-Chuyển sang thư mục PhysBot: *cd PhysBots*
-Nếu dùng Visual Code Studio thì có thể vào File->Open Folder->PhysBots

## Create environment

-Tạo môi trường để khởi động app.py: *python -m venv .venv* hoặc *py -m venv .venv*

## Activate environment

-Kích hoạt môi trường ảo:
+Windows: *.\.venv\Scripts\activate*
(Nếu gặp lỗi về "Execution Policies", chạy: Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted
sẽ cho phép máy có quyền chạy lệnh)
+Linux: *source ./venv/bin/activate*

## Install modules using the python-pip command:

-Tải các framework cần thiết:
+tensorflow: *pip install tensorflow*
+keras: *pip install keras*
+nltk: *pip install nltk*
+flask: *pip install flask*

## Select file to activate flask

-Chọn file app.py để kích hoạt flask: *$env:FLASK_APP = "app.py"*

## Activate flask

-Khởi động flask: *flask --debug run*
(--debug: Cập nhật lại ứng dụng mỗi khi có thay đổi)
