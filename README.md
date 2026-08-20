# External

面向 **Mihomo / Clash 系客户端与 Shadowrocket** 的分流配置与持续维护规则集。

提供订阅预处理配置以及 `Direct`、`Proxy`、`AI`、`Media`、`Ad` 等分类规则，支持远程引用与自动更新。

![数据规模](https://img.shields.io/github/repo-size/akaspyrean/external?label=数据规模)
![更新频率](https://img.shields.io/badge/更新频率-持续维护-brightgreen)
![开源许可](https://img.shields.io/badge/开源许可-MIT%20License-orange)
![最近更新](https://img.shields.io/badge/最近更新-2026--08--20%20UTC%2B08-blue?maxAge=0)

## 配置

| 客户端          | 文件                                                  | 说明                          |
| ------------ | --------------------------------------------------- | --------------------------- |
| Clash 系      | [`ParsersforClash.yml`](config/ParsersforClash.yml) | 订阅 Parser，自动配置 DNS、策略组与远程规则 |
| Shadowrocket | [`shadowrocket.conf`](config/shadowrocket.conf)     | Shadowrocket 分流配置           |

### Clash Parser

`ParsersforClash.yml` 用于支持 Parser 的 Clash 系客户端，对订阅配置进行预处理，包括：

* 自动识别专线与普通节点
* 自动生成策略组
* AI 独立分流
* 流媒体独立分流
* 国内流量直连
* Mihomo GeoSite / GeoIP 分流
* 在线加载本仓库规则集

Raw：

```text
https://raw.githubusercontent.com/akaspyrean/external/main/config/ParsersforClash.yml
```

### Shadowrocket

`shadowrocket.conf` 提供与 Clash 配置基本一致的分流结构：

```text
https://raw.githubusercontent.com/akaspyrean/external/main/config/shadowrocket.conf
```

## 规则

规则同时提供：

* `.yaml`：适用于 Mihomo / Clash Rule Provider
* `.list`：适用于 Shadowrocket 等文本规则客户端

| 规则     | 用途    | YAML                               | LIST                               |
| ------ | ----- | ---------------------------------- | ---------------------------------- |
| Direct | 直连流量  | [`direct.yaml`](rules/direct.yaml) | [`direct.list`](rules/direct.list) |
| Proxy  | 代理流量  | [`proxy.yaml`](rules/proxy.yaml)   | [`proxy.list`](rules/proxy.list)   |
| AI     | AI 服务 | [`ai.yaml`](rules/ai.yaml)         | [`ai.list`](rules/ai.list)         |
| Media  | 流媒体   | [`media.yaml`](rules/media.yaml)   | [`media.list`](rules/media.list)   |
| Ad     | 广告规则  | [`ad.yaml`](rules/ad.yaml)         | [`ad.list`](rules/ad.list)         |

规则文件持续维护，可通过 Raw URL 直接作为远程规则订阅。

例如：

```text
https://raw.githubusercontent.com/akaspyrean/external/main/rules/ai.yaml
```

或：

```text
https://raw.githubusercontent.com/akaspyrean/external/main/rules/ai.list
```

## 分流逻辑

默认策略大致为：

```text
局域网 / 国内服务
        ↓
      DIRECT

AI 服务
        ↓
    人工智能策略

流媒体
        ↓
    影音视听策略

其他代理规则
        ↓
      扶梯出行

未匹配流量
        ↓
      扶梯出行
```

不同客户端的具体行为以对应配置文件为准。

## License

[MIT License](LICENSE)

## Disclaimer

本仓库仅用于网络配置、规则维护与技术研究。

规则可能来源于公开数据，并会随着网络服务变化持续调整。使用者应自行确认相关规则、配置以及网络服务符合所在地法律法规及服务条款。

