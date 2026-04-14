# Bittensor 128子网深度挖矿调研报告

> **生成时间**：2026年4月12日 | **最后验证**：2026年4月14日（SN01-SN34 二次全量核查）
> **TAO参考价格**：~$300（实际约 $285-320）  
> **日总排放**：3,600 TAO（2025年12月减半后）  
> **研究范围**：全部 128 个活跃子网

## 🚨 重要数据准确性警告

**Bittensor 子网 UID 分配会随时间变化！** 低排放子网可能被注销，新项目接管原有 UID。

### 2026年4月14日 SN01-SN34 二次核查（重大更新）

> ⚠️ **触目惊心的发现**：SN01-SN34 范围内绝大多数子网已更换运营方，不只是 SN35+ 范围。

| UID | 原记录 | taostats 当前名称 | Alpha价格 | 状态 |
|-----|--------|-----------------|-----------|------|
| SN01 | Text Prompting | **Apex** | 0.0112 | 已修正 |
| SN01 | Text Prompting | **Apex** | 0.0112 | 已修正 |
| SN02 | Omron（Inference Labs） | **DSperse** | 0.0087 | 已修正 |
| SN03 | τemplar（$134.9M市值） | **deprecat...** | 0.0296 | ⚠️ 疑似废弃，重大风险 |
| SN05 | OpenKaito | **Hone** | 0.0180 | 已修正 |
| SN06 | Nous Research（Finetuning） | **Numinous** | 0.0053 | 已修正 |
| SN09 | Pre-Training | **iota** | 0.0244 | 已修正 |
| SN10 | Apollo ZK | **Swap** | 0.0060 | 已修正 |
| SN11 | Transcription（Cazure） | **Trajecto...** | 0.0125 | 已修正 |
| SN12 | ComputeHorde | **Compute...** | 0.0067 | ⚠️ 可能改名，待确认 |
| SN14 | LLM Defender | **TAOHash** | 0.0089 | 已修正 |
| SN15 | Blockchain Insights | **ORO** | 0.0147 | 已修正 |
| SN17 | ThreeGen（PlixML） | **404—GEN** | 0.0148 | 已修正 |
| SN18 | Cortex.T（Corcel API） | **Zeus** | 0.0072 | 已修正 |
| SN19 | Nineteen（Rayon Labs） | **blockmac...** | 0.0140 | 已修正 |
| SN20 | BitAgent（RogueTensor） | **GroundLa...** | 0.0040 | 已修正 |
| SN23 | NicheImage（NicheTensor） | **Trishool** | 0.0042 | 已修正 |
| SN24 | Omega Labs | **Quasar** | 0.0147 | 已修正 |
| SN25 | Hivetrain | **Mainfram...** | 0.0049 | 已修正 |
| SN26 | Image Alchemy | **Kinitro** | 0.0038 | 已修正 |
| SN28 | Foundry S&P500 Oracle | **Unknown** | 0.0102 | 已修正，无运营方 |
| SN29 | Fractal（视频生成） | **Coldint** | 0.0140 | 已修正 |
| SN31 | NAS Chain | **Halftime** | 0.0043 | 已修正 |
| SN33 | 待确认 | **ReadyAI** | — | 已识别 |
| SN34 | 待确认 | **BitMind** | — | 已识别 |

**仍确认正确的子网**：SN04 Targon ✅、SN07 Allways ✅、SN08 Vanta ✅、SN16 BitAds ✅、SN22 Desearch ✅、SN27 Nodexo ✅、SN32 ItsAI ✅

---

### 2026年4月13日 全量验证结果（SN35-SN128）

通过逐一访问 taostats.io/subnets/{UID}/metagraph 完成所有128个子网的名称核查，主要修正：

| 原记录 | taostats 实际名称 | 状态 |
|--------|------------------|------|
| SN07 SubVortex | **Allways**（BTC↔TAO跨链） | 已修正 |
| SN36 Web Agents | **Unknown** | 已修正 |
| SN39 待确认 | **Deprecated**（已废弃） | 已修正 |
| SN42 Masa | **Unknown** | 已修正 |
| SN56 待确认 | **Gradient**（Rayon Labs子网） | 已修正 |
| SN67 Tenex | **Harnyx** | 已修正 |
| SN78 Deregistration风险 | **Loosh** | 已修正 |
| SN81 待确认 | **Deprecated**（已废弃） | 已修正 |
| SN82 Deregistration风险 | **Hermes** | 已修正 |
| SN96 新子网 | **Verathos**（Alpha价格2.87，异常高） | 重要发现 |
| SN104 待确认 | **for sale**（待售/空置） | 重要发现 |

**已识别子网**（SN35-SN128范围）：
Cartha(35)、Aurelius(37)、Colosseum(38)、Chunking(40)、Almanac(41)、Graphite(43)、Score(44)、RESI(46)、EvolAI(47)、Quantum(48)、Dojo(52)、Efficient LLM(53)、NIOME(55)、Sparket(57)、Handshake(58)、Babelbit(59)、RedTeam(61)、Enigma(63)、TAO Privacy(65)、Harnyx(67)、NOVA(68)、NexisGen(70)、Leadpoet(71)、MetaHash(73)、Gittensor(74)、Byzantium(76)、Liquidity(77)、Loosh(78)、MVTRX(79)、Hermes(82)、CliqueAI(83)、Luminar(87)、Bitstart(91)、Bitcast(93)、Bitsota(94)、Verathos(96)、Leoma(99)、Platform(100)、ConnitoA(102)、Djinn(103)、VoidAI(106)、Minos(107)、TalkHead(108)、Academia(109)、Minotaur(112)、SOMA(114)、TaoLend(116)、Satori(119)、Bitrecs(122)、Swarm(124)、8 Ball(125)、Poker44(126)、Astrid(127)

**使用本报告前，必须做的验证步骤：**
1. 访问 **https://taostats.io/subnets/{UID}/metagraph** 确认子网名称和当前运营方
2. 对比本报告记录的名称 vs taostats 实时显示的名称
3. 若不匹配，以 taostats 链上数据为准

> 链上数据是唯一可靠来源。Bittensor 生态变化极快，建议每月重新验证一次。

---

## 🚀 核心结论：最值得立即行动的机会

> ⚠️ **2026年4月13日全量验证后重大更新**：原TOP榜单中大多数子网已更换运营方，旧ROI数据完全失效。
> 以下为基于当前验证数据的更新结论。**行动前必须在 taostats.io 核查最新状态。**

### 已验证可继续研究的子网（名称未变）

| 排名 | 子网 | 类型 | 最低门槛 | 备注 |
|------|------|------|----------|------|
| 🥇 | [SN22 Desearch](subnets/SN22-desearch.md) | 社交数据 | **CPU + Twitter API** | 名称已验证，方向不变 |
| 🥈 | [SN13 Data Universe](subnets/SN13-data-universe.md) | 数据采集 | **CPU（无GPU）** | 原Dataverse改名，方向相似 |
| 🥉 | [SN07 Allways](subnets/SN07-allways.md) | 跨链交换 | CPU + TAO抵押品 | 原SubVortex，**需锁定TAO作抵押，风险增加** |

### 需重新评估的子网（名称已变，旧ROI失效）

**2026年4月14日发现：SN01-SN34 范围大规模更换运营方，以下为所有已变更子网**

| 子网 | 原名称 | 当前名称 | Alpha价格 |
|------|--------|---------|-----------|
| SN02 | Omron | **DSperse** | 0.0087 |
| SN06 | Nous Research | **Numinous** | 0.0053 |
| SN08 | Taoshi | **Vanta** | 0.0329 |
| SN09 | Pre-Training | **iota** | 0.0244 |
| SN10 | Apollo ZK | **Swap** | 0.0060 |
| SN11 | Transcription | **Trajecto...** | 0.0125 |
| SN14 | LLM Defender | **TAOHash** | 0.0089 |
| SN15 | Blockchain Insights | **ORO** | 0.0147 |
| SN17 | ThreeGen | **404—GEN** | 0.0148 |
| SN18 | Cortex.T | **Zeus** | 0.0072 |
| SN19 | Nineteen（Rayon） | **blockmac...** | 0.0140 |
| SN20 | BitAgent | **GroundLa...** | 0.0040 |
| SN21 | Omega Storage | **AdTAO** | — |
| SN23 | NicheImage | **Trishool** | 0.0042 |
| SN24 | Omega Labs | **Quasar** | 0.0147 |
| SN25 | Hivetrain | **Mainfram...** | 0.0049 |
| SN26 | Image Alchemy | **Kinitro** | 0.0038 |
| SN27 | NI Compute | **Nodexo** | 0.0045 |
| SN28 | Foundry Oracle | **Unknown** | 0.0102 |
| SN29 | Fractal | **Coldint** | 0.0140 |
| SN30 | Bettensor | **Pending** | — |
| SN31 | NAS Chain | **Halftime** | 0.0043 |
| SN42 | Masa | **Unknown** | — |

> ⚠️ 以上所有子网的历史 ROI 数据均已失效。行动前必须在 taostats.io 核查当前运营方和挖矿机制。

### 特别关注机会

| 子网 | 名称 | 原因 |
|------|------|------|
| [SN96](subnets/SN96-verathos.md) | **Verathos** | Alpha价格2.87（全网最高），排放可能异常高，高风险高机会 |
| [SN44](subnets/SN44-score.md) | **Score** | Alpha价格0.0312，$45M市值，较大排放 |

---

## ⚠️ 避开这些子网

| 子网 | 原因 |
|------|------|
| [SN64 Chutes](subnets/SN64-chutes.md) | Rayon 垄断排放，外部矿工系统性劣势 |
| [SN56 Gradient](subnets/SN56-gradient.md) | Rayon Labs 旗下，与SN64同一主体 |
| [SN03](subnets/SN03-templar.md) | ⚠️ taostats显示"deprecat..."，疑似废弃，原τemplar已消失 |
| [SN19](subnets/SN19-nineteen.md) | 原Rayon旗下Nineteen已更名为blockmac，机制未知，需重新评估 |
| SN51 lium.io | 500+ H100已入网，消费级GPU无竞争力（名称已验证：lium.io，Alpha 0.0501） |
| SN39/SN81 | taostats显示"Deprecated"，已废弃 |
| SN28 | 原Foundry Oracle，当前显示Unknown，无运营方 |
| SN55/SN57/SN78/SN82/SN84/SN117/SN118 | Deregistration 风险名单 |
| SN104 | taostats显示"for sale"，子网空置 |

---

## 文件结构

```
bittensor-research/
├── README.md                          ← 本文件（总索引）
├── summary/
│   ├── top10-mining-roi.md            ← TOP10 详细分析
│   ├── mining-feasibility.md          ← 全128子网可行性矩阵
│   └── hardware-guide.md             ← 按硬件配置推荐指南
├── data/
│   └── subnet-master-table.md        ← 汇总数据表
└── subnets/                          ← 128个子网独立研究文档
    ├── SN01-text-prompting.md
    ├── SN02-omron.md
    ├── SN03-templar.md
    ... (共128个)
    └── SN128-unknown.md
```

---

## 关键背景数据

### Bittensor 经济模型（2026年4月）

| 指标 | 数值 |
|------|------|
| TAO 总供应上限 | 21,000,000 TAO（类比比特币） |
| 当前日排放 | 3,600 TAO（2025年12月减半） |
| 下次减半 | 2026年12月（→ 1,800 TAO/天） |
| 矿工分配比例 | **41%** = ~1,476 TAO/天 |
| 验证者分配 | 41% |
| 子网所有者 | 18% |
| 当前活跃子网数 | 128个 |
| 全网子网市值合计 | ~$11.2亿（2026年3月） |

### dTAO（动态TAO）机制说明

- 每个子网有独立的 **Alpha 代币** 和 **AMM 流动性池**
- 子网排放量 = 该子网净 TAO 质押流入量决定（非固定）
- 质押流入越多 → Alpha 价格上涨 → 排放比例增加
- 这意味着**热门子网会吸引更多排放**，形成正向飞轮

### 当前最高市值子网（2026年3月）

| 排名 | 子网 | 市值 |
|------|------|------|
| 1 | SN64 Chutes (Rayon) | $132.9M |
| 2 | SN03 τemplar | $134.9M |
| 3 | SN04 Targon | $91.8M |
| 4 | SN120 Affine | $71.8M |
| 5 | SN51 Lium | $52.1M |
| 6 | SN62 Ridges AI | $50.8M |
| 7 | SN08 Taoshi | $47.4M |
| 8 | SN44 Score | $45.0M |
| 9 | SN09 iota (Pretraining) | $44.6M |
| 10 | SN75 Hippius | $41.3M |

---

## 快速行动指南

### 今天可以开始的步骤

**步骤1：安装 Bittensor 钱包**
```bash
pip install bittensor
btcli wallet new_coldkey --wallet.name myminer
btcli wallet new_hotkey --wallet.name myminer --wallet.hotkey default
```

**步骤2：检查注册费**
```bash
btcli subnet lock_cost --netuid 7  # SN07示例
```

**步骤3：充值 TAO（至少 5-20 TAO 备用）**
- 交易所购买 TAO：Binance、Coinbase、OKX
- 发送到冷钱包地址

**步骤4：注册目标子网**
```bash
btcli subnet register --netuid 7 --wallet.name myminer
```

**步骤5：启动矿工（以 SN22 Desearch 为例，当前推荐）**
```bash
# SN22 Desearch - 需 Twitter API 访问权限
# 查询当前 GitHub：搜索 "Desearch Bittensor SN22"
# 或访问 https://taostats.io/subnets/22/metagraph 找到官方链接

# SN07 Allways（需锁定TAO作抵押，高风险）
git clone https://github.com/entrius/allways
cd allways
cp .env.example .env  # 配置 PORT 和 WALLET_PATH
docker compose up miner
```

> ⚠️ **注意**：SN07 已从 SubVortex（CPU节点）变为 Allways（跨链交换），需要锁定 TAO 作为抵押品，存在 Slashing 风险，不再是纯被动收入。

---

## 实时数据查询

- **子网列表和排放**：https://taostats.io/subnets
- **矿工排名详情**：https://taostats.io/subnets/{UID}/metagraph
- **子网市值排名**：https://taomarketcap.com
- **开发者文档**：https://docs.learnbittensor.org
- **矿工社区**：Bittensor Discord

---

## 重要免责声明

1. **ROI 数据为估算**：实际收益因矿工排名、竞争动态、TAO 价格大幅波动
2. **注册费为沉没成本**：注册后无法退回，需谨慎决策
3. **dTAO 排放动态变化**：每个 epoch（~72分钟）排放量实时更新
4. **竞争快速变化**：今日低竞争子网可能快速饱和
5. **TAO 价格风险**：2026年4月 TAO 价格约 $285-320，但 TAO 已在 2026年4月创下年内新低（受 Covenant AI 退出事件影响，单日跌幅 -11%）
6. **Rayon 中心化风险**：Rayon Labs 控制约 23.7% 全网排放，是 Bittensor 去中心化的隐患

---

*报告生成于 2026年4月12日，数据可能已过时，请在 taostats.io 验证最新链上数据后再做决策。*
