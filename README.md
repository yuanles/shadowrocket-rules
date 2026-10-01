# shadowrocket-rules

Shadowrocket 配置文件，在上游 `sr_top500_banlist_ad.conf` 基础上手工补充了**加密货币 PROXY 规则**（约 200 条）。

## 文件

- `sr_top500_banlist_ad_crypto.conf` — 主配置文件

## 配置地址

在 Shadowrocket 中添加以下任一 URL 作为配置：

- GitHub Raw：`https://raw.githubusercontent.com/yuanles/shadowrocket-rules/main/sr_top500_banlist_ad_crypto.conf`
- jsDelivr 加速（国内更快）：`https://cdn.jsdelivr.net/gh/yuanles/shadowrocket-rules@main/sr_top500_banlist_ad_crypto.conf`

## 加密货币规则说明

新增段落位于 `[Rule]` 的"手工定义的 Proxy 列表"之后，覆盖：

- 中心化交易所（CEX）
- 去中心化衍生品 / Perp DEX（Hyperliquid、dYdX、Aster、Lighter…）
- 去中心化现货 / 聚合器 DEX
- Meme / 链上交易工具（pump.fun、GMGN、BullX、Axiom…）
- 钱包（Phantom、Rabby、Backpack、NEAR/Sui/Aptos 系…）
- 行情 / 数据 / 新闻（含中文加密媒体）
- 链上浏览器、RPC 基础设施、DeFi / 质押、预测市场、NFT、治理 / 任务 / 域名、稳定币发行方

GFWList 段已覆盖的大所域名（如 binance.com / okx.com）不再重复添加。

## 维护

- 上游原版：https://github.com/johnshall/Shadowrocket-ADBlock-Rules-Forever
- 上游更新后如需合并：下载新版，在相同位置重新插入"加密货币"段落即可（段落有明确注释标记）。
