# NEGAN Streams — OTA

Repo này chứa **manifest + IPA** cho shortcut cài đặt OTA của NEGAN Streams.

## Shortcut

```text
itms-services://?action=download-manifest&url=https://cdn.jsdelivr.net/gh/neganconsole-backup/download@latest/manifest.plist
```

## Files

- `q7f2m9x4k1.ipa` — IPA đã ký, bundle ID `app.orange695.durian8453`
- `manifest.plist` — manifest trỏ tới IPA

## Bản hiện tại

- Version: **2.22 (26)**
- Title: **NEGAN Streams 2.22**

## Phát hành bản mới

1. Build & ký IPA.
2. Cập nhật `q7f2m9x4k1.ipa` và `manifest.plist` (`bundle-version`, `title`).
3. Commit + push `main`.
4. Tạo/cập nhật tag `v<version>` trỏ tới commit mới.
5. Purge cache jsDelivr:
   - `https://purge.jsdelivr.net/gh/neganconsole-backup/download@latest/manifest.plist`
   - `https://purge.jsdelivr.net/gh/neganconsole-backup/download@latest/q7f2m9x4k1.ipa`
6. Shortcut giữ nguyên; bấm lại sẽ cài bản mới.

## Liên kết

- Source: https://github.com/neganconsole-backup/SOURCE-IOS-APPS/tree/main/STREAMS-APPS
- Cert & quy trình ký: repo `CERT-IOS`
