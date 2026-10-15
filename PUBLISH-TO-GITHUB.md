# Hướng dẫn duy trì repository

Repository hiện đặt tài liệu trong `docs/` để tài liệu được version cùng plugin.

## Phát hành bản mới

1. Xác nhận bạn có quyền phân phối JAR.
2. Đưa JAR phiên bản mới vào mục **Releases** dưới dạng release asset.
3. Tạo tag theo phiên bản, ví dụ `v1.1.1`.
4. Dùng file tương ứng trong `release-notes/` làm ghi chú phát hành.
5. Cập nhật checksum SHA-256 theo file nhị phân thực tế.
6. Kiểm tra lại README, docs, cấu hình và cách cài trên server staging.

## GitHub Wiki

Các trang trong `docs/` là Markdown bình thường. Nếu bật GitHub Wiki riêng, có thể sao chép các trang cần thiết sang Wiki; nội dung ở `docs/` không tự đồng bộ sang Wiki.

## Trạng thái binary hiện tại

Kết nối xuất bản được dùng trong phiên này chỉ cung cấp thao tác tạo/cập nhật file văn bản, không có thao tác upload binary Release asset trực tiếp. Vì vậy JAR chưa được tải lên GitHub bởi tiến trình này; hãy đính kèm `artifacts/NovusAdventureLevel-1.1.1.jar` thủ công ở trang Releases hoặc dùng Git trên máy đã đăng nhập GitHub để commit file nhị phân. Không đánh dấu release hoàn tất trước khi xác minh asset.
