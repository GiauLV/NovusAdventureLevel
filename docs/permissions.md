# Permissions

Các node khai báo trong `plugin.yml` của JAR 1.1.1:

| Permission | Default | Ý nghĩa |
|---|---:|---|
| `novusal.use` | `true` | Dùng GUI AL/chỉ số |
| `novusal.top` | `true` | Dùng bảng xếp hạng |
| `novusal.admin` | `op` | Quyền quản trị AL tổng |
| `novusal.admin.give` | `op` | Cộng AE |
| `novusal.admin.set` | `op` | Đặt cấp/AE |
| `novusal.admin.take` | `op` | Trừ AE |
| `novusal.admin.see` | `op` | Xem dữ liệu người chơi |
| `novusal.admin.reset` | `op` | Reset dữ liệu người chơi |
| `novusal.admin.reload` | `op` | Reload cấu hình chính |
| `novusadventurelevel.bicanh.use` | `true` | Dùng GUI/lệnh Bí Cảnh |
| `novusadventurelevel.bicanh.admin` | `op` | Quản trị Bí Cảnh |
| `novusadventurelevel.bicanh.command-bypass` | `false` | Bypass chặn lệnh khi đang trong Bí Cảnh |

## Ví dụ LuckPerms

```text
/lp group helper permission set novusal.admin.see true
/lp group admin permission set novusadventurelevel.bicanh.admin true
```

Chỉ cấp quyền cần dùng; không mặc định cấp `*`. Kiểm tra lại permission nodes khi nâng cấp phiên bản.