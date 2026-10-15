# Tích hợp plugin khác

Các plugin tích hợp là tùy chọn theo chức năng:

| Plugin | Dùng cho |
|---|---|
| PlaceholderAPI | Cung cấp placeholder `%novusal_...%` |
| MythicMobs | Nhận diện mob, hook phần thưởng và mob Bí Cảnh |
| LevelledMobs | Quy tắc AE theo level/entity |
| MythicLib | Hook chỉ số nhân vật |
| MMOCore | Được khai báo trong soft-dependencies; hành vi cụ thể phụ thuộc cấu hình và phiên bản đang cài |

Trong `mob-rewards.yml`, thứ tự ưu tiên mặc định là `MYTHICMOBS_DROP`, `MYTHICMOBS_INTERNAL_ID`, `LEVELLEDMOBS`, `ENTITY_TYPE`, `DEFAULT`.

## Checklist tích hợp

- Thử placeholder với người chơi online bằng `/papi parse`.
- Hạ mob MythicMobs và LevelledMobs, xác nhận AE chính xác và không bị trả hai lần.
- Kiểm tra quyền nhận reward cho projectile owner theo cấu hình `recipients`.
- Xác nhận internal ID của mob được dùng trong Bí Cảnh tồn tại.
- Xem log khởi động để đảm bảo hook đã nạp; không suy luận tích hợp hoạt động chỉ vì plugin phụ thuộc được cài.