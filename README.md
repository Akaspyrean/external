<div align="center">

# External

![开源许可](https://img.shields.io/badge/开源许可-MIT%20License-blue)
![最近更新](https://img.shields.io/badge/最近更新-2026--08--20%20UTC%2B08-brightgreen?maxAge=0)

**Mihomo / Clash & Shadowrocket 智能分流配置与在线规则**

统一桌面与移动端分流策略，自动选路，规则集自动维护并远程更新。

</div>

## Features

* **双端一致** — Mihomo / Clash 与 Shadowrocket 共用分流逻辑
* **自动选路** — 自动识别专线与普通节点并测速优选
* **独立分流** — AI、Media 与常规代理采用独立策略
* **自动维护** — Direct / Proxy / AI / Media / Ad 规则集持续自动更新
* **自动同步** — 客户端通过远程 Rule Provider / Rule Set 自动获取最新规则

## Config

| Client         | Config                                              |
| -------------- | --------------------------------------------------- |
| Mihomo / Clash | [`ParsersforClash.yml`](config/ParsersforClash.yml) |
| Shadowrocket   | [`shadowrocket.conf`](config/shadowrocket.conf)     |

## Rules

| Rule   | YAML                        | LIST                        |
| ------ | --------------------------- | --------------------------- |
| Direct | [`yaml`](rules/direct.yaml) | [`list`](rules/direct.list) |
| Proxy  | [`yaml`](rules/proxy.yaml)  | [`list`](rules/proxy.list)  |
| AI     | [`yaml`](rules/ai.yaml)     | [`list`](rules/ai.list)     |
| Media  | [`yaml`](rules/media.yaml)  | [`list`](rules/media.list)  |
| Ad     | [`yaml`](rules/ad.yaml)     | [`list`](rules/ad.list)     |

## Raw

```text
https://raw.githubusercontent.com/akaspyrean/external/main/rules/ai.yaml
```

替换规则名称即可直接引用。

## License

MIT
