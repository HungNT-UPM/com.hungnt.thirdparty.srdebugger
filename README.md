# HungNT 3rd-party: SRDebugger

Asset gốc: [SRDebugger — Console & Tools On-Device (Stompy Robot)](https://assetstore.unity.com/packages/tools/gui/srdebugger-console-tools-on-device-27688)

## Cài đặt

Thêm vào `Packages/manifest.json`:

```json
"com.hungnt.thirdparty.srdebugger": "https://github.com/HungNT-UPM/com.hungnt.thirdparty.srdebugger.git"
```

Hoặc Package Manager → **Add package from git URL...**:

```
https://github.com/HungNT-UPM/com.hungnt.thirdparty.srdebugger.git
```

## Note

- Giữ nguyên namespace gốc của asset: `SRDebugger` / `SRF` (asmdef `StompyRobot.SRDebugger`, `StompyRobot.SRF`) — drop-in, code/tutorial của asset chạy ngay.
- Mặc định **tự khởi tạo** lúc runtime (trừ khi tắt trong settings). Mở debug panel bằng cách **triple-tap** vào trigger ở góc trên-trái màn hình; hoặc gọi `SRDebug.Init()` để init thủ công, `SRDebug.Instance.ShowDebugPanel()` để mở panel.
- Cấu hình: menu **Window → SRDebugger Settings** (trigger, pin entry, opacity...).
- Define constraint `!DISABLE_SRDEBUGGER` — thêm symbol `DISABLE_SRDEBUGGER` để loại SRDebugger khỏi build.
