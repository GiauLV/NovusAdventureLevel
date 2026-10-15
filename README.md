# NovusAdventureLevel

Plugin Minecraft cung cấp hệ thống Adventure Level (AL), Điểm Thám Hiểm (AE), chỉ số, danh hiệu và Bí Cảnh Đột Phá.

> **Phiên bản được tài liệu hóa:** 1.1.1  
> **Java build:** 21  
> **API mục tiêu trong metadata JAR:** Paper API 1.21

## Trạng thái phát hành

Tài liệu và các file cấu hình mặc định đã được đưa vào repository. **JAR chưa được đính kèm trên GitHub** vì kết nối xuất bản hiện tại không hỗ trợ tải lên binary Release asset. Không có Release tải xuống nào được tạo ở thời điểm này.

File JAR gốc trong gói làm việc có tên `NovusAdventureLevel-1.1.1.jar`. Để hoàn tất phát hành công khai, hãy đính kèm file này trong **Releases** và xác minh asset sau khi tải lên.

## Cài đặt

Sau khi JAR được đính kèm vào Release:

1. Dừng máy chủ Minecraft.
2. Tải `NovusAdventureLevel-1.1.1.jar` từ trang [Releases](../../releases).
3. Đặt JAR vào thư mục `plugins/`.
4. Khởi động máy chủ và kiểm tra console.
5. Sao lưu cấu hình trước khi thay đổi các file do plugin tạo ra.

## Lệnh

| Lệnh | Chức năng |
|---|---|
| `/capmaohiem` | Mở GUI Cấp Mạo Hiểm |
| `/bicanh` | Mở GUI Bí Cảnh Đột Phá |
| `/adminbicanh` / `/adbc` | Quản trị Bí Cảnh |

Xem [tài liệu lệnh chi tiết](docs/commands.md) và [permissions](docs/permissions.md).

## Tài liệu

- [Mục lục tài liệu](docs/README.md)
- [Cài đặt và nâng cấp](docs/installation.md)
- [Lệnh](docs/commands.md)
- [Permissions](docs/permissions.md)
- [PlaceholderAPI](docs/placeholders.md)
- [Cấu hình](docs/configuration.md)
- [Bí Cảnh Đột Phá](docs/bicanh.md)
- [Phần thưởng AE từ mob](docs/mob-rewards.md)
- [Tích hợp plugin khác](docs/integrations.md)
- [API dành cho developer](docs/api.md)
- [Xử lý sự cố](docs/troubleshooting.md)
- [Cấu hình YAML mặc định](defaults/)
- [Ghi chú v1.1.1](release-notes/v1.1.1.md)
- [Hướng dẫn duy trì/phát hành](PUBLISH-TO-GITHUB.md)

## Giấy phép

Repository hiện có [LICENSE](LICENSE) theo MIT. Trước khi phát hành binary công khai, hãy xác nhận bạn có quyền phân phối JAR và MIT thực sự áp dụng cho phần mềm được phát hành. Chỉ có file LICENSE trong repository không tự chứng minh quyền sở hữu hoặc quyền phân phối của binary.
