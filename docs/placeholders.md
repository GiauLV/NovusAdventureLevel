# PlaceholderAPI

Khi PlaceholderAPI được cài, expansion dùng identifier `novusal`; mẫu `%novusal_<key>%`.

## AL/AE

| Placeholder | Ý nghĩa |
|---|---|
| `%novusal_level%` / `%novusal_level_raw%` | Cấp AL dạng định dạng / thô |
| `%novusal_exp%` / `%novusal_exp_raw%` | AE hiện tại |
| `%novusal_required_exp%` / `%novusal_required_exp_raw%` | AE yêu cầu cho cấp hiện tại |
| `%novusal_remaining_exp%` / `%novusal_remaining_exp_raw%` | AE còn cần lên cấp |
| `%novusal_total_exp%` / `%novusal_total_exp_raw%` | Tổng AE tích lũy |
| `%novusal_progress%` | Tiến trình đã định dạng |
| `%novusal_progress_percent%` | Tiến trình phần trăm |
| `%novusal_progress_bar%` | Thanh tiến trình |
| `%novusal_max_level%` / `%novusal_max_level_raw%` | Cấp tối đa |
| `%novusal_is_max_level%` | Đã đạt cấp tối đa hay chưa |
| `%novusal_title%` / `%novusal_title_raw%` | Danh hiệu hiện tại |
| `%novusal_next_title%` / `%novusal_next_title_raw%` | Danh hiệu tiếp theo |
| `%novusal_next_title_min_level%` | Cấp tối thiểu danh hiệu tiếp theo |
| `%novusal_rank_number%` | Thứ hạng theo khoảng danh hiệu |
| `%novusal_rank_range%` | Khoảng cấp danh hiệu |

## Bí Cảnh

`%novusal_bicanh_required%`, `%novusal_bicanh_ready%`, `%novusal_bicanh_id%`, `%novusal_bicanh_name%`, `%novusal_bicanh_gate_level%`, `%novusal_bicanh_status%`, `%novusal_bicanh_wave%`, `%novusal_bicanh_max_wave%`, `%novusal_bicanh_time_left%`.

## Chỉ số

Dùng `%novusal_stat_<key>%`; thêm `_raw` để lấy giá trị thô. Ví dụ: `%novusal_stat_max_health%`, `%novusal_stat_attack_damage%`, `%novusal_stat_defense%`, `%novusal_stat_movement_speed%`. Key phải được định nghĩa/bật trong `stats.yml`; tác động chỉ số còn phụ thuộc tích hợp MythicLib.

## Kiểm tra

```text
/papi parse <player> %novusal_level%
/papi parse <player> %novusal_title%
/papi parse <player> %novusal_progress_bar%
```

Nếu chuỗi placeholder còn nguyên, kiểm tra plugin đã enable và placeholder/key có đúng chính tả.