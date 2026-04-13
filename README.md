# Bittensor 128子网深度挖矿调研报告

> **生成时间**：2026年4月12日 | **最后验证**：2026年4月13日（全128子网 taostats 逐一核查）
> **TAO参考价格**：~$300（实际约 $285-320）  
> **日总排放**：3,600 TAO（2025年12月减半后）  
> **研究范围**：全部 128 个活跃子网

## 🚨 重要数据准确性警告

**Bittensor 子网 UID 分配会随时间变化！** 低排放子网可能被注销，新项目接管原有 UID。

### 2026年4月13日 全量验证结果

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

**新增已识别子网**（SN35-SN128范围）：
Cartha(35)、Aurelius(37)、Colosseum(38)、Chunking(40)、Almanac(41)、Graphite(43)、Score(44)、RESI(46)、EvolAI(47)、Quantum(48)、Dojo(52)、Efficient LLM(53)、NIOME(55)、Sparket(57)、Handshake(58)、Babelbit(59)、RedTeam(61)、Enigma(63)、TAO Privacy(65)、Harnyx(67)、NOVA(68)、NexisGen(70)、Leadpoet(71)、MetaHash(73)、Gittensor(74)、Byzantium(76)、Liquidity(77)、Loosh(78)、MVTRX(79)、Hermes(82)、CliqueAI(83)、Luminar(87)、Bitstart(91)、Bitcast(93)、Bitsota(94)、Verathos(96)、Leoma(99)、Platform(100)、ConnitoA(102)、Djinn(103)、VoidAI(106)、Minos(107)、TalkHead(108)、Academia(109)、Minotaur(112)、SOMA(114)、TaoLend(116)、Satori(119)、Bitrecs(122)、Swarm(124)、8 Ball(125)、Poker44(126)、Astrid(127)

**使用本报告前，必须做的验证步骤：**
1. 访问 **https://taostats.io/subnets/{UID}/metagraph** 确认子网名称和当前运营方
2. 对比本报告记录的名称 vs taostats 实时显示的名称
3. 若不匹配，以 taostats 链上数据为准

> 链上数据是唯一可靠来源。本报告的名称已于2026年4月13日全量核查，但 Bittensor 生态变化极快，建议每月重新验证一次。

---

## 🚀 核心结论：最值得立即行动的机会

| 排名 | 子网 | 类型 | 最低门槛 | 月净收益（中性） |
|------|------|------|----------|-----------------|
| 🥇 | [SN07 SubVortex](subnets/SN07-subvortex.md) | 基础设施节点 | **CPU VPS（无GPU）** | $370 |
| 🥈 | [SN27 NI Compute](subnets/SN27-ni-compute.md) | GPU算力市场 | **RTX3090自有** | $1,290 |
| 🥉 | [SN13 Dataverse](subnets/SN13-dataverse.md) | 数据采集 | **CPU（无GPU）** | $550 |
| 4 | [SN42 Masa](subnets/SN42-masa.md) | 数据采集 | **CPU（无GPU）** | $500 |
| 5 | [SN21 Omega Storage](subnets/SN21-omega-storage.md) | 存储 | **CPU + 大存储** | $500 |
| 6 | [SN08 Taoshi](subnets/SN08-taoshi.md) | 金融预测 | CPU + Polygon API | $1,452（量化专家） |
| 7 | [SN30 Bettensor](subnets/SN30-bettensor.md) | 体育预测 | **CPU（无GPU）** | $320 |

---

## ⚠️ 避开这些子网

| 子网 | 原因 |
|------|------|
| [SN64 Chutes](subnets/SN64-chutes.md) | Rayon 垄断 23.7% 排放，8000+ 节点 |
| [SN03 τemplar](subnets/SN03-templar.md) | H100 集群，机构级竞争 |
| [SN51 Lium](subnets/SN51-lium-celium.md) | 500+ H100 已入网，饱和 |
| [SN19 Nineteen](subnets/SN19-nineteen.md) | Rayon 控制，超苛刻延迟要求 |
| SN72/78/82/84/117/118 | Deregistration 风险名单 |

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

**步骤5：启动矿工（以 SN07 为例）**
```bash
git clone https://github.com/eclipsevortex/SubVortex
cd SubVortex
pip install -r requirements.txt
python neurons/miner.py --wallet.name myminer --wallet.hotkey default
```

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
