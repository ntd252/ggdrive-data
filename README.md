# ggdrive-data
Giải pháp cứu dữ liệu Google Drive tạm thời của timetokill87 (https://www.reddit.com/u/timetokill87/s/kYvelZXAFS)
 
Sự cố mất dữ liệu được cho là gây ra bởi bản cập nhật Google Drive client trên máy tính gần đây, khiến bộ nhớ đệm (cache) của ứng dụng bị đặt lại. Bộ nhớ đệm này lưu trữ các file đang chờ để được đồng bộ lên bộ nhớ đám mây, tuy nhiên chưa kịp đồng bộ xong đã bị bản cập nhật của ứng dụng GG Drive xóa đi. Do đó giải pháp tạm thời là cài lại ứng dụng Google Drive client bản cũ hơn.
 
Trình tự thao tác:
1. Gỡ Google Drive
2. Cài bản Google Drive cũ hơn (bản số 82/83)
3. Tắt 2 dịch vụ Google Update trong Services
4. Tắt tác vụ Google Update trong Task Scheduler
5. Đảm bảo Google Drive không chạy ở trong danh sách Processes của Task Manager
6. Tìm thư mục có dãy số dài trong thư mục bộ nhớ đệm DriveFS
Windows: %USERPROFILE%\AppData\Local\Google\DriveFS
macOS: ~/Library/Application Support/Google/DriveFS
7. Trong thư mục ở bước 6, tìm một thư mục khác có tên "Backups". Trong Backups, lại có 1 thư mục có tên dài. Di chuyển toàn bộ dữ liệu ở trong này ra ngoài thư mục ở bước 6
8. Bật Google Drive
9. Mở thư mục Google Drive trong File Explorer hoặc Finder để xem có thấy dữ liệu gần đây mà bị mất không. Nếu có thì copy ra ngoài
10. Không dùng Google Drive cho đến khi có bản cập nhật sử lỗi
From <https://www.reddit.com/r/DataHoarder/comments/1854w2n/google_drive_appears_to_have_lost_some_of_its/>
