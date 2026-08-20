<div align="center">

# External

![开源许可](https://img.shields.io/badge/开源许可-MIT%20License-blue)
![最近更新](https://img.shields.io/badge/最近更新-2026--08--20%20UTC%2B08-brightgreen?maxAge=0)

**Mihomo / Clash 与 Shadowrocket 智能分流配置及在线规则集**

统一桌面与移动端分流策略，自动选路，规则集自动维护并持续更新。

</div>

## 特色

* **自动同步**：客户端通过远程规则自动获取最新内容
* **自动选路**：自动识别专线与普通节点，并进行测速优选
* **独立分流**：人工智能、影音与常规代理分别采用独立策略
* **双端一致**：Mihomo / Clash 与 Shadowrocket 共用分流逻辑
* **自动维护**：直连、代理、人工智能、影音、广告规则集持续自动更新


## 配置

| 客户端            | 配置文件                                                |
| -------------- | --------------------------------------------------- |
| Mihomo / Clash | [`ParsersforClash.yml`](config/ParsersforClash.yml) |
| Shadowrocket   | [`shadowrocket.conf`](config/shadowrocket.conf)     |

## 规则

| 类型   | YAML                               | LIST                               |
| ---- | ---------------------------------- | ---------------------------------- |
| 直连   | [`direct.yaml`](rules/direct.yaml) | [`direct.list`](rules/direct.list) |
| 广告   | [`ad.yaml`](rules/ad.yaml)         | [`ad.list`](rules/ad.list)         |
| 代理   | [`proxy.yaml`](rules/proxy.yaml)   | [`proxy.list`](rules/proxy.list)   |
| 流媒体  | [`media.yaml`](rules/media.yaml)   | [`media.list`](rules/media.list)   |
| 人工智能 | [`ai.yaml`](rules/ai.yaml)         | [`ai.list`](rules/ai.list)         |

## 在线引用

```text
https://raw.githubusercontent.com/akaspyrean/external/main/rules/ai.yaml
```

替换规则文件名即可引用其他规则。

## 开源许可

MIT
