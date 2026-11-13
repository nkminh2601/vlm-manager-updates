# VL-IDLE Manager Updates

Official public release channel for the Windows x64 VL-IDLE Manager.

## For users

1. Download `ManagerLauncher.exe` from the latest release and keep it in the folder where you want Manager installed.
2. Open the launcher. It checks for the latest approved Manager release, downloads the app, and installs the pinned Node.js and Electron runtimes when missing.
3. Use **Kiểm tra cập nhật**, **Thử lại**, and **Vào Manager hiện tại** from the launcher. Download and install progress appears in the launcher window.

Only the launcher is a manual download. The launcher downloads the Manager update ZIP and any missing official runtimes over HTTPS. Your local `data` folder stays beside the launcher and is not part of release ZIPs.

## Release format

- Manager app packages are named `fix<number>.zip` and contain the `app/` tree only.
- Each ZIP is published with a SHA-256 sidecar.
- A release is made stable only after the Fix has been explicitly approved.
- This repository contains release assets and documentation only. It must never contain the development workspace, account records, cookies, passwords, or other personal data.

## Platform

Windows x64. A working Internet connection is needed for first install and updates. Existing installations can still be started from the launcher when an update check fails.