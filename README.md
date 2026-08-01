![数据规模](https://img.shields.io/github/repo-size/akaspyrean/external?label=数据规模)
![更新频率](https://img.shields.io/badge/更新频率-持续维护-brightgreen)
![开源许可](https://img.shields.io/badge/开源许可-MIT%20License-orange)
![最近更新](https://img.shields.io/badge/最近更新-2026--08--02%20UTC%2B08-blue?maxAge=0)

## Clash.F.Win

轻量、中文化的 Mihomo 图形客户端。

### 核心更新

- 替换为 Mihomo v1.19.20 内核。
- 增强现代规则兼容性，支持 `GEOIP,CN`、`GEOSITE,cn`、Rule Provider 等规则能力。
- 优化配置解析与加载稳定性。
- 保留并适配 TUN 模式及服务模式管理能力。

### 界面与汉化

- 深度汉化主界面、设置页、日志页、连接页、资源页及托盘菜单。
- 修正日志级别弹窗，完整翻译“修改日志级别”、说明文本及全部选项。
- 默认日志级别调整为“错误”。
- 修复部分英文残留、术语不统一与状态文案不准确的问题。
- 优化页面间距、控件右对齐与开关状态显示。

## 便携版优化

- 调整为 `App / Data / Other / Clash.F.Win.exe` 结构。
- 配置与运行数据集中保存在根目录 `Data` 文件夹。
- 首次运行自动补齐默认配置，不覆盖已有用户配置。
- 保持旧框架所需的数据目录兼容性，避免因目录层级变化导致内核无法启动。
- 自解压包仅负责解压，不会自动启动程序。

### 使用方法

1. 解压程序至任意目录。
2. 运行根目录中的 `Clash.F.Win.exe`。
3. 在“配置”页面导入订阅或本地配置。
4. 在“主页”确认 Mihomo 内核状态后，根据需要启用系统代理或 TUN 模式。

程序数据保存在根目录的 `Data` 文件夹中，便于备份、迁移与清理。

### TUN 模式说明

TUN 模式需要系统具备相应网络驱动与权限。首次启用前，请在“服务模式”中完成必要组件的安装或管理。

启用 TUN 前建议：

- 使用管理员权限运行相关安装操作；
- 确认虚拟网卡驱动可正常使用；
- 遇到网络异常时，先关闭 TUN 模式并检查服务状态。

### 配置建议

建议优先使用 Mihomo 规则语法，例如：

```yaml
GEOSITE,private,DIRECT
GEOSITE,cn,DIRECT
GEOIP,CN,DIRECT
MATCH,扶梯出行。
```

## 📑 配置文件：Clash & Shadowrocket 深度适配

* Clash (.yaml)：针对 Mihomo 特性优化的配置文件，预设科学的分流逻辑。
* ​Shadowrocket (.conf)​：适配小火箭的配置方案，实现移动端与 PC 端策略一致。

**📡 分流规则​：动态更新的规则集**

* ​代理转发 (Proxy)​：全面收集海外高频访问站点，减少漏网之鱼。
* ​绕过直连 (Direct)：涵盖国内主流网站，确保本地流量不走弯路。
* 人工智能 (AI)：精准覆盖 OpenAI、Anthropic、Claude 等主流 AI 服务。
* ​影音视听 (Media)​：针对 YouTube、Netflix、Disney 等流媒体进行分流优化。
* ​`.yaml` 格式：适配 Clash 系列客户端，全面支持规则集调用与在线自动更新。
* ​`.list` 格式​：兼容 Shadowrocket (小火箭) 及其他支持纯文本规则列表的客户端。

<img width="637.5" height="452.4" alt="01" src="https://github.com/user-attachments/assets/457ba1ec-4c08-4cb9-8703-725baa70a138" />
<img width="637.5" height="452.4" alt="02" src="https://github.com/user-attachments/assets/6a62e89e-60c5-4bba-b595-28edd169029e" />



## ⚠️ 免责声明

1. 本仓库内容仅供学习与技术研究使用。
2. 部分资源来自公开网络，版权归原作者或相关平台。
3. 请勿将本仓库任何内容用于商业用途或任何违法行为。

