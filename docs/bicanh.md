# Bí Cảnh Đột Phá

Bí Cảnh là lượt thử thách theo wave gắn với cổng AL. File mẫu trong JAR là `default-bicanh.yml`; lệnh tạo sinh file theo dạng `bicanh/<id>.yml`.

## Thiết lập

1. Đứng tại điểm vào rồi chạy `/adbc create <id>`.
2. Sửa `bicanh/<id>.yml`: `enabled`, cấp cổng, thời gian, hình phạt, số wave và danh sách mob.
3. Tới cửa vào, chạy `/adbc setspawn <id>`.
4. Tại các điểm spawn mob, chạy `/adbc set <id> diem1`, rồi `diem2`… tối đa `diem10`.
5. Chạy `/adbc reload`, sau đó `/adbc info <id>`.
6. Chạy `/adbc test <id>` trên server test trước khi mở cho người chơi.

## Nhóm cấu hình mẫu

- `id`, `ten`, `enabled`.
- `he-thong-cap-do.enabled`.
- `thoigian-hoanthanh` (phút).
- `trung-phat`: bật/tắt hình phạt, số cấp trừ và level tối thiểu.
- `spawn`: điểm vào.
- `diem-spawn-quai`: tối đa 10 điểm.
- `capdobicanh`: cổng, loại, wave, số mob mỗi wave và danh sách mob.

Mẫu có ID placeholder như `__ID__`, `__GATE_LEVEL__` và mob ví dụ. Thay bằng dữ liệu hợp lệ. Cấu hình mặc định có `trung-phat.enabled: true`, nên kiểm tra kỹ mức phạt trước khi chạy. Test mode theo thông báo của plugin không thay đổi AL/AE và không áp hình phạt; vẫn nên xác minh trên bản staging.