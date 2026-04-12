# SN27 - NI Compute (Neural Internet Compute)

## 基本信息
| 字段 | 数据 |
|------|------|
| UID | SN27 |
| 名称 | NI Compute |
| 运营方/团队 | Neural Internet |
| 子网类型 | 去中心化 GPU 算力市场 |
| GitHub | https://github.com/neuralinternet/SN27 |
| 官网 | https://neuralinternet.ai |
| 子网状态 | 活跃 |

## 功能描述

可验证的分布式超级计算平台。矿工贡献 GPU 算力，验证者管理算力调度，用户（企业和开发者）可以租用这些 GPU 运行 ML 训练/推理任务。集成 Oracle、Coreweave、Latitude.sh 等企业级云平台。文档最完善的算力类子网之一。

## 挖矿机制

- 矿工提供 GPU 服务器，开放端口接受算力请求
- 验证者通过发送标准化算力测试评估矿工性能
- 按 GPU 性能（TFLOPS）、稳定性、响应速度综合评分
- 有机任务（真实用户请求）获得额外奖励

**端口要求**：
- 4444（验证者分配）
- 8091（Axon 服务）
- 27015-27018（外部客户端访问）

## 硬件要求

| 配置项 | 最低要求 | 推荐配置 |
|--------|----------|----------|
| GPU | RTX 3090 / A6000 | **H100 80GB / A100 80GB** |
| VRAM | 24 GB | 80 GB |
| CPU | 16核 | 32核+ |
| RAM | 64 GB | **256 GB**（推荐） |
| 存储 | 500 GB NVMe | 2 TB NVMe |
| 带宽 | 1 Gbps | 10 Gbps |
| 操作系统 | Ubuntu 22.04 | Ubuntu 22.04 |

> ⚠️ **重要限制**：
> - **不支持** Vast.ai、RunPod 等容器化云平台
> - 支持：Oracle Cloud、Coreweave、Latitude.sh 等裸金属服务器
> - 每个 UID 限制绑定一个外部 IP
> - 需要 GPU 驱动最新版本

## 经济数据（2026年4月）

| 指标 | 数值 |
|------|------|
| 排放占比 | ~1-3% |
| 注册费（TAO） | ~3-15 TAO |
| 当前矿工数 | ~100-256 |
| 子网市值 | 中 |

## ROI分析

**TAO价格基准：$300**

### 场景1：云端 H100（Oracle/Coreweave）

| 情景 | 日收益(TAO) | 月毛收益(USD) | 月成本(USD) | 月净收益(USD) |
|------|------------|--------------|------------|--------------|
| 保守 | ~0.15 | ~$1,350 | $3,000 | **-$1,650** |
| 中性 | ~0.50 | ~$4,500 | $3,000 | **+$1,500** |
| 乐观 | ~1.20 | ~$10,800 | $3,000 | **+$7,800** |

### 场景2：自有 RTX 3090（24GB）

| 情景 | 日收益(TAO) | 月毛收益(USD) | 月成本(USD) | 月净收益(USD) |
|------|------------|--------------|------------|--------------|
| 保守 | ~0.05 | ~$450 | $60（电费） | **+$390** |
| 中性 | ~0.15 | ~$1,350 | $60 | **+$1,290** |
| 乐观 | ~0.35 | ~$3,150 | $80 | **+$3,070** |

> ✅ **自有 GPU 场景 ROI 极佳！**
> RTX 3090 购买成本约 $1,200-1,500（二手），预计 1-2 个月回本（中性情景+注册费）

- **主要成本（自有GPU）**：电费 $0.1-0.2/度 × 350W × 720小时 ≈ $25-50/月
- **竞争饱和度**：**中**（H100 优于 RTX 3090，但 RTX 3090 仍可参与）
- **注册押金**：无特别要求

## 可行性评级

- **总评：🟢 立即可参与**（尤其推荐自有 GPU 用户）
- **适合人群**：
  - 有 RTX 3090/4090 等消费级高端 GPU 的矿工
  - 可以接入 Oracle Cloud/Coreweave 的用户
  - Linux 服务器运维能力强的技术人员
- **主要优势**：
  - **文档最完善的 GPU 算力子网**，新手友好
  - 性能越强收益越高，线性可扩展
  - 自有 GPU 情景下 ROI 非常可观
- **主要风险**：
  - 不支持 VastAI/RunPod 等便宜云平台
  - 网络要求严格（需稳定静态 IP）
  - H100 用户会在排名中压制 RTX 3090
- **新手难度：★★★☆☆**（需要 Linux + GPU 驱动配置能力）

## 快速开始

```bash
# 系统要求：Ubuntu 22.04，NVIDIA GPU 驱动最新版

# 1. 克隆仓库
git clone https://github.com/neuralinternet/SN27
cd SN27

# 2. 安装依赖
pip install -r requirements.txt

# 3. 配置防火墙
ufw allow 4444
ufw allow 8091
ufw allow 27015:27018/tcp

# 4. 注册矿工
btcli subnet register --netuid 27 --wallet.name miner

# 5. 启动矿工
python neurons/miner.py --netuid 27 --wallet.name miner
```

## 参考资源
- GitHub: https://github.com/neuralinternet/SN27
- 矿工指南: https://neuralinternet.ai/blog/mining
- DeepWiki: https://deepwiki.com/neuralinternet/SN27
- TaoStats: https://taostats.io/subnets/27/metagraph

## 数据采集时间
2026年4月
