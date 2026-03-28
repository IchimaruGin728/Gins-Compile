# Gins-Compile (Sing-Box for OpenWrt A53 APK)

This repository contains a GitHub Actions workflow to compile the **reF1nd** fork of `sing-box` for OpenWrt devices with ARM Cortex-A53 processors (using the `.apk` package format).

## Target Specs
- **Model/Arch**: ARM Cortex-A53 (`aarch64`)
- **Package Format**: `.apk` (OpenWrt 24.xx+)
- **Branch**: `reF1nd-testing-next` (Default)

## How to use
1. Push this folder to a GitHub repository.
2. Go to the **Actions** tab in your repository.
3. Select the **Compile Sing-Box OpenWrt APK** workflow.
4. Click **Run workflow**. 
5. You can optionally specify a different branch from the `reF1nd` repository.
6. Once the build finishes, download the APK from the **Artifacts** section.

## Included Features (Build Tags)
- QUIC
- DHCP
- WireGuard
- ECH (Encrypted Client Hello)
- uTLS
- Reality Server
- Clash API
- gVisor
- V2Ray API
