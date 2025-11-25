# Python Cheat Sheet cơ bản cho macOS

## 1. Quản lý môi trường ảo (Virtual Environment)

- Tạo môi trường ảo:
```
python3 -m venv <tên_môi_trường>
```
Ví dụ: `python3 -m venv myenv`
- Kích hoạt môi trường ảo:
```
source <tên_môi_trường>/bin/activate
```
Ví dụ: `source myenv/bin/activate`  
Sau khi kích hoạt, bạn thấy tên môi trường ở đầu dòng terminal.

- Hủy kích hoạt môi trường ảo:
```
deactivate
```
- Xóa môi trường ảo:
- Chỉ cần xóa folder môi trường, ví dụ: 
```
rm -rf <tên_môi_trường>
```
Ví dụ: `rm -rf myenv`

## 2. Cài đặt và quản lý gói Python với pip

- Cài gói mới:
```
pip install <tên_gói>
```
Ví dụ: `pip install numpy`

- Ghi danh sách gói hiện tại ra file requirements.txt:
```
pip freeze > requirements.txt
```

- Cài gói từ file requirements.txt:
```
pip install -r requirements.txt
```

## 3. Cài đặt hoặc quản lý Python trên macOS

- Cài Python mới (nên dùng Homebrew):
```
brew install python
```

- Kiểm tra phiên bản Python:
```
python3 --version
```
- Cập nhật pip:
```
pip install --upgrade pip
```
## 4. Kiểm tra pip đang trỏ vào môi trường ảo
- Lệnh xem đường dẫn thực thi của pip:
```
which pip
```
Kết quả nên nằm trong thư mục môi trường ảo, ví dụ `/path/to/myenv/bin/pip`

- Lệnh xem đường dẫn thực thi của python:
```
which python
```
Kết quả cũng nên nằm trong thư mục môi trường ảo, ví dụ `/path/to/myenv/bin/python`

## 5. Hiển thị phiên bản pip hiện hành để xác nhận pip trong môi trường ảo
```
pip --version
```
Kết quả sẽ hiển thị đường dẫn của pip kèm theo version, ví dụ:
pip 23.0.1 from /path/to/myenv/lib/python3.x/site-packages/pip (python 3.x)

## 6. Hiển thị danh sách các gói đã cài trong môi trường ảo
```
pip list
```
Chỉ hiện các gói được cài trong môi trường ảo hiện tại. Các gói hệ thống sẽ không hiển thị.

## 7. Lưu ý thêm

- Khi môi trường ảo chưa được kích hoạt, pip sẽ trỏ đến pip của hệ thống, bạn có thể xác định bằng `which pip` không nằm trong thư mục môi trường ảo.
- Luôn kiểm tra bằng lệnh `which pip` và `which python` để đảm bảo bạn đang thao tác đúng với môi trường ảo.
- Cài đặt gói sau khi kích hoạt môi trường để gói đó nằm trong môi trường ảo, không ảnh hưởng đến hệ thống toàn cục.


*Lưu ý:* Trên macOS, sử dụng `python3` để đảm bảo gọi đúng phiên bản Python 3 vì Python 2 có thể vẫn tồn tại trên hệ thống.

---




