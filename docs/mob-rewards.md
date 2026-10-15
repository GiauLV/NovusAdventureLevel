# Phần thưởng AE từ mob

`mob-rewards.yml` quy định thưởng Điểm Thám Hiểm (AE) khi mob bị hạ.

Các key chính:

- `settings.enabled`: bật/tắt phần thưởng.
- `settings.prevent-duplicate-rewards`: tránh trả thưởng trùng.
- `settings.priority`: thứ tự khớp nguồn thưởng.
- `recipients`: quy tắc người nhận cho melee, projectile, thú thuần hóa và môi trường.
- `mythicmobs.enabled`, `mythicmobs.drop-identifiers`, `mythicmobs.fallback-rewards`: tích hợp và thưởng dự phòng MythicMobs.
- `levelledmobs.enabled`, `levelledmobs.entity-rewards`, `levelledmobs.global-default`: phần thưởng theo mob/level LevelledMobs.
- `notifications`: thông báo AE, bossbar lên cấp và milestone.

Thứ tự ưu tiên mặc định: `MYTHICMOBS_DROP`, `MYTHICMOBS_INTERNAL_ID`, `LEVELLEDMOBS`, `ENTITY_TYPE`, `DEFAULT`. Kiểm tra `settings.prevent-duplicate-rewards` (mặc định `true`).

Ví dụ cú pháp fallback cần dùng internal ID thật của mob:

```yaml
mythicmobs:
  fallback-rewards:
    enabled: true
    mobs:
      ZombieB:
        ae: 8
      LinhThaoThu:
        ae: "3-6"
```

Fallback mặc định không bật. Sao lưu cấu hình, chỉ đổi một nguồn thưởng mỗi lần và test kill bằng melee/projectile để xác nhận không nhận AE trùng.