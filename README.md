<div align="center">

# External

![规则数量](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fakaspyrean%2Fexternal%2Fmain%2Fstats.json&query=%24.display&label=%E8%A7%84%E5%88%99%E6%95%B0%E9%87%8F&color=4F6D7A)
![自动更新](https://img.shields.io/badge/%E8%A7%84%E5%88%99%E7%BB%B4%E6%8A%A4-%E8%87%AA%E5%8A%A8%E6%9B%B4%E6%96%B0-66856A)
![开源许可](https://img.shields.io/github/license/akaspyrean/external?label=%E5%BC%80%E6%BA%90%E8%AE%B8%E5%8F%AF&color=A98652)

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
