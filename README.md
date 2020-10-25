Lên trang chủ của Anaconda, tải bản cập nhật mới nhất
https://docs.conda.io/en/latest/miniconda.html
Lưu ý trong quá trình cài đặt, nhớ chọn 2 option này để tạo biến môi trường trong windown.

Mở Command Prompt or Windown PowerShell trong thư mục code chạy các lệnh sau:
- pip install -U -r requirements.txt
- pip install torch==1.6.0+cu101 torchvision==0.7.0+cu101 -f https://download.pytorch.org/whl/torch_stable.html
Để cài đặt tất cả các thư viện cần thiết được nêu ở đầu mục 3.3.2
* Sau khi cài đặt tất cả:
Để chạy app với đầu vào là link RTSP
- python track.py --save-txt
Để chạy app với đầu vào là video
- python track.py --source test1.mp4 --save-txt
Với test1.mp4 là tên video bỏ vào cùng đường dẫn với file track.py trong project.
Tắt màn hình hiển thị video bằng phím tắt ‘Q’ để lưu thông tin output vào file.
Sau khi chạy hoàn tất, thông tin thu thập được sẽ được lưu trong đường dẫn
