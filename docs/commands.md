# Lệnh

## Người chơi

| Lệnh | Chức năng |
|---|---|
| `/capmaohiem` | Mở GUI Cấp Mạo Hiểm |
| `/capmaohiem menu` | Mở GUI chính |
| `/capmaohiem stats` | Mở GUI chỉ số |
| `/capmaohiem profile` | Xem hồ sơ AL/AE trong chat |
| `/capmaohiem top` | Mở GUI bảng xếp hạng |
| `/capmaohiem top chat` | Hiển thị bảng xếp hạng trong chat |
| `/capmaohiem help` | Trợ giúp |
| `/capmaohiem reload` | Nạp lại cấu hình chính |
| `/bicanh` | Mở GUI Bí Cảnh Đột Phá |

Alias `/capmaohiem`: `/cmh`, `/al`, `/adventurelevel`. Alias quản trị Bí Cảnh `/adminbicanh`: `/adbc`.

## Quản trị AL/AE

```text
/al give <player> <amount|range> [-s] [-sf]
/al take <player> <amount> [-sf]
/al set <player> <exp> [-sf]
/al see <player>
/capmaohiem admin give <player> <amount>
/capmaohiem admin set <player> <level> [exp]
/capmaohiem admin take <player> <amount>
/capmaohiem admin see <player>
/capmaohiem admin reset <player>
```

`-s` ẩn thông báo nhận AE theo hành vi trong thông điệp trợ giúp của plugin; `-sf` điều khiển phản hồi lệnh. Amount parser mặc định hỗ trợ hậu tố `k`, `m`, `b`.

## Quản trị Bí Cảnh

```text
/adbc create <id>
/adbc setspawn <id>
/adbc unsetspawn <id>
/adbc set <id> <diem1..diem10>
/adbc unset <id> <diem1..diem10>
/adbc info <id>
/adbc danhsach
/adbc test <id>
/adbc test stop
/adbc reload
```

Lệnh thiết lập vị trí cần người chơi đang đứng tại tọa độ mong muốn; không chạy lệnh đó từ console. Dùng `/adbc info <id>` để kiểm tra trạng thái sẵn sàng. Lệnh reset có thể làm mất tiến trình người chơi: sao lưu trước khi dùng.

## Quyền

Xem [permissions.md](permissions.md) trước khi cấp quyền staff.