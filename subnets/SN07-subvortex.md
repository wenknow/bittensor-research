# SN07 - SubVortex

## 基本信息
| 字段 | 数据 |
|------|------|
| UID | SN07 |
| 名称 | SubVortex |
| 运营方/团队 | eclipsevortex |
| 子网类型 | 基础设施节点 |
| GitHub | https://github.com/eclipsevortex/SubVortex |
| 官网 | https://www.subvortex.com/ |
| 子网状态 | 活跃 |

## 功能描述

SubVortex 通过构建去中心化的 Subtensor 节点网络来增强 Bittensor 整体网络的稳定性与去中心化程度。矿工通过运行 Subtensor（Bittensor 的底层区块链节点）来为全网提供基础设施服务。

**核心价值主张**：解决 Bittensor 节点中心化问题，确保网络健壮性，服务完全免费向社区开放。

## 挖矿机制

矿工运行一个本地 Subtensor 节点，验证者根据以下指标对矿工评分：

| 评分维度 | 权重 |
|----------|------|
| **可用性（Availability）** | 高 |
| **延迟（Latency）** | 高 |
| **可靠性（Reliability）** | 高 |
| **全球分布（Distribution）** | 中 |

评分周期：持续监控，无单次任务提交机制。

## 硬件要求

| 配置项 | 最低要求 | 推荐配置 |
|--------|----------|----------|
| **GPU** | **不需要** | **不需要** |
| VRAM | — | — |
| CPU | 4核+ | 8核+ |
| RAM | 16 GB | 32 GB |
| 存储 | 500 GB SSD | 1 TB NVMe SSD |
| 带宽 | 100 Mbps | 1 Gbps |
| 操作系统 | Ubuntu 20.04+ | Ubuntu 22.04 |

> ⭐ **关键优势：无需GPU！** 这是极少数可以用普通服务器/VPS参与的子网之一。

## 经济数据（2026年4月）

| 指标 | 数值 |
|------|------|
| 排放占比 | ~0.5-1%（基础设施类，不是高排放子网） |
| 注册费（TAO） | 动态，约 0.5-3 TAO（需实时查询） |
| 当前矿工数 | ~100-256（需 taostats 实时确认） |
| 服务费 | **免费**（子网声明服务全免费） |
| 子网市值 | 较低（基础设施类） |

## ROI分析

**TAO价格基准：$300**

| 情景 | 说明 | 日收益(TAO) | 月毛收益(USD) | 月运营成本(USD) | 月净收益(USD) |
|------|------|------------|--------------|----------------|--------------|
| 保守 | 底部30%，高延迟节点 | ~0.02 | ~$180 | $50（VPS费） | **+$130** |
| 中性 | 中位数，稳定节点 | ~0.05 | ~$450 | $80（VPS费） | **+$370** |
| 乐观 | TOP节点，低延迟 | ~0.10 | ~$900 | $120（专线） | **+$780** |

- **注册成本**：约 0.5-3 TAO × $300 = $150-$900（一次性沉没成本）
- **回本周期（中性）**：注册费/月净收益 ≈ 1-2.5个月
- **主要成本**：VPS服务器费用（$20-$80/月），电费可忽略
- **竞争饱和度**：**中**（节点质量有差异，好的地理位置有优势）

## 可行性评级

- **总评：🟢 立即可参与**
- **适合人群**：有 Linux 服务器运营经验的矿工；有 VPS/服务器资源的用户；不具备高端 GPU 但想参与 Bittensor 的新手
- **主要优势**：
  - **零GPU要求**，普通 VPS 即可
  - 服务完全免费，无API订阅等额外成本
  - 文档相对清晰（官方+GitHub）
  - 运行稳定后接近被动收入
- **主要风险**：
  - 排放占比较低，收益绝对值不高
  - 节点需要持续在线，网络中断影响评分
  - 注册费动态变化，需把握时机

- **新手难度：★★☆☆☆**（需要基本Linux服务器运维能力）

## 快速开始指南

```bash
# 1. 克隆仓库
git clone https://github.com/eclipsevortex/SubVortex
cd SubVortex

# 2. 安装依赖（需要Python 3.10+）
pip install -r requirements.txt

# 3. 创建钱包
btcli wallet new_coldkey --wallet.name miner
btcli wallet new_hotkey --wallet.name miner --wallet.hotkey default

# 4. 注册到子网7
btcli subnet register --netuid 7 --wallet.name miner

# 5. 运行矿工
python neurons/miner.py --wallet.name miner --wallet.hotkey default
```

## 参考资源
- **GitHub**: https://github.com/eclipsevortex/SubVortex
- **官网**: https://www.subvortex.com/
- **TaoStats**: https://taostats.io/subnets/7/metagraph
- **矿工指南**: SubVortex GitHub README

## 数据采集时间
2026年4月
