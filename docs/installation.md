# Cài đặt và nâng cấp

## Yêu cầu

- Minecraft/Paper API tương thích với `api-version: '1.21'` trong plugin.yml.
- JAR được build bằng Java 21; khuyến nghị chạy server bằng Java 21.
- Các tích hợp như PlaceholderAPI, MythicMobs, LevelledMobs và MythicLib chỉ cần khi dùng tính năng liên quan.

## Cài đặt

1. Dừng máy chủ.
2. Sao lưu thư mục `plugins/` và dữ liệu server.
3. Đặt `NovusAdventureLevel-1.1.1.jar` trực tiếp vào `plugins/`.
4. Khởi động server và kiểm tra log nạp plugin.
5. Xác nhận các file cấu hình được tạo, sau đó chỉnh cấu hình trên bản test trước khi triển khai.

## Nâng cấp

1. Dừng server và sao lưu thư mục dữ liệu plugin.
2. Thay JAR cũ bằng bản mới; tránh để hai bản JAR cùng tồn tại.
3. Khởi động server, kiểm tra log và rà soát thay đổi cấu hình trước khi mở server cho người chơi.

Không xóa dữ liệu người chơi để xử lý lỗi khởi động. Lưu ý: cấu hình mặc định nằm trong `defaults/` của repository; chúng không nhất thiết giống cấu hình đã tùy chỉnh ở máy chủ đang chạy.