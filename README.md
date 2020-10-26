- Lên trang chủ của Anaconda, tải bản cập nhật mới nhất: https://docs.conda.io/en/latest/miniconda.html
- Lưu ý trong quá trình cài đặt, nhớ chọn 2 option này để tạo biến môi trường trong windown.

* Mở Command Prompt or Windown PowerShell trong thư mục code chạy các lệnh sau:
- pip install -U -r requirements.txt
- pip install torch==1.6.0+cu101 torchvision==0.7.0+cu101 -f https://download.pytorch.org/whl/torch_stable.html 
(Để cài đặt tất cả các thư viện cần thiết được nêu ở đầu mục 3.3.2)

* Sau khi cài đặt tất cả có 2 chế độ để chạy app:
1) Để chạy app với đầu vào là link RTSP
- python track.py --save-txt
2) Để chạy app với đầu vào là video
- python track.py --source test1.mp4 --save-txt

**NOTE**
Với test1.mp4 là tên video bỏ vào cùng đường dẫn với file track.py trong project.
Tắt màn hình hiển thị video bằng phím tắt ‘Q’ để lưu thông tin output vào file.
Sau khi chạy hoàn tất, thông tin thu thập được sẽ được lưu trong đường dẫn


download the yolov5 weight from https://drive.google.com/drive/folders/1Drs_Aiu7xx6S-ix95f9kNsA6ueKRpN2J. Place the downlaoded .pt file under yolov5/weights/
download the deep sort weights from https://drive.google.com/drive/folders/1xhG0kRH1EX5B9_Iz8gQJb7UNnn_riXi6. Place ckpt.t7 file underdeep_sort/deep/checkpoint/