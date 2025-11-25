# Jupyter lab cơ bản
## Sử dụng kernel
Dùng lệnh trong terminal:
- Để xem các kernel đã cài,
```
jupyter kernelspec list
```
- Để xoá kernel đó khỏi hệ thống.
```
jupyter kernelspec uninstall tên_kernel_cần_xoá
```
- Cài đặt kernel mới cho môi trường Python hiện tại bằng:
```
python -m ipykernel install --user --name tên_kernel_mới --display-name "Tên hiển thị"
```
