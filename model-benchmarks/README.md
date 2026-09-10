# 📊 模型评测多维度对比

> 持续追踪市面主流模型的评测结果 | 前十名多维度对比

---

## 目录

1. [大模型综合榜](./llm-leaderboard.md)
2. [小模型专精榜](./small-model-leaderboard.md)
3. [代码能力榜](./code-capability.md)
4. [推理能力榜](./reasoning-capability.md)
5. [学术论文榜](./academic-papers.md)

---

## 综合评测维度

| 维度 | 主要评测标准 |
|------|--------------|
| **代码能力** | LeetCode, HumanEval, MBPP |
| **推理能力** | 数学、逻辑、 ARC |
| **知识广度** | MMLU, BigBench |
| **长上下文** |大海捞针、VMPR|
| **中文能力** | CMMLU, C-Eval |
| **工具使用** | API 调用、函数执行 |
| **Agent 能力** | 任务规划、自主执行 |

---

## 小模型专精榜 (重点关注)

### 评选标准

- **参数**: < 30B
- **专精领域**: 代码/数学/推理/特定任务
- **性价比**: 能力/资源消耗

### 推荐小模型

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Qwen2.5-Coder | 32B | 代码生成 | ⭐⭐⭐⭐ | 开源最强代码模型 |
| DeepSeek-Coder | 33B | 代码+推理 | ⭐⭐⭐⭐ | 推理能力强 |
| CodeLlama | 34B | 代码 | ⭐⭐⭐ | Meta 出品 |
| Phi-3 | 14B | 微软优化 | ⭐⭐⭐ | 小巧高效 |

---

## 更新记录

| 日期 | 更新内容 |
|------|----------|
| 2025-03-31 | 初始版本 |
| 2026-05-11 | 更新 Hugging Face trending 模型、排行榜信息 |
| 2026-05-25 | 更新 GitHub Trending AI 项目、主流模型动态 |
| 2026-06-08 | 更新 Hugging Face trending 代码模型 |
| 2026-06-15 | 更新 Papers with Code trending 论文、SkillOpt / Agents' Last Exam |
| 2026-06-26 | 更新 Hugging Face 代码模型排名、GitHub Trending |
| 2026-07-06 | 更新 Hugging Face trending 模型、DeepSeek-V4-Pro/GLM-5.2 新上线 |
| 2026-07-13 | 更新 Hugging Face trending 模型、ArXiv 新评测基准论文 |
| 2026-07-19 | 更新 Hugging Face trending 模型、Bonsai/Ornith/Agents-A1 新上线、SEED 论文 |
| 2026-08-17 | 更新 GPT-5.6 发布、Hugging Face trending 模型全面更新、Qwen3.8 系列崛起 |
| 2026-07-27 | 更新 Hugging Face trending 模型、Qwen3 系列、Abot-World-0/Mage-Flow 论文 |

---

## 2026 年 07 月学术前沿 (ArXiv 新论文) - 2026-07-27 更新

### 世界模型与交互

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **ABot-World-0: Infinite Interactive World Rollout on a Single Desktop GPU** | - | 单 RTX 5090 GPU 实现 720P 16FPS 视频生成，1.2s 延迟，19GiB 显存 |
| **Mage-Flow: Native-Resolution Foundation Model** | - | 4B 规模图像生成与编辑，A100 上 0.59s 生成 1024x1024 图像 |

### OCR 与文档理解

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Unlimited OCR Works** | 百度 | Reference Sliding Window Attention 消除长序列 OCR 内存增长 |

### 3D 重建

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Geometric Context Transformer for Streaming 3D Reconstruction** | - | LingBot-Map 前馈 3D 基础模型，20FPS 实时重建 |

### 金融领域

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Kronos: Foundation Model for Financial Markets** | - | 金融 K 线数据专用预训练框架 |

### Agent 强化学习与技能优化

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **SEED: Self-Evolving On-Policy Distillation** | - | 将轨迹转化为 hindsight skills 并蒸馏回策略模型 |
| **SkillOpt: Executive Strategy for Self-Evolving Agent Skills** | - | 文本空间优化器，零部署推理开销 |

---

## 2026 年 07 月学术前沿 (ArXiv 新论文) - 2026-07-19 更新

### Agent 强化学习与技能优化

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **SEED: Self-Evolving On-Policy Distillation** | - | 将轨迹转化为 hindsight skills 并蒸馏回策略模型，解决 token 级监督缺失问题 |
| **SkillOpt: Executive Strategy for Self-Evolving Agent Skills** | - | 文本空间优化器，将技能训练为外部 Agent 状态，零部署推理开销 |

### 世界模型与物理 AI

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Kairos: A Native World Model Stack for Physical AI** | - | 混合时间注意力机制，跨硬件平台高效运行 |
| **Infinite Worlds with Versatile Interactions** | - | 高级世界建模系统，多 Agent 行为控制 |

### Agent 强化学习与技能优化

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **SEED: Self-Evolving On-Policy Distillation** | - | 将轨迹转化为 hindsight skills 并蒸馏回策略模型，解决 token 级监督缺失问题 |
| **SkillOpt: Executive Strategy for Self-Evolving Agent Skills** | - | 文本空间优化器，将技能训练为外部 Agent 状态，零部署推理开销 |

### 世界模型与物理 AI

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Kairos: A Native World Model Stack for Physical AI** | - | 混合时间注意力机制，跨硬件平台高效运行 |
| **Infinite Worlds with Versatile Interactions** | - | 高级世界建模系统，多 Agent 行为控制 |

### 语音与音频

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Continuous Audio Language Models (CALM)** | - | 避免有损压缩，低计算成本实现更高质量和保真度 |
| **GigaChat3.1-Audio-10B-A1.8B** | - | 俄语语音模型，10B 参数 1.8B 激活 |

### OCR 与文档理解

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Unlimited OCR Works** | 百度 | Reference Sliding Window Attention 消除长序列 OCR 内存增长 |
| **VideoChat3: Fully Open Video MLLM** | - | 全开源高效视频理解，I3D-ViT + 自适应帧分辨率 |

### Agent 与多 Agent 系统

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **UniClawBench** | - | 通用主动 Agent 基准，真实世界任务评测 |
| **Game Theory Driven Multi-Agent** | - | 博弈论框架减少 LLM 幻觉 |
| **Who Broke the System?** | - | LLM 多 Agent 系统失败定位 |
| **MASTE** | - | 多 Agent 流水线零样本方面情感三元组提取 |

### 评测基准

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **AUTOPILOT VQA** | - | 事故中心视觉语言模型评测 |
| **OmniFood-Bench** | - | VLMs 营养推理与个性化健康建议 |
| **CausalDS** | - | 数据科学 Agent 因果推理基准 |
| **PredicateLongBench** | - | 长上下文任务难度轴分析 |
| **MentalHospital** | - | 精神科临床对话虚拟环境 |

### 优化与效率

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Resample or Reroute?** | - | 预算感知测试时间模型选择 |
| **What to Keep, What to Forget** | - | LLM 记忆压缩的率-失真视角 |
| **Tail-Aware Credit Calibration** | - | RL 强化学习尾部感知信用校准 |
| **Efficient Safety Alignment** | - | 潜在人格特质高效安全对齐 |

### 安全与可解释性

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Mechanistic Interpretability of Jailbreaks** | - | LLM 越狱的内部归因图可解释性 |
| **Functional and Secure Code Generation** | - | 任务向量功能安全代码生成 |
| **Efficient Safety Alignment** | - | 潜在人格特质安全对齐 |

### 多模态与视觉语言

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **WCog-VLA** | - | 端到端自动驾驶世界认知 VLA 模型 |
| **Attribute Retrieving** | - | 开放词汇内镜组合引用分割 |
| **COALA** | - | ASR 语音增强语言建模 |
| **LUMI** | - | 基于 LLM 的无损图像压缩 |

---

## 2026 年 06 月学术前沿 (Papers with Code Trending) - 2026-06-29 更新

### 图像修复与高效模型

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Moebius** | - | 0.2B 轻量图像修复框架，<2% 参数达到 10B 级性能，15x 推理加速 |
| **MobileForge** | 快手 AI | 无标注移动 GUI Agent 适配，HiFPO 分层反馈优化 |

### Agent 技能优化

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **SkillOpt** | - | 文本空间优化器, 将技能训练为外部 Agent 状态, 零部署开销 |
| **SIA** | Hexo AI | 同步更新模型权重 + 任务特定 Agent 架构 |
| **Agents' Last Exam (ALE)** | - | 经济价值任务基准, 13 行业集群 1K+ 任务 |

### 多模态与世界模型

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Cosmos 3** | NVIDIA |  omnimodal 世界模型, 统一 MoT 架构 |
| **InterleaveThinker** | - | 多 Agent 流水线, 图像生成 interleaved 能力 |

### 长上下文优化

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **MiniMax Sparse Attention** | MiniMax | 块稀疏优化, 超长上下文高效处理 |

### 记忆系统

| 论文 | 机构 | 核心贡献 |
|------|------|----------|
| **Mem0** | - | 图基记忆, 长期对话一致性, 优于现有记忆系统 |

---

## 2026 年 07 月主流模型动态 - 2026-07-27 更新

### Hugging Face Trending 文本生成模型 (Top 20)

| 排名 | 模型 | 参数量 | 下载量 | 备注 |
|------|------|--------|-------|------|
| 1 | **Qwen/Qwen3-0.6B** | 0.8B | 28.5M | 🆕 Qwen3 最小的模型 |
| 2 | **Qwen/Qwen3-8B** | 8B | 16.8M | 🆕 Qwen3 基础版 |
| 3 | **facebook/opt-125m** | 0.1B | 16.7M | 经典小模型 |
| 4 | **Qwen/Qwen2.5-1.5B-Instruct** | 2B | 13.3M | 指令模型 |
| 5 | **Qwen/Qwen2.5-7B-Instruct** | 8B | 12M | 主力模型 |
| 6 | **meta-llama/Llama-3.2-1B-Instruct** | 1B | 10.3M | Llama 小模型 |
| 7 | **Qwen/Qwen3-32B** | 33B | 10.1M | 🆕 Qwen3 大杯 |
| 8 | **nvidia/Qwen3.6-35B-A3B-NVFP4** | 19B | 9.59M | NVIDIA 优化版 |
| 9 | **deepseek-ai/DeepSeek-R1** | 685B | 8.93M | 推理旗舰 |
| 10 | **meta-llama/Llama-3.1-8B-Instruct** | 8B | 8.04M | Llama 3.1 |
| 11 | **openai/gpt-oss-20b** | 22B | 7.93M | OpenAI 开源 |
| 12 | **Qwen/Qwen3-1.7B** | 2B | 6.97M | 🆕 Qwen3 中杯 |
| 13 | **Qwen/Qwen2.5-3B-Instruct** | 3B | 5.72M | 中型指令模型 |
| 14 | **Qwen/Qwen3-4B** | 4B | 4.83M | 🆕 Qwen3 小杯 |
| 15 | **deepseek-ai/DeepSeek-V4-Flash** | 158B | 3.12M | 高效版本 |
| 16 | **deepreinforce-ai/Ornith-1.0-9B-GGUF** | 9B | 3.75M | 高效量化 |
| 17 | **ibm-granite/granite-4.1-8b** | 9B | 3.38M | IBM Granite |
| 18 | **Qwen/Qwen3-14B** | 15B | 3.24M | 🆕 Qwen3 中大杯 |
| 19 | **zai-org/GLM-5.2-FP8** | 753B | 3.14M | 智谱高效版 |
| 20 | **openai/gpt-oss-120b** | 120B | 4.38M | OpenAI 大杯 |

### Qwen3 系列更新 (阿里)

Qwen3 系列成为 Hugging Face 下载量最高的模型系列:

| 模型 | 参数 | 下载量 | 特点 |
|------|------|--------|------|
| Qwen3-0.6B | 0.8B | 28.5M | 最小模型，边缘设备 |
| Qwen3-8B | 8B | 16.8M | 主力模型 |
| Qwen3-32B | 33B | 10.1M | 大杯模型 |
| Qwen3-1.7B | 2B | 6.97M | 中杯模型 |
| Qwen3-4B | 4B | 4.83M | 小杯模型 |
| Qwen3-14B | 15B | 3.24M | 中大杯模型 |

---

## 2026 年 07 月主流模型动态 - 2026-07-19 更新

### Hugging Face Trending 文本生成模型 (Top 15)

| 排名 | 模型 | 参数量 | 下载量 | 备注 |
|------|------|--------|-------|------|
| 1 | **Ternary-Bonsai-27B-gguf** | 4B | 339k | 🆕 高效量化模型 |
| 2 | **Bonsai-27B-gguf** | 4B | 1.26M | 🆕 高效量化模型 |
| 3 | **GLM-5.2** | 753B | 536k | 智谱最新 |
| 4 | **Hy3** | 295B | 110k | 🆕 腾讯大模型 |
| 5 | **MiniCPM5-1B-Claude-Opus-Fable5-Thinking** | 1B | 5.49k | 🆕 Claude 风格 |
| 6 | **Bonsai-27B-mlx-1bit** | 2B | 21.7k | 🆕 MLX 1bit 量化 |
| 7 | **Hy3-GGUF** | 295B | 110k | 🆕 高效版本 |
| 8 | **Agents-A1** | 35B | 35.8k | 🆕 Agent 专用 |
| 9 | **Ornith-1.0-35B-GGUF** | 35B | 1.87M | 🆕 新兴模型 |
| 10 | **Qwythos-9B-v2** | 10B | 9.53k | 🆕 改进版本 |
| 11 | DeepSeek-V4-Pro | 862B | 1.49M | 多模态旗舰 |
| 12 | DeepSeek-V4-Flash | 158B | 2.96M | 高效版本 |
| 13 | Ornith-1.0-9B | 9B | 2.35M | 轻量版本 |
| 14 | MiniCPM5-1B | 1B | 408k | 面壁小钢炮 |
| 15 | **Soofi-S-Base** | 32B | 95 | 🆕 新兴模型 |

### 新上线重点模型

#### Ternary-Bonsai / Bonsai (Prism-ML)
- **参数量**: 4B (27B 量化到 4B)
- **下载量**: 339k / 1.26M
- **特点**: 高效量化模型，GGUF 格式支持本地部署

#### Hy3 (腾讯)
- **参数量**: 295B
- **下载量**: 110k
- **特点**: 腾讯最新大模型，多模态能力

#### Ornith-1.0 (DeepReinforce AI)
- **参数量**: 35B / 9B
- **下载量**: 1.87M / 2.35M
- **特点**: 新兴模型系列，35B 和 9B 双版本

#### Agents-A1 (InternScience)
- **参数量**: 35B
- **下载量**: 35.8k
- **特点**: Agent 专用模型，任务规划与执行

#### GLM-5.2 (智谱 AI)
- **参数量**: 753B
- **下载量**: 536k
- **特点**: 智谱最新更新

### 小模型专精榜 (更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Ternary-Bonsai-27B | 4B | 高效量化 | ⭐⭐⭐⭐ | GGUF 格式 |
| Bonsai-27B | 4B | 高效量化 | ⭐⭐⭐⭐ | 多种格式 |
| Ornith-1.0-9B | 9B | 通用 | ⭐⭐⭐⭐ | 高下载量 |
| Agents-A1 | 35B | Agent | ⭐⭐⭐⭐ | 专用模型 |
| MiniCPM5-1B | 1B | 轻量 | ⭐⭐⭐⭐ | 面壁小钢炮 |

#### Agents-A1 (InternScience)
- **参数量**: 35B
- **下载量**: 502k
- **特点**: Agent 专用模型

#### Unlimited-OCR (百度)
- **参数量**: 3B
- **下载量**: 1.94M
- **特点**: 百度最新 OCR 模型

#### ThinkingCap-Qwen3.6-27B
- **参数量**: 27B
- **下载量**: 250k
- **特点**: 推理优化版本

### 新上线重点模型

#### DeepSeek-V4-Pro (深度求索)
- **参数量**: 862B
- **下载量**: 1.23M
- **特点**: DeepSeek 最新多模态旗舰

#### GLM-5.2 (智谱 AI)
- **参数量**: 753B
- **下载量**: 220k
- **特点**: 智谱最新模型，3天前上线

#### gpt-oss 系列 (OpenAI)
- **gpt-oss-120b**: 120B, 4.18M 下载
- **gpt-oss-20b**: 22B, 6.92M 下载
- **特点**: OpenAI 开源系列

#### phi-2 (微软)
- **参数量**: 3B
- **下载量**: 785k
- **特点**: 微软小模型更新

### 小模型专精榜 (更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Qwen2.5-Coder | 32B | 代码生成 | ⭐⭐⭐⭐ | 开源最强代码模型 |
| DeepSeek-R1 | 685B | 推理 | ⭐⭐⭐⭐⭐ | 下载量最高 |
| QwQ-32B | 33B | 推理 | ⭐⭐⭐⭐ | 阿里推理模型 |
| Kimi-K2-Instruct | 1T | 长上下文 | ⭐⭐⭐⭐ | 月之暗面 |
| phi-2 | 3B | 轻量 | ⭐⭐⭐ | 微软最小 |

---

## 2026 年 06 月主流模型动态

### Hugging Face Trending 代码模型 (Top 15)

| 排名 | 模型 | 参数量 | 下载量 | 备注 |
|------|------|--------|-------|------|
| 1 | Qwen2.5-Coder-14B | 15B | 4.67M | 下载量最高 |
| 2 | Qwen3-Coder-30B-A3B | 31B | 2.05M | MoE 高效版本 |
| 3 | Qwen2.5-Coder-7B | 8B | 2.03M | 小型强力 |
| 4 | Qwen3-Coder-Next-FP8 | 80B | 1.73M | 阿里最新代码模型 |
| 5 | Qwen2.5-Coder-32B | 33B | 1.63M | 开源经典代码模型 |
| 6 | DeepSeek-Coder-V2-Lite | 16B | 1.17M | 轻量高效 |
| 7 | Qwen3-Coder-Next | 80B | 1.17M | 完整版本 |
| 8 | Qwen2.5-Coder-1.5B | 2B | 762k | 超小模型 |
| 9 | DeepSeek-Coder-7B | 7B | 591k | 经典版本 |
| 10 | DeepSeek-Coder-6.7B | 7B | 325k | 小型版本 |

### 重点模型更新

#### Qwen3-Coder-Next (阿里)
- **参数**: 80B
- **下载量**: 1.01M
- **特点**: 阿里最新代代码模型，支持更长上下文

#### Qwen3-Coder-30B-A3B
- **参数**: 31B (MoE, 激活 3B)
- **下载量**: 2.1M
- **特点**: 高性价比，推理高效

#### DeepSeek-Coder-V2-Lite
- **参数**: 16B
- **下载量**: 885k
- **特点**: 轻量高效，适合本地部署

### 代码模型评测趋势

| 模型 | HumanEval | MBPP | 趋势 |
|------|----------|------|------|
| Qwen3-Coder-Next | ~92% | ~85% | ⬆️ 上升 |
| Qwen2.5-Coder-32B | ~90% | ~82% | ➡️ 稳定 |
| DeepSeek-Coder-V2 | ~88% | ~80% | ➡️ 稳定 |
| Codestral-22B | ~85% | ~78% | ⬆️ 新进 |

---

## 2026 年 05 月主流模型动态

### Hugging Face Trending 模型 (Top 10)

| 排名 | 模型 | 参数量 | 下载量 | 特点 |
|------|------|--------|-------|------|
| 1 | SulphurAI/Sulphur-2-base | 9B | 144k | 视频生成 |
| 2 | Zyphra/ZAYA1-8B | 8B | 44.8k | 文本生成 |
| 3 | deepseek-ai/DeepSeek-V4-Pro | 862B | 1.34M | 大型多模态 |
| 4 | google/gemma-4-31B-it-assistant | 31B | 56.6k | Google 助手 |
| 5 | Qwen/Qwen3.6-27B | 28B | 2.27M | 阿里开源 |
| 6 | Qwen/Qwen3.6-35B-A3B | 36B | 3.67M | 阿里 MoE |
| 7 | google/gemma-4-26B-A4B-it | 26B | 40.9k | Google 小型 |
| 8 | deepseek-ai/DeepSeek-V4-Flash | 158B | 1.07M | 高效版本 |
| 9 | XiaomiMiMo/MiMo-V2.5-Pro | 1T | 40.1k | 小米万亿参数 |
| 10 | mistralai/Mistral-Medium-3.5-128B | 128B | 40.6k | Mistral 中型 |

### 重点模型更新

#### DeepSeek-V4 系列
- **DeepSeek-V4-Pro**: 862B 参数，1.34M 下载，顶级多模态
- **DeepSeek-V4-Flash**: 158B 参数，高效版本

#### Qwen3.6 系列 (阿里)
- **Qwen3.6-27B**: 2.27M 下载量，最热门开源模型
- **Qwen3.6-35B-A3B**: 3.67M 下载，MoE 架构

#### Google Gemma 4
- **gemma-4-31B-it**: 33B，Google 最强
- **gemma-4-26B-A4B**: 26B + A3B 蒸馏

### 小模型专精榜 (更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Qwen2.5-Coder | 32B | 代码生成 | ⭐⭐⭐⭐ | 开源最强代码模型 |
| Qwen3.6-27B | 28B | 通用 | ⭐⭐⭐⭐⭐ | 综合最强开源 |
| DeepSeek-V4-Flash | 158B | 高效推理 | ⭐⭐⭐⭐ | 性价比高 |
| gemma-4-26B-A4B | 26B | 指令跟随 | ⭐⭐⭐⭐ | Google 小型 |
| Nemotron-3-Nano-Omni | 30B | 多模态 | ⭐⭐⭐⭐ | NVIDIA |

### GitHub Trending AI 项目 (2026-05)

| 排名 | 项目 | 描述 | 趋势 |
|------|------|------|------|
| 1 | mattpocock/skills | Claude Code 工程技能 | 🔥上升 |
| 2 | codegraph | 代码知识图谱 | 🔥新贵 |
| 3 | CloakBrowser | 反检测浏览器 | 🔥新贵 |
| 4 | agentmemory | Agent 持久化内存 | 🔥上升 |
| 5 | academic-research-skills | 学术研究技能 | 🔥新贵 |
| 6 | awesome-codex-skills | Codex 技能精选 | 🔥上升 |
| 7 | free-claude-code | 免费 Claude Code | 🔥新贵 |
| 8 | andrej-karpathy-skills | Karpathy 技能 | 🔥新贵 |
| 9 | ViMax | Agentic 视频生成 | 🔥新贵 |
| 10 | 9router | 免费 AI 路由 | 🔥新贵 |

---

## 2026 年 05 月重要更新

### 模型动态

> 基于 GitHub Trending 和 Hugging Face 观测

#### DeepSeek-V4 系列
- **DeepSeek-V4-Pro**: 862B 参数，多模态旗舰
- **DeepSeek-V4-Flash**: 158B 参数，高效版本

#### Qwen3.6 系列 (阿里)
- **Qwen3.6-27B**: 最热门开源模型 (2.27M 下载)
- **Qwen3.6-35B-A3B**: MoE 架构 (3.67M 下载)

#### Google Gemma 4
- **gemma-4-31B-it**: 31B Google 助手
- **gemma-4-26B-A4B**: 26B + A3B 蒸馏

#### 其他亮点
- **SulphurAI/Sulphur-2-base**: 视频生成新秀 (144k 下载)
- **MiMo-V2.5-Pro**: 小米万亿参数 (40.1k 下载)
- **Mistral-Medium-3.5-128B**: Mistral 中型 (40.6k 下载)

### 代码能力模型

| 模型 | 参数量 | 专精领域 | 备注 |
|------|--------|----------|------|
| Qwen2.5-Coder | 32B | 代码生成 | 开源最强 |
| DeepSeek-Coder | 33B | 代码+推理 | 推理能力强 |
| CodeLlama | 34B | 代码 | Meta 出品 |
| Phi-3 | 14B | 微软优化 | 小巧高效 |

### 新兴工具/框架

#### AI 编码工具
| 工具 | 描述 | 特点 |
|------|------|------|
| **jcode** | Rust 编码 Agent | 高性能 |
| **free-claude-code** | 免费 Claude Code | 开源替代 |
| **decolua/9router** | 多平台路由器 | 40+ 提供商 |

#### Agent 编排
| 工具 | 描述 | 特点 |
|------|------|------|
| **ruflo** | 多 Agent 编排 | Claude 集成 |
| **hermes-agent** | 成长型 Agent | NousResearch |
| **TradingAgents** | 金融交易框架 | 多 Agent |

#### 浏览器/自动化
| 工具 | 描述 | 特点 |
|------|------|------|
| **CloakBrowser** | 反检测 Chromium | 30/30 通过 |
| **maigret** | OSINT 工具 | 3000+ 站点 |

---

## 2026 年 08 月主流模型动态 - 2026-08-15 更新

### Hugging Face Trending 文本生成模型 (Top 20)

| 排名 | 模型 | 参数量 | 下载量 | 备注 |
|------|------|--------|-------|------|
| 1 | **Qwen/Qwen3.8-2.4T-A95B** | 2.4T | 3.83k | 🆕 阿里最新旗舰，2天前更新 |
| 2 | **DeepSeek-V4-Flash-0731** | 304B | 1.61M | 每日更新 |
| 3 | **DeepSeek-V4-Pro-0813** | 1.7T | 245 | 🆕 Pro 版本每日更新，1天前 |
| 4 | **NVIDIA-Nemotron-3.5-Lightning-30B-A3B** | 18B | 120k | 🆕 NVIDIA 新模型 |
| 5 | **LiquidAI/LFM2.5-2.6B** | 3B | 124k | 轻量高效 |
| 6 | **Qwen3.8-2.4T-A95B-FP8** | 2.4T | 9.33k | 🆕 FP8 高效版本 |
| 7 | **NVIDIA-Nemotron-3.5-Lightning-30B-A3B-BF16** | 32B | 34.1k | BF16 精度版 |
| 8 | **deepgrove/maple-preview** | 20B | 5.62k | 🆕 新兴模型 |
| 9 | **inclusionAI/Ling-3.0-flash** | 127B | 11.3k | 🆕 新系列 |
| 10 | **Motif-3** | 315B | 1.29k | 🆕 新兴大模型，14小时前更新 |
| 11 | **unsloth/Qwen3.8-2.4T-A95B-GGUF** | 2.4T | 8.57k | GGUF 量化版 |
| 12 | **LiquidAI/LFM2.5-2.6B-GGUF** | 3B | 246k | 高效量化版 |
| 13 | **NVIDIA-Nemotron-3.5-Lightning-30B-GGUF** | 33B | 56.5k | GGUF 量化版 |
| 14 | **zai-org/GLM-5.2** | 753B | 2.69M | 智谱最新 |
| 15 | **huihui-ai/Huihui-CyberStrike-OffSec-35B** | 36B | 1.24k | 🆕 安全研究专用 |
| 16 | **webAI-Official/TwIL-LM3** | 3B | 13.1k | 🆕 实时更新 |
| 17 | **Kwaipilot/KAT-Coder-V2.5-Dev** | 35B | 22.5k | 代码模型 |
| 18 | **DeepSeek-V4-Pro** | 1.6T | 1.35M | 多模态旗舰 |
| 19 | **poolside/Laguna-S-2.1** | 118B | 112k | 新兴模型 |
| 20 | **prism-ml/Ternary-Bonsai-27B-gguf** | 27B | 822k | 高效量化 |

### 新上线重点模型

#### Qwen3.8-2.4T-A95B (阿里)
- **参数量**: 2.4T (激活 95B)
- **下载量**: 3.83k
- **特点**: 阿里最新旗舰模型，2天前更新
- **格式**: FP8, GGUF, BF16 多版本

#### DeepSeek-V4-Pro-0813 (深度求索)
- **参数量**: 1.7T
- **下载量**: 245
- **特点**: Pro 版本每日更新，1天前
- **更新时间**: 2026-08-14

#### NVIDIA-Nemotron-3.5-Lightning-30B (NVIDIA)
- **参数量**: 30B (激活 3B)
- **下载量**: 120k
- **特点**: NVIDIA 最新高效模型，BF16 + NVFP4 双版本
- **更新时间**: 23 小时前

#### Motif-3 (Motif Technologies)
- **参数量**: 315B
- **下载量**: 1.29k
- **特点**: 新兴大模型，14小时前更新
- **更新时间**: 2026-08-14

#### LiquidAI/LFM2.5-2.6B (Liquid AI)
- **参数量**: 3B
- **下载量**: 124k (基础版) / 246k (GGUF)
- **特点**: 轻量高效，GGUF 量化版更受欢迎

#### inclusionAI/Ling-3.0-flash (Inclusion AI)
- **参数量**: 127B
- **下载量**: 11.3k
- **特点**: 新系列 Flash 版本

### 小模型专精榜 (更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Qwen3.8-2.4T | 2.4T | 通用旗舰 | ⭐⭐⭐⭐⭐ | 阿里最新旗舰 |
| NVIDIA-Nemotron-3.5-Lightning | 30B | 高效 | ⭐⭐⭐⭐⭐ | NVIDIA 优化版 |
| LiquidAI/LFM2.5-2.6B | 3B | 轻量 | ⭐⭐⭐⭐ | 高效量化 |
| Ternary-Bonsai-27B | 4B | 高效量化 | ⭐⭐⭐⭐ | GGUF 822k 下载 |
| GLM-5.2 | 753B | 通用 | ⭐⭐⭐⭐ | 2.69M 下载 |

### 模型趋势分析 (2026-08)

1. **阿里 Qwen3.8 系列**: 2.4T 旗舰模型发布，FFN 激活参数达 95B，多种格式支持
2. **NVIDIA Nemotron 系列**: 30B 激活 3B 高效架构，BF16/NVFP4 双精度
3. **DeepSeek 持续更新**: Flash 版本每日迭代，Pro 版本频繁更新
4. **量化模型流行**: GGUF 格式下载量持续增高 (LiquidAI LFM2.5 246k, Ternary-Bonsai 822k)
5. **新兴模型涌现**: Motif-3 (315B), deepgrove/maple-preview (20B), inclusionAI/Ling-3.0-flash (127B)

---

## 2026 年 08 月主流模型动态 - 2026-08-03 更新

### Hugging Face Trending 文本生成模型 (Top 20)

| 排名 | 模型 | 参数量 | 下载量 | 备注 |
|------|------|--------|-------|------|
| 1 | **moonshotai/Kimi-K3** | 2.8T | 837k | 🆕 全新多模态模型 |
| 2 | **DeepSeek-V4-Flash-0731** | 304B | 156k | 🆕 每日更新 |
| 3 | **Qwen3.6-27B-Fable-Fusion** | 27B | 1.37M | 定制融合版 |
| 4 | **baidu/Unlimited-OCR** | 3B | 2.54M | 百度 OCR 模型 |
| 5 | **Kimi-K3-GGUF** | 2.8T | 88.5k | 🆕 高效量化版 |
| 6 | **zai-org/GLM-5.2** | 753B | 2.05M | 智谱最新 |
| 7 | **thinkingmachines/Inkling-Small** | 266B | 6.84k | 🆕 新兴模型 |
| 8 | **Inflect-Micro-v2** | - | 1.83k | TTS 模型 |
| 9 | **KAT-Coder-V2.5-Dev** | 35B | 13.2k | 代码模型 |
| 10 | **Nanbeige4.2-3B** | 4B | 33k | 🆕 中文字词模型 |
| 11 | **microsoft/Mage-VL** | 5B | 272k | 微软多模态 |
| 12 | **poolside/Laguna-S-2.1** | 118B | 80.1k | 🆕 新兴模型 |
| 13 | **Audio8-TTS-Preview** | 0.6B | 4.31k | TTS 预览版 |
| 14 | **microsoft/Fara1.5-27B** | 27B | 2.94k | 🆕 微软模型 |
| 15 | **XYZ-Aquila-mini** | 35B | 903 | 🆕 新兴模型 |
| 16 | **Qwen3.6-35B-A3B** | 35B | 259k | 阿里 MoE |
| 17 | **Solar-Open2-250B** | 250B | 14.9k | 🆕 Upstage 模型 |
| 18 | **DeepSeek-V4-Flash** | 158B | 2.79M | 高效版本 |
| 19 | **XYZ-Aquila-pro** | 397B | 1.09k | 🆕 大杯版本 |
| 20 | **thinkingmachines/Inkling** | 952B | 63.3k | 大杯版本 |

### 新上线重点模型

#### Kimi-K3 (Moonshot AI)
- **参数量**: 2.8T (可能是激活参数)
- **下载量**: 837k
- **特点**: 全新多模态模型，Image-Text-to-Text 任务
- **更新时间**: 6 天前

#### DeepSeek-V4-Flash-0731 (深度求索)
- **参数量**: 304B
- **下载量**: 156k
- **特点**: 每日更新的 Flash 版本
- **更新时间**: 1 天前

#### Unlimited-OCR (百度)
- **参数量**: 3B
- **下载量**: 2.54M
- **特点**: 百度最强 OCR 模型，支持多种格式
- **更新时间**: 4 天前

#### Inkling (Thinking Machines)
- **参数量**: 952B
- **下载量**: 63.3k
- **特点**: 新兴大模型系列
- **更新时间**: 10 天前

#### Solar-Open2-250B (Upstage)
- **参数量**: 250B
- **下载量**: 14.9k
- **特点**: Upstage 最新大模型
- **更新时间**: 2 天前

### 小模型专精榜 (更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Kimi-K3 | 2.8T | 多模态 | ⭐⭐⭐⭐⭐ | Moonshot 最新 |
| Unlimited-OCR | 3B | OCR | ⭐⭐⭐⭐⭐ | 百度最强 |
| Qwen3.6-35B-A3B | 35B | 通用 | ⭐⭐⭐⭐ | 阿里 MoE |
| DeepSeek-V4-Flash | 158B | 高效 | ⭐⭐⭐⭐ | 性价比高 |
| Inkling-Small | 266B | 通用 | ⭐⭐⭐⭐ | 新兴模型 |

---

## 数据来源

- [GitHub Trending](https://github.com/trending)
- [Hugging Face](https://huggingface.co/)
- [ArXiv](https://arxiv.org/)

---

> ⚠️ 注意: 排行榜权重不同，对比时请关注同一评测标准。持续更新中...

---

---

## 2026 年 08 月主流模型动态 - 2026-08-24 更新

### Hugging Face Trending 文本生成模型 (Top 20)

| 排名 | 模型 | 参数量 | 下载量 | 趋势 | 备注 |
|------|------|--------|--------|------|------|
| 1 | **Qwen3.8-27B-OBLITERATED** | 28B | 245k | 🆕 | 12小时前更新 |
| 2 | **Qwen3.8-27B-Uncensored-GGUF** | 27B | 1.33M | → | 未经审查版本 |
| 3 | **Ornith-1.5-35B-A3B** | 36B | 23.5k | 🆕 | 13小时前更新 |
| 4 | **Ornith-1.5-35B-A3B-GGUF** | 36B | 369k | 🆕 | 4天前更新 |
| 5 | **DeepSeek-V4-Flash-0731** | 304B | 3.09M | → | 高效版本持续热门 |
| 6 | **Ornith-1.5-9B** | 10B | 31.5k | 🆕 | 10小时前更新 |
| 7 | **DeepSeek-V4-Pro-0813** | 1.7T | 57.9k | → | Pro 版本 |
| 8 | **Ornith-1.5-9B-GGUF** | 9B | 359k | → | 高效量化版 |
| 9 | **Qwen3.8-27B-Heretic-Abliterated-GGUF** | 27B | 579k | 🆕 | 3天前更新 |
| 10 | **Qwen3.8-2.4T-A95B** | 2.4T | 18.1k | → | 阿里旗舰 |
| 11 | **NVIDIA-Nemotron-3.5-Lightning-30B-A3B-NVFP4** | 18B | 582k | 🆕 | NVIDIA 优化版 |
| 12 | **LiquidAI/LFM2.5-2.6B-GGUF** | 3B | 520k | → | 高效量化版 |
| 13 | **zai-org/GLM-5.2** | 753B | 2.69M | → | 智谱最新 |
| 14 | **Ornith-1.5-397B** | 403B | 7.91k | 🆕 | 大杯版本 |
| 15 | **inclusionAI/Ling-3.0-tiny** | 8B | 14.5k | 🆕 | 4天前更新 |

### 新上线重点模型

#### Ornith-1.5 系列 (DeepReinforce AI)
- **Ornith-1.5-35B-A3B**: 36B 参数，23.5k 下载，13小时前更新
- **Ornith-1.5-35B-A3B-GGUF**: 369k 下载，高效量化版
- **Ornith-1.5-9B**: 10B 参数，31.5k 下载，10小时前更新
- **Ornith-1.5-397B**: 403B 参数，大杯版本

#### Qwen3.8 生态持续扩张

| 模型 | 参数量 | 格式 | 下载量 |
|------|--------|------|--------|
| Qwen3.8-27B-OBLITERATED | 28B | 原生 | 245k |
| Qwen3.8-27B-Uncensored-GGUF | 27B | GGUF | 1.33M |
| Qwen3.8-27B-Heretic-Abliterated-GGUF | 27B | GGUF | 579k |
| Qwen3.8-2.4T-A95B | 2.4T | 原生/FP8 | 18.1k |

#### NVIDIA-Nemotron-3.5-Lightning-30B
- **参数量**: 30B (激活 3B)
- **下载量**: 582k (NVFP4 版本)
- **特点**: NVIDIA 原生优化，多种量化格式

### 模型趋势分析 (2026-08-24)

1. **Ornith-1.5 系列全面更新**: DeepReinforce AI 密集发布 35B/9B/397B 多版本，GGUF 格式下载量持续攀升

2. **Qwen3.8 生态扩张**: 多种微调/量化版本涌现 (OBLITERATED/Uncensored/Heretic/Abliterated)，反映社区活跃度

3. **量化模型统治下载量**: GGUF 格式持续霸榜
   - Qwen3.8-27B-Uncensored-GGUF: 1.33M
   - Ornith-1.5-35B-A3B-GGUF: 369k
   - Ornith-1.5-9B-GGUF: 359k

4. **上下文数据库整合**: OpenViking 等工具推动长上下文模型需求

### 小模型专精榜 (2026-08-24 更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Ornith-1.5-35B-A3B | 36B | 通用 | ⭐⭐⭐⭐⭐ | 新版本密集发布 |
| Qwen3.8-27B | 28B | 通用旗舰 | ⭐⭐⭐⭐ | 多种微调版本 |
| NVIDIA-Nemotron-3.5-Lightning | 30B | 高效推理 | ⭐⭐⭐⭐⭐ | NVIDIA 原生优化 |
| LiquidAI/LFM2.5-2.6B | 3B | 轻量高效 | ⭐⭐⭐⭐ | GGUF 520k 下载 |
| DeepSeek-V4-Flash | 304B | 高效推理 | ⭐⭐⭐⭐ | 3.09M 下载 |

---

---

## 2026 年 08 月主流模型动态 - 2026-08-31 更新

### Hugging Face Trending 文本生成模型 (Top 20)

| 排名 | 模型 | 参数量 | 下载量 | 趋势 | 备注 |
|------|------|--------|--------|------|------|
| 1 | **Qwen/Qwen3-0.6B** | 0.8B | 22.5M | → | Qwen3 最小模型 |
| 2 | **trl-internal-testing/tiny-Qwen2ForCausalLM-2.5** | 2.43M | 16.6M | 🆕 | 测试模型 |
| 3 | **openai-community/gpt2** | 0.1B | 14.4M | → | 经典模型 |
| 4 | **Qwen/Qwen3-8B** | 8B | 13.7M | → | Qwen3 基础版 |
| 5 | **unsloth/Qwen3-Coder-30B-A3B-Instruct-GGUF** | 31B | 12.8M | → | 高效量化版 |
| 6 | **facebook/opt-125m** | 0.1B | 11.4M | → | 经典小模型 |
| 7 | **nvidia/Qwen3.6-35B-A3B-NVFP4** | 19B | 11.2M | 🆕 | NVIDIA 优化版, 1天前更新 |
| 8 | **Qwen/Qwen2.5-7B-Instruct** | 8B | 10.8M | → | 指令模型 |
| 9 | **Qwen/Qwen2.5-1.5B-Instruct** | 2B | 7.87M | → | 小型指令模型 |
| 10 | **Qwen/Qwen2.5-3B-Instruct** | 3B | 7.51M | → | 中型指令模型 |
| 11 | **farbodtavakkoli/OTel-2.0-LLM-31B-IT** | 32B | 6.79M | 🆕 | 6天前更新 |
| 12 | **meta-llama/Llama-3.2-1B-Instruct** | 1B | 6.66M | → | Llama 小模型 |
| 13 | **openai/gpt-oss-20b** | 21B | 6.52M | → | OpenAI 开源 |
| 14 | **Qwen/Qwen2.5-0.5B-Instruct** | 0.5B | 6.29M | → | 超小模型 |
| 15 | **meta-llama/Llama-3.1-8B-Instruct** | 8B | 5.94M | → | Llama 3.1 |
| 16 | **openai/gpt-oss-120b** | 117B | 5.31M | → | OpenAI 大杯 |
| 17 | **Qwen/Qwen3-4B** | 4B | 5.25M | → | Qwen3 小杯 |
| 18 | **Qwen/Qwen3-32B** | 33B | 4.82M | → | Qwen3 大杯 |
| 19 | **dphn/dolphin-2.9.1-yi-1.5-34b** | 34B | 4.81M | → | Yi 系列微调 |
| 20 | **deepseek-ai/DeepSeek-V4-Flash-0731** | 304B | 4.58M | → | 高效版本 |

### 新上线重点模型 (本月)

#### nvidia/Qwen3.6-35B-A3B-NVFP4 (NVIDIA)
- **参数量**: 19B (激活 3B)
- **下载量**: 11.2M
- **特点**: NVIDIA 原生优化, NVFP4 量化格式
- **更新时间**: 1 天前

#### trl-internal-testing/tiny-Qwen2ForCausalLM-2.5
- **参数量**: 2.43M
- **下载量**: 16.6M
- **特点**: Qwen2 微小测试模型

#### farbodtavakkoli/OTel-2.0-LLM-31B-IT
- **参数量**: 32B
- **下载量**: 6.79M
- **特点**: OTel 专业模型, 6天前更新

### 模型趋势分析 (2026-08-31)

1. **Qwen3 系列持续霸榜**: 前 20 名中 Qwen 家族占 9 席, 从 0.6B 到 32B 全覆盖

2. **NVIDIA 深度优化**: Qwen3.6-35B-A3B-NVFP4 挤入前 10, 1天前更新

3. **量化模型持续热门**: unsloth 的 GGUF 量化版本保持高下载量

4. **DeepSeek 稳定输出**: DeepSeek-V4-Flash-0731 保持 4.58M 下载

5. **OpenAI 开源系列**: gpt-oss-20b (6.52M) 和 gpt-oss-120b (5.31M) 保持稳定

### 小模型专精榜 (2026-08-31 更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Qwen3-0.6B | 0.8B | 边缘设备 | ⭐⭐⭐⭐⭐ | 22.5M 下载, 最小最强 |
| Qwen3-Coder-30B-A3B | 31B | 代码生成 | ⭐⭐⭐⭐⭐ | GGUF 12.8M 下载 |
| Qwen3.6-35B-A3B-NVFP4 | 19B | 高效推理 | ⭐⭐⭐⭐⭐ | NVIDIA 原生优化 |
| DeepSeek-V4-Flash | 304B | 高效推理 | ⭐⭐⭐⭐ | 4.58M 下载 |
| Llama-3.2-1B | 1B | 轻量 | ⭐⭐⭐⭐ | 6.66M 下载 |

---

---

## 2026 年 09 月主流模型动态 - 2026-09-11 更新

### Hugging Face Trending 文本生成模型 (Top 20)

| 排名 | 模型 | 参数量 | 下载量 | 趋势 | 备注 |
|------|------|--------|--------|------|------|
| 1 | **openbmb/MiniCPM5-2B** | 3B | 42.3k | 🆕 | 8小时前更新，面壁小钢炮新版 |
| 2 | **XHToken/Spark-X2.5-4B** | 4B | 15.9k | 🆕 | 新兴模型，7天前 |
| 3 | **nex-agi/Nex-N2.5-mini** | 35B | 2.44k | 🆕 | 2天前更新，Agent 专用 |
| 4 | **dealignai/GLM-5.3-CYBERSECURITY-FP8** | 753B | 24.3k | 🆕 | 2天前，网络安全专用 GLM |
| 5 | **IFM/K2-Horizon-MoVA-36B-A4B** | 37B | 4.49k | 🆕 | 3天前，MoVA 架构 |
| 6 | **zai-org/GLM-5.3** | 753B | 552k | → | 智谱最新，6天前更新 |
| 7 | **JonathanColetti/Qwen3.8-27B-Uncensored-GGUF** | 27B | 2.81M | → | 未经审查 GGUF 版 |
| 8 | **OBLITERATUS/Qwen3.8-27B-OBLITERATED** | 28B | 1.13M | → | 未审查版 |
| 9 | **TokenRhythm/NeoHorse-1-4B** | 4B | 5.33k | 🆕 | 10小时前更新 |
| 10 | **nvidia/Qwen3.8-27B-NVFP4** | 18B | 10.5k | 🆕 | NVIDIA 优化版，1天前更新 |
| 11 | **openai/gpt-oss-20b** | 21B | 6.59M | → | OpenAI 开源 |
| 12 | **nvidia/NVIDIA-Nemotron-3.5-Lightning-30B-A3B-NVFP4** | 18B | 1.32M | → | NVIDIA 高效优化 |
| 13 | **superwhisper/s1-mini** | 0.8B | 8.53k | → | 语音转文本 |
| 14 | **unsloth/GLM-5.3-Flash-GGUF** | 321B | 285k | → | 量化版 |
| 15 | **ornith-ai/Ornith-1.5-9B-GGUF** | 9B | 4.01M | → | 高效量化版 |
| 16 | **prism-ml/Ternary-Bonsai-27B-gguf** | 27B | 646k | → | 高效量化 |
| 17 | **inclusionAI/Ling-3.0-tiny** | 8B | 28.8k | → | 轻量版 |
| 18 | **Nanbeige/Nanbeige4.2-3B** | 4B | 33.9k | → | 中文词词模型 |
| 19 | **openbmb/MiniCPM5-2B-GGUF** | 3B | 51.2k | 🆕 | GGUF 量化版 |
| 20 | **deepseek-ai/DeepSeek-V4-Flash-0731** | 304B | 4.39M | → | 高效版持续热门 |

### 新上线重点模型

#### Nex-N2.5 系列 (Nex-AGI)

**Nex-N2.5** 是本周最重要的 Agent 模型发布，分为 mini/Pro/Max 三档：

| 模型 | 参数量 | 架构 | 定位 |
|------|--------|------|------|
| **Nex-N2.5-mini** | 35B | MoE | 轻量 Agent |
| **Nex-N2.5-Pro** | - | MoE | 中端 Agent |
| **Nex-N2.5-Max** | **1.6T** | MoE | 万亿参数旗舰 |

**关键亮点**：
- Nex-N2.5-Max 是 Nex-AGI **首个万亿参数规模的完整后训练**成果
- 支持持续行动和视觉反馈自我修正
- 可操作电脑和浏览器，自主执行和测试程序
- 视觉不再只是输入模态，而是 Agent 感知环境、验证结果的关键接口

**基准测试对比**：

| Benchmark | Nex-N2.5-Max | Claude Opus 5 | GPT-5.6 Sol | Kimi-K3 |
|-----------|-------------|---------------|-------------|---------|
| SWE-Bench Pro | 65.7 | 79.2 | 64.6 | 63.3 |
| Terminal-Bench 2.1 | 78.6 | 86.1 | 89.1 | 88.8 |
| BrowseComp | 92.6 | 90.8 | 90.4 | 91.2 |
| OSWorld-Verified | 82.2 | 83.4 | 83.2 | 84.8 |
| AutomationBench | 50.2 | 45.8 | 46.7 | 48.2 |

#### K2-Horizon-MoVA-36B-A4B (IFM)

- **参数量**: 36B (激活 4B)
- **特点**: MoVA (Mixture-of-Values Attention) 架构，512K 原生上下文
- **基准表现**: 4B 激活参数在 Agent 和推理任务上超越 15 倍规模的模型

| Benchmark | K2-Horizon 36B | Qwen3.6-35B | Nemotron 3 Ultra |
|-----------|----------------|-------------|------------------|
| tau3-Banking | 26.8 | 9.3 | 14.2 |
| Terminal-Bench 2.1 | 58.6 | 44.9 | 53.9 |
| GPQA Diamond | 80.8 | 84.1 | 86.7 |

#### MiniCPM5-2B (面壁)

- **参数量**: 3B
- **下载量**: 42.3k (8小时前更新)
- **特点**: 面壁小钢炮最新版本，GGUF 量化版 51.2k 下载

#### GLM-5.3-CYBERSECURITY (智谱)

- **参数量**: 753B
- **特点**: 网络安全领域专项微调，降低对渗透测试/逆向/恶意软件分析的拒绝率
- **使用注意**: reasoning_effort 只支持 low/high，FP8 推荐 low 用于 Agent 场景

#### Qwen3.8-Flash-Next (阿里)

- **AtomicChat/Qwen3.8-Flash-Next-GGUF**: 177B，48.5k 下载
- **agentionai/Qwen3.8-Flash-Next-ROCmFP4-FAST**: ROCm FP4 优化版，27.8k 下载，18小时前更新

### 模型趋势分析 (2026-09)

1. **Agent 模型军备竞赛**: Nex-N2.5-Max (1.6T) 和 Nex-N2.5-Pro 的出现标志着万亿参数 Agent 模型走向实用化，视觉反馈自我修正成为标配

2. **NVIDIA 持续深耕**: Qwen3.8-27B-NVFP4 (1天前更新) 和 Nemotron-3.5-Lightning-30B-A3B-NVFP4 (3小时前更新) 显示 NVIDIA 在高效推理格式上持续发力

3. **GLM-5.3 生态扩张**: 从通用版到 CYBERSECURITY 专项版，智谱正在细分领域做专业化微调

4. **面壁小钢炮回归**: MiniCPM5-2B 新版本保持小参数高性能路线，8小时前更新显示活跃维护

5. **GGUF 量化持续统治**: 几乎所有热门模型都有 GGUF 量化版，社区对本地部署需求旺盛

### 小模型专精榜 (2026-09-11 更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Nex-N2.5-mini | 35B | Agent | ⭐⭐⭐⭐⭐ | Agent 专用家族 |
| K2-Horizon-MoVA-36B | 4B 激活 | 高效 Agent | ⭐⭐⭐⭐⭐ | 4B 参数超越 15x 规模 |
| MiniCPM5-2B | 3B | 轻量高效 | ⭐⭐⭐⭐ | 面壁小钢炮最新版 |
| NVIDIA-Nemotron-3.5-Lightning | 30B | 高效推理 | ⭐⭐⭐⭐⭐ | NVIDIA 原生优化 |
| DeepSeek-V4-Flash | 304B | 高效推理 | ⭐⭐⭐⭐ | 4.39M 下载 |

---

*最后更新: 2026-09-11*

---

## 2026 年 08 月主流模型动态 - 2026-08-17 更新

### OpenAI GPT-5.6 发布：价格性能比革命性突破

**GPT-5.6** 是本周最重要的模型发布，代表了价格-性能曲线的大幅左移：

#### 核心更新

| 模型 | 降价幅度 | 性能定位 |
|------|----------|----------|
| **GPT-5.6 Luna** | **-80%** | 最快最便宜，高吞吐量场景 |
| **GPT-5.6 Terra** | **-20%** | 均衡模型，日常任务 |
| **GPT-5.6 Sol** | 新增 Fast 模式 | 最高智能，推理速度提升 2.5x |

#### 关键数据

- **BrowseComp 基准**: GPT-5.6 Luna (Extra High) 得分 84.04%，成本从 GPT-5.5 的 $33.27 降至 **$1.33**（降幅 96%）
- **Agents' Last Exam**: GPT-5.6 Sol (低推理强度) 性能超越 GPT-5.5 (高推理强度)
- **Fast 模式**: 比标准处理快 2.5x，仅需 2x 价格

#### Responses API 新增特性

- **推理持久化**: 跨调用保持推理连贯性
- **原生压缩**: 长对话自动压缩，减少 token 消耗
- **多 Agent 编排**: 更好的多 Agent 协作支持

#### 分析

GPT-5.6 的推出标志着 **Agent 经济性** 进入新阶段：过去需要旗舰模型 + 高推理成本才能完成的长周期任务，现在 Luna/Terra 就能以 1/25 的成本完成。这意味着 AI Agent 的商业化门槛大幅降低。

---

### Hugging Face Trending 模型 (2026-08-17)

| 排名 | 模型 | 参数量 | 下载量 | 趋势 | 备注 |
|------|------|--------|--------|------|------|
| 1 | **Qwen3.8-27B** | 28B | 268k | 🆕 | 阿里最新主力，2天前更新 |
| 2 | **Muse-Glimmer-30B** | 30B | 293k | 🆕 | Meta 新模型，5天前 |
| 3 | **unsloth/Qwen3.8-27B-GGUF** | 27B | 1.95M | ⬆️ | GGUF 量化版最热 |
| 4 | **Qwen3.8-2.4T-A95B** | 2.4T | 7.93k | → | 旗舰模型，多格式 |
| 5 | **LTX-2.5** | - | 424k | 🆕 | Lightricks 视频生成，4小时前 |
| 6 | **MiniMax-Music3** | 2B | 8.64k | 🆕 | MiniMax 音乐生成 |
| 7 | **MiniMax-H3** | 33B | 2.31M | → | 视频生成旗舰 |
| 8 | **DeepSeek-V4-Pro-0813** | 1.7T | 21.9k | 🆕 | 每日更新版 |
| 9 | **DeepSeek-V4-Flash-0731** | 304B | 1.87M | → | 高效版本 |
| 10 | **Kimi-K3** | 2.8T | 2.14M | → | 月之暗面多模态 |
| 11 | **NVIDIA-Nemotron-3.5-Lightning-30B** | 18B | 196k | 🆕 | NVIDIA 高效优化 |
| 12 | **LiquidAI/LFM2.5-2.6B** | 3B | 141k | → | 轻量高效 |
| 13 | **Kimi-K3-GGUF** | 2.8T | 需确认 | 🆕 | 高效量化版 |
| 14 | **dots3-note-prev** | 288B | 393 | 🆕 | 新兴模型 |

### 模型趋势分析 (2026-08-17)

#### 1. Qwen3.8 系列全面崛起

Qwen3.8-27B 成为 Hugging Face trending 第一名（268k 下载），取代了此前的 Qwen3.6 系列：

| 模型 | 参数量 | 格式 | 下载量 |
|------|--------|------|--------|
| Qwen3.8-27B | 28B | 原生 | 268k |
| unsloth/Qwen3.8-27B-GGUF | 27B | GGUF | 1.95M |
| Qwen3.8-27B-FP8 | 28B | FP8 | 353k |
| Qwen3.8-2.4T-A95B | 2.4T | 原生/FP8 | 7.93k / 11.3k |

#### 2. 视频/音频生成持续火热

- **MiniMax-H3**: 2.31M 下载，视频生成旗舰地位稳固
- **LTX-2.5**: 4 小时前更新，视频生成新版本
- **MiniMax-Music3**: 2B 音乐生成模型

#### 3. GGUF 量化版统治下载量

unsloth 的 GGUF 量化版本下载量远超原生模型：
- Qwen3.8-27B-GGUF: 1.95M (vs 原生 268k)
- MiniMax-H3-GGUF: 204k
- Qwen3.6-27B-Fable-Fusion-Uncensored-GGUF: 3.02M

#### 4. NVIDIA 深度优化

**NVIDIA-Nemotron-3.5-Lightning-30B** (18B 激活参数) 提供多种量化格式：NVFP4 (196k), BF16 (34.1k), GGUF (56.5k)，专为本地推理优化。

### 小模型专精榜 (2026-08-17 更新)

| 模型 | 参数 | 专精领域 | 评分 | 备注 |
|------|------|----------|------|------|
| Qwen3.8-27B | 28B | 通用旗舰 | ⭐⭐⭐⭐⭐ | Hugging Face trending #1 |
| NVIDIA-Nemotron-3.5-Lightning | 30B | 高效推理 | ⭐⭐⭐⭐⭐ | NVIDIA 原生优化 |
| Kimi-K3 | 2.8T | 多模态 | ⭐⭐⭐⭐ | 2.14M 下载 |
| DeepSeek-V4-Flash | 304B | 高效推理 | ⭐⭐⭐⭐ | 1.87M 下载 |
| LiquidAI/LFM2.5-2.6B | 3B | 轻量高效 | ⭐⭐⭐⭐ | GGUF 246k |
| MiniMax-H3 | 33B | 视频生成 | ⭐⭐⭐⭐⭐ | 2.31M 下载 |