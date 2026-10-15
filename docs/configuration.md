# Cấu hình

Các tệp trong `defaults/` là bản nhúng trong JAR 1.1.1, không phải bản cấu hình runtime đã được admin chỉnh sửa.

| File | Vai trò |
|---|---|
| `config.yml` | AL tối đa/khởi đầu, công thức AE, parse số, leaderboard, bossbar/milestone và thiết lập Bí Cảnh chung |
| `messages.yml` | Thông điệp và trợ giúp |
| `menus.yml` | Bố cục GUI |
| `mob-rewards.yml` | Quy tắc cộng AE khi mob bị hạ |
| `stats.yml` | Định nghĩa/cap chỉ số và giá trị theo khoảng AL |
| `titles.yml` | Danh hiệu theo khoảng AL |
| `default-bicanh.yml` | Mẫu tạo Bí Cảnh mới |
| `bicanh/<id>.yml` | Cấu hình mỗi Bí Cảnh trong runtime |

## Giá trị mặc định nổi bật trong config.yml

| Key | Mặc định |
|---|---:|
| `settings.max-level` | `2000` |
| `settings.start-level` | `1` |
| `settings.start-exp` | `0` |
| `settings.clear-exp-at-max-level` | `true` |
| `settings.allow-level-down-when-taking-exp` | `false` |
| `settings.auto-save-minutes` | `5` |
| `exp-formula.base` | `60` |
| `exp-formula.linear` | `18` |
| `exp-formula.quadratic` | `3.0` |
| `leaderboard.entries` | `10` |
| `placeholder.progress-bar.length` | `20` |

## Quy trình chỉnh cấu hình

1. Sao lưu file hiện tại.
2. Sửa trên server thử nghiệm và giữ đúng YAML indentation/kiểu dữ liệu.
3. Dùng `/capmaohiem reload` để nạp cấu hình chính; dùng `/adbc reload` cho Bí Cảnh.
4. Kiểm tra console và kết quả trong game trước khi triển khai server chính.