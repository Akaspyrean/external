![数据规模](https://img.shields.io/github/repo-size/akaspyrean/external?label=数据规模)
![更新频率](https://img.shields.io/badge/更新频率-持续维护-brightgreen)
![开源许可](https://img.shields.io/badge/开源许可-MIT%20License-orange)
![最近更新](https://img.shields.io/badge/最近更新-2026--08--01%20UTC%2B08-blue?maxAge=0)

## Clash.F.Win

轻量、中文化的 Mihomo 图形客户端。

Clash.F.Win 基于 Clash for Windows v0.20.39 开发版进行二次修订：保留原版的交互逻辑与整体使用习惯，替换为 Mihomo 内核，并完成界面汉化、视觉细节与兼容性修订。

### 版本特性

- 内核升级：集成 Mihomo v1.19.20，提升新协议与现代配置的兼容性。
- 规则增强：支持 `GEOIP,CN`、`GEOSITE,cn`、Rule Provider 等现代规则能力。
- TUN 模式：支持系统级流量接管，适用于 UWP 应用、游戏及无法使用系统代理的程序。
- 深度汉化：界面、弹窗、菜单与常用说明均按中文使用习惯重构。
- 视觉修订：修正原版部分布局、间距与右侧控件对齐问题。
- 极简设计：不加入推广、反馈入口或无关功能，保持原版轻量与流畅。
- 默认安全配置：默认日志级别为“错误”，减少无意义日志与磁盘写入。

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

**📑 配置文件：Clash & Shadowrocket 深度适配**

* Clash (.yaml)：针对 Mihomo 特性优化的配置文件，预设科学的分流逻辑。
* ​Shadowrocket (.conf)​：适配小火箭的配置方案，实现移动端与 PC 端策略一致。

**📡 分流规则​：动态更新的规则集**

* ​代理转发 (Proxy)​：全面收集海外高频访问站点，减少漏网之鱼。
* ​绕过直连 (Direct)：涵盖国内主流网站，确保本地流量不走弯路。
* 人工智能 (AI)：精准覆盖 OpenAI、Anthropic、Claude 等主流 AI 服务。
* ​影音视听 (Media)​：针对 YouTube、Netflix、Disney 等流媒体进行分流优化。
* ​`.yaml` 格式：适配 Clash 系列客户端，全面支持规则集调用与在线自动更新。
* ​`.list` 格式​：兼容 Shadowrocket (小火箭) 及其他支持纯文本规则列表的客户端。

<img width="500" height="333" alt="image" src="https://github.com/user-attachments/assets/d9f1de78-723b-47af-8f22-834252c48032" />

<img width="500" height="333" alt="image" src="https://github.com/user-attachments/assets/3f4637df-a51b-4cfe-a4c8-cdd98e83d557" />

<img width="500" height="333" alt="image" src="https://github.com/user-attachments/assets/0f362511-8637-475b-8024-705a7d642fa5" />



## ⚠️ 免责声明

1. 本仓库内容仅供学习与技术研究使用。
2. 部分资源来自公开网络，版权归原作者或相关平台。
3. 请勿将本仓库任何内容用于商业用途或任何违法行为。

