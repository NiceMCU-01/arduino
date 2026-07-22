# NiceMCU Arduino 开发板管理器

[English](./README_EN.md)

NiceMCU BK 系列芯片的官方 Arduino 开发板支持包。

## 快速开始

在 Arduino IDE 中打开“文件 → 首选项”，将以下地址添加到“附加开发板管理器网址”：

```text
https://github.com/NiceMCU-01/arduino/releases/download/global/package_NICEMCU_BK_index.json
```

随后打开“工具 → 开发板 → 开发板管理器”，搜索并安装 `NICEMCU BK7238`。

> 请使用上述稳定地址。后续版本发布后，Arduino IDE 会自动发现更新，无需修改已配置的网址。

## 当前支持

| 芯片 | 开发板 | 当前版本 | 主机环境 |
| --- | --- | --- | --- |
| BK7238 | WB3S | 1.3.0 | Windows |

首发仅提供 Windows 工具链。Linux 和 macOS 支持将在获得完整且经过验证的工具链后再加入。

## 安装步骤

1. 安装 [Arduino IDE](https://www.arduino.cc/en/software)。
2. 打开“文件 → 首选项”。
3. 在“附加开发板管理器网址”中添加上方稳定 JSON 地址。
4. 打开“工具 → 开发板 → 开发板管理器”。
5. 搜索 `NICEMCU BK7238`，并安装最新版本。

## 使用开发板

安装完成后：

1. 在“工具 → 开发板”中选择 `WB3S`。
2. 在“工具 → 端口”中选择实际连接的串口。
3. 打开或创建 Arduino Sketch，编译后上传至开发板。

上传速度和串口连接方式应以实际硬件与项目说明为准。

## 更新方式

本仓库通过 GitHub Releases 发布核心包、工具链与版本索引。

- `global`：Arduino IDE 使用的稳定 JSON 索引。
- `support`：Windows 编译、打包与烧录工具链。
- `vX.Y.Z`：各版本的开发板核心包与索引快照。

用户只需保留同一个 `global` 地址。新版本发布后，开发板管理器将显示可安装的更新版本。

## 从旧地址迁移

旧 Sparkleiot BK7238 开发板管理器地址可继续供已安装用户使用。新用户和后续安装建议使用本仓库的 NiceMCU 稳定 JSON 地址。

## 后续支持

当前首发支持 BK7238/WB3S。NiceMCU 后续将根据硬件与工具链准备情况，逐步增加其他 BK 系列芯片的 Arduino 开发板支持。

## 支持与反馈

如遇安装、编译、上传或开发板兼容性问题，请通过 [Issues](https://github.com/NiceMCU-01/arduino/issues) 提交反馈，并尽量附上：

- Arduino IDE 版本
- 操作系统版本
- 开发板型号、所选端口与上传速率
- 完整报错信息或串口日志
- 可复现问题的最小示例（如有）

如需定制固件或技术合作，请联系：[song@sparkleiot.com](mailto:song@sparkleiot.com)。
