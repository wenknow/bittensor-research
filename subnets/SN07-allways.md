# SN07 - Allways

## ⚠️ 数据修正说明
> 本文档于 2026年4月12日修正。SN07 当前为 **Allways**（跨链交换协议），
> 原 SubVortex 已不在此 UID，请以 taostats.io 实时数据为准。

---

## 基本信息
| 字段 | 数据 |
|------|------|
| UID | SN07 |
| 名称 | **Allways** |
| 运营方/团队 | entrius |
| 子网类型 | 跨链原生交换 / 通用交易层 |
| GitHub | https://github.com/entrius/allways |
| 官网 | — |
| 子网状态 | 活跃（Beta） |

## 功能描述

Allways 是"通用交易层"（Universal Transaction Layer），实现不同链资产之间的**无需信任的原生跨链交换**。

**当前上线**：BTC ↔ TAO 原生互换
**设计目标**：可扩展至任意可验证资产的跨链交换

核心机制：资产在各自链上原生移动（非 Wrapped Token），矿工完成交换订单，验证者独立验证链上结果。智能合约管理抵押品、交换生命周期和验证者投票。

## 挖矿机制

| 角色 | 职责 |
|------|------|
| **矿工（Miner）** | 发布交换汇率对、提供抵押品（Collateral）、执行交换订单 |
| **验证者（Validator）** | 监控交换、验证链上交易、对结果进行投票 |

**抵押品机制**：矿工需锁定 TAO 作为抵押，若交换失败/作弊则触发 Slashing（扣押抵押品）。

**当前状态**：Beta 软件，规范仍在演进中。

## 硬件要求

| 配置项 | 要求 |
|--------|------|
| GPU | **不需要** |
| CPU | 普通服务器即可 |
| RAM | 低（4-8 GB 估计） |
| 存储 | 低 |
| 带宽 | 稳定网络连接 |
| 软件 | Python 3.10+、Docker & Docker Compose、Bittensor 钱包 |

> ✅ **无 GPU 需求**，但需要锁定 TAO 作为矿工抵押品

## 核心风险：抵押品 Slashing

- 矿工必须锁定 TAO 作为抵押（具体金额查阅 GitHub Issues）
- 若交换订单未按时执行或结果有误，**抵押 TAO 将被没收**
- 这是与纯 CPU 节点类子网（如原 SubVortex）的关键区别
- **Beta 阶段风险较高**：协议规则可能变化，智能合约存在未知漏洞

## 经济数据（2026年4月）

| 指标 | 数值 |
|------|------|
| Alpha 代币价格 | 0.0040（taostats 数据） |
| 排放占比 | 请查询 taostats.io/subnets/7 |
| 注册费（TAO） | 请查询链上实时数据 |
| 当前矿工数 | 请查询 taostats.io |

## ROI分析

**无法可靠估算**，原因：
1. Beta 阶段，矿工激励数据不公开
2. 抵押品金额不明
3. Slashing 风险引入不确定损失

## 快速开始（技术参考）

```bash
# 环境要求
# Python 3.10+, Docker & Docker Compose

# 克隆仓库
git clone https://github.com/entrius/allways
cd allways

# 配置 .env 文件
cp .env.example .env
# 填写 PORT 和 WALLET_PATH

# 启动矿工
docker compose up miner
```

## 可行性评级

- **总评：🟡 有条件可参与（高风险早期机会）**
- **适合人群**：了解跨链协议和智能合约的开发者；愿意承担 Beta 风险的早期矿工
- **主要优势**：
  - 无 GPU 要求，门槛相对低
  - 跨链交换赛道需求明确（BTC↔TAO 直接互换）
  - 早期参与者竞争少
- **主要风险**：
  - **Beta 软件，存在智能合约风险**
  - 抵押品 Slashing 机制：操作失误可能损失 TAO
  - 协议规则仍在演进，可能频繁变化
  - Alpha 代币价格极低（0.0040），市值有限
- **新手难度：★★★☆☆**（技术门槛适中，但需理解跨链机制和抵押品风险）

## 参考资源
- **GitHub**: https://github.com/entrius/allways
- **TaoStats**: https://taostats.io/subnets/7/metagraph
- **抵押合约**: https://github.com/bittensor-church/collateral-contracts

## 数据采集时间
2026年4月12日（已修正）
