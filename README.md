# Gins-Compile

用于编译 `sing-box` (reF1nd 版本) 的独立工作流仓库。

## 使用方法

1. 在 GitHub 仓库中点击 **Actions**。
2. 选择 **Build Sing-box (reF1nd)**。
3. 点击 **Run workflow**，输入版本号（例如 `v1.14.0-alpha.1-reF1nd`）并运行。
4. 编译完成后，在 Summary 页面底部下载二进制文件。

## 编译参数说明

本工作流使用的编译参数与 `reF1nd` 官方 release 保持一致：
- **Go Version**: 1.24
- **Tags**: `with_gvisor,with_quic,with_dhcp,with_wireguard,with_utls,with_acme,with_clash_api,with_tailscale,with_ccm,with_ocm,with_naive_outbound,badlinkname,tfogo_checklinkname0`
- **LDFLAGS**: `-X internal/godebug.defaultGODEBUG=multipathtcp=0 -checklinkname=0`
