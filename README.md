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

---

*Lưu ý:* Trên macOS, sử dụng `python3` để đảm bảo gọi đúng phiên bản Python 3 vì Python 2 có thể vẫn tồn tại trên hệ thống.

---




