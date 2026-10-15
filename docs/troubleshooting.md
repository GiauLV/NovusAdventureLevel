# Xử lý lỗi

## Plugin không enable

- Xác nhận JAR đặt trực tiếp trong `plugins/`.
- Kiểm tra tương thích `api-version: '1.21'` và Java runtime; JAR được build bằng Java 21.
- Đọc toàn bộ log enable/stack trace.

## Placeholder không hoạt động

- Xác nhận PlaceholderAPI đã được nạp.
- Thử `/papi parse <player> %novusal_level%`.
- Kiểm tra identifier chính xác là `novusal`.

## Không nhận AE khi giết mob

- Kiểm tra `settings.enabled` trong `mob-rewards.yml`.
- Bật tích hợp phù hợp (`mythicmobs.enabled` hoặc `levelledmobs.enabled`).
- Xác nhận entity type/internal ID/level, `settings.priority`, `prevent-duplicate-rewards` và `recipients`.

## Bí Cảnh chưa sẵn sàng

- Chạy `/adbc info <id>`.
- Xác nhận `enabled: true`, điểm vào và điểm spawn mob đã đặt.
- Kiểm tra ID mob, cổng AL, wave, hình phạt và các điểm `diem1`…`diem10`.
- Chạy `/adbc reload`, đọc log rồi thử `/adbc test <id>` trên staging.

## Cấu hình không cập nhật

- Chỉnh đúng file cấu hình runtime, không phải bản tham khảo trong repository.
- Dùng `/capmaohiem reload` hoặc `/adbc reload` phù hợp.
- Kiểm tra YAML indentation và kiểu boolean/số. Sao lưu trước khi sửa.

## Báo lỗi

Đính kèm phiên bản plugin, Paper/Minecraft, `java -version`, danh sách phụ thuộc, log console và cấu hình tối thiểu để tái hiện. Loại bỏ token, mật khẩu và dữ liệu riêng tư.