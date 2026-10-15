# API dành cho developer

JAR cung cấp public interface `vn.novusmc.adventurelevel.api.AdventureLevelAPI`, implementation `AdventureLevelAPIImpl`, event trong `vn.novusmc.adventurelevel.event` và enum `ExpSource`.

## Phương thức theo chữ ký public

| Phương thức | Mục đích theo chữ ký |
|---|---|
| `getLevel(UUID)` | Lấy AL |
| `getExp(UUID)` | Lấy AE hiện tại |
| `getRequiredExp(int)` | AE yêu cầu cho level |
| `getRemainingExp(UUID)` | AE còn cần |
| `getTotalExp(UUID)` | Tổng AE |
| `getTitleRaw(UUID)` | Danh hiệu raw |
| `getTitleDisplay(UUID)` | Danh hiệu dạng Adventure `Component` |
| `isStatUnlocked(UUID, String)` | Kiểm tra chỉ số mở khóa |
| `getCalculatedStat(UUID, String)` | Lấy chỉ số đã tính |
| `getStatUnlockLevel(String)` | Level mở khóa chỉ số |
| `giveExp(UUID, long)` / `giveExp(UUID, long, ExpSource)` | Cộng AE |
| `takeExp(UUID, long)` | Trừ AE |
| `setLevel(UUID, int)` | Đặt AL |
| `setExp(UUID, long)` | Đặt AE |

`ExpSource`: `ADMIN_COMMAND`, `INTERNAL_API`, `MYTHICMOBS_DROP`, `MYTHICMOBS_FALLBACK`, `LEVELLEDMOBS`, `BICANH_BREAKTHROUGH`, `BICANH_PENALTY`, `OTHER_PLUGIN`.

## Event public

- `AdventureExpGainEvent`
- `AdventureLevelUpEvent`
- `AdventureBreakthroughEvent`
- `AdventureTitleChangeEvent`

Tài liệu này xác nhận class/method theo chữ ký bytecode; không thay thế source code/Javadoc. Hãy kiểm tra constructor, cancellability, getter, thread-safety và thứ tự event trước khi triển khai tích hợp.