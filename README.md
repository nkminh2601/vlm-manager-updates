# VL-IDLE Manager Updates

Official public release channel for the Windows x64 VL-IDLE Manager.

## For users

1. Download [ManagerLauncher.exe](https://github.com/nkminh2601/vlm-manager-updates/releases/download/fix384/ManagerLauncher.exe) and keep it in the folder where you want Manager installed. This is launcher 1.1.0.
2. Open the launcher. It checks the latest approved Manager release, verifies the update ZIP and installs the pinned official Node.js/Electron runtimes when missing.
3. Use **Kiểm tra cập nhật**, **Thử lại**, and **Vào Manager hiện tại**. Progress appears in the launcher window.

Existing users: update to Fix384 or later using the existing launcher, then open Manager. Manager verifies the bundled launcher and upgrades the recognized old standard `ManagerLauncher.exe` after its file lock clears. Failed swaps retain or restore the previous launcher. Personal, unknown or newer launcher binaries are preserved. If Windows has already quarantined the old launcher, download the new launcher manually once using the link above.

Your local `data` folder stays beside the launcher and is not part of release ZIPs.

## Release format

- Manager packages are named `fix<number>.zip` and contain the `app/` tree only.
- Downloads are verified against GitHub release-asset SHA-256 digests; no separate `.sha256` asset is required.
- From Fix384, `app/launcher/` contains the verified launcher bundle and its migration manifest.
- A standalone `ManagerLauncher.exe` asset is uploaded when the launcher changes; ordinary app-only releases need only their Fix ZIP.
- Stable releases are published only after the exact Fix is explicitly approved.
- This repository contains release assets and documentation only, never the development workspace, account records, cookies, passwords or personal data.

## Platform

Windows x64. Internet access is needed for first install and updates. Existing installations can still start when update checks fail. The launcher is currently unsigned, so SmartScreen or other security products may still display warnings.
