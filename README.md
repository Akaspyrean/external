![数据规模](https://img.shields.io/github/repo-size/akaspyrean/external?label=数据规模)
![更新频率](https://img.shields.io/badge/更新频率-持续维护-brightgreen)
![开源许可](https://img.shields.io/badge/开源许可-MIT%20License-orange)
![最近更新](https://img.shields.io/badge/最近更新-2026--08--18%20UTC%2B08-blue?maxAge=0)

## Clash.F.Win v20.26.0801 R8.1

基于 Clash for Windows v0.20.39 开发版修订，保留原版操作逻辑，集成 Mihomo v1.19.20。

### 功能与特性

* 默认深色主题，提供柔和浅色主题。
* 便携目录结构：`App / Data / Other / Clash.F.Win.exe`。
* 完整中文化：覆盖主界面、设置、菜单、提示与右键操作。
* 支持现代 Mihomo 规则：`GEOSITE`、`GEOIP`、规则集与 TUN。
* 内置预处理：过滤流量/到期等提示节点，提供自动优选、人工优选及分流策略组。
* GeoSite/GeoIP 统一手动更新：代理优先、双文件原子替换、失败保留旧数据、可直接重试

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

<img width="2125" height="1508" alt="01" src="https://github.com/user-attachments/assets/0eba6132-33d6-441f-b5b9-5a89d428cfd4" /><img width="2125" height="1508" alt="03" src="https://github.com/user-attachments/assets/d436ebbd-70b2-4d1e-bb10-5bac1a9d8adb" />



## ⚠️ 免责声明

1. 本仓库内容仅供学习与技术研究使用。
2. 部分资源来自公开网络，版权归原作者或相关平台。
3. 请勿将本仓库任何内容用于商业用途或任何违法行为。

