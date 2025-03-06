# Awesome Direct Preference Optimization

A list of selected paper and possible corresponding codes in our review paper [A Survey of Direct Preference Optimization]().

*If you find there is a missed paper or a possible mistake in our survey, please feel free to email me ([shunyu.liu@ntu.edu.sg](mailto:shunyu.liu@ntu.edu.sg)) or pull a request here. I am more than glad to receive your advice. Thanks!*

## Table of Contents

## Overview

## A Taxonomy of Direct Preference Optimization

### Data Strategy

#### Data Quality - Heterogeneity

- Direct Preference Optimization With Unobserved Preference Heterogeneity [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.15065)
- MallowsPO: Fine-Tune Your LLM with Preference Dispersions [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.14953)
- Group Robust Preference Optimization in Reward-free RLHF [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.20304)

- No Preference Left Behind: Group Distributional Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.12-b31b1b.svg)](https://arxiv.org/abs/2412.20299)

#### Data Quality - Distinguishability

- Gap-Aware Preference Optimization: Enhancing Model Alignment with Perception Margin [[OpenReview]](https://openreview.net/forum?id=N2sN3LESoW)
- Direct Preference Optimization with an Offset [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.10571)
- Adaptive Preference Scaling for Reinforcement Learning with Human Feedback [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.02764)
- Reward Difference Optimization For Sample Reweighting In Offline RLHF [![arXiv](https://img.shields.io/badge/arXiv-2024.08-b31b1b.svg)](https://arxiv.org/abs/2408.09385)
- Geometric-Averaged Preference Optimization for Soft Preference Labels [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.06691)
- Plug-and-Play Training Framework for Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.12-b31b1b.svg)](https://arxiv.org/abs/2412.20996)
- Filtered Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.13846)
- β-dpo: Direct preference optimization with dynamic β [![arXiv](https://img.shields.io/badge/arXiv-2024.07-b31b1b.svg)](https://arxiv.org/abs/2407.08639)
- Direct Alignment of Language Models via Quality-Aware Self-Refinement [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.21040)
- α -DPO: Adaptive Reward Margin is What Direct Preference Optimization Needs [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.10148)
- sDPO: Don't Use Your Data All at Once [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.192)
- Enhancing Alignment using Curriculum Learning & Ranked Preferences [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.07230)
- Mixed Preference Optimization: Reinforcement Learning with Data Selection and Better Reference Model [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.19443)

#### Data Quality - Noise

- Understanding Generalization of Preference Optimization Under Noisy Feedback [[OpenReview]](https://openreview.net/forum?id=H8gLQwg1eC)
- Provably Robust DPO: Aligning Language Models with Noisy Feedback [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.00409)
- Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.07-b31b1b.svg)](https://arxiv.org/abs/2407.07880)

- Combating inherent noise for direct preference optimization [[OpenReview]](https://openreview.net/forum?id=MlxeUVCQgD)
- Perplexity-aware Correction for Robust Alignment with Noisy Preferences [[OpenReview]](https://openreview.net/pdf?id=OUXnnPJzXJ)
- Impact of Preference Noise on the Alignment Performance of Generative Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.09824)
- Spread Preference Annotation: Direct Preference Judgment for Efficient LLM Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.04412)
- ROPO: Robust Preference Optimization for Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.04102)

#### Preference Feedback - Point-Wise

- General Preference Modeling with Preference Representations for Aligning Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.02197)
- KTO: Model Alignment as Prospect Theoretic Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.01306)
- Binary Classifier Optimization for Large Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.04656)
- Offline Regularised Reinforcement Learning for Large Language Models Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.19107)
- Distributional Preference Alignment of LLMs via Optimal Transport [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.05882)
- Cal-DPO: Calibrated Direct Preference Optimization for Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.12-b31b1b.svg)](https://arxiv.org/abs/2412.14516)
- Noise Contrastive Alignment of Language Models with Explicit Rewards [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.05369)
- ULMA: Unified Language Model Alignment with Human Demonstration and Point-wise Preference [![arXiv](https://img.shields.io/badge/arXiv-2023.12-b31b1b.svg)](https://arxiv.org/abs/2312.02554)

#### Preference Feedback - Pair-Wise

- IOPO: Empowering LLMs with Complex Instruction Following via Input-Output Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.11-b31b1b.svg)](https://arxiv.org/abs/2411.06208)
- Negating negatives: Alignment without human positive samples via distributional dispreference optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.03419)
- Negative preference optimization: From catastrophic collapse to effective unlearning [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.05868)
- Self-Augmented Preference Optimization: Off-Policy Paradigms for Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.20830)
- Simplicity Prevails: Rethinking Negative Preference Optimization for LLM Unlearning [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.07163)
- Preference Optimization as Probabilistic Inference [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.04166)
- Bridging and Modeling Correlations in Pairwise Data for Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.08-b31b1b.svg)](https://arxiv.org/abs/2408.07471)
- On Extending Direct Preference Optimization to Accommodate Ties [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.17431)
- Direct Preference Optimization: Your Language Model is Secretly a Reward Model [![arXiv](https://img.shields.io/badge/arXiv-2023.05-b31b1b.svg)](https://arxiv.org/abs/2305.18290)

#### Preference Feedback - List-Wise

- LiPO: Listwise Preference Optimization through Learning-to-Rank [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.01878)
- Panacea: Pareto Alignment via Preference Adaptation for LLMs [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.02030)
- LIRE: listwise reward enhancement for preference alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.13516)

- Ordinal Preference Optimization: Aligning Human Preferences via NDCG [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.04346)
- Preference Optimization with Multi-Sample Comparisons [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.12138)
- Optimizing Preference Alignment with Differentiable NDCG Ranking [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.18127)

- TODO: Enhancing LLM Alignment with Ternary Preferences [![arXiv](https://img.shields.io/badge/arXiv-2024.11-b31b1b.svg)](https://arxiv.org/abs/2411.02442)
- Relative Preference Optimization: Enhancing LLM Alignment through Contrasting Responses across Identical and Diverse Prompts [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.10958)

#### Preference Granularity - Token-Level

- DPO Meets PPO: Reinforced Token Optimization for RLHF [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.18922)
- Selective Preference Optimization via Token-Level Reward Function Estimation [![arXiv](https://img.shields.io/badge/arXiv-2024.08-b31b1b.svg)](https://arxiv.org/abs/2408.13518)
- EPO: Hierarchical LLM Agents with Environment Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.08-b31b1b.svg)](https://arxiv.org/abs/2408.16090)
- TIS-DPO: Token-level Importance Sampling for Direct Preference Optimization With Estimated Weights [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.04350)
- SparsePO: Controlling Preference Alignment of LLMs via Sparse Token Masks [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.05102)
- Token-level Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.11999)
- Earlier Tokens Contribute More: Learning Direct Preference Optimization From Temporal Decay Perspective [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.1234)
- From r to Q∗: Your Language Model is Secretly a Q-Function [![arXiv](https://img.shields.io/badge/arXiv-2404.12358-b31b1b.svg)](https://arxiv.org/abs/2404.12358)

#### Preference Granularity - Step-Level

- Step-DPO: Step-wise Preference Optimization for Long-chain Reasoning of LLMs [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.18629)
- Data-Centric Human Preference Optimization with Rationales [![arXiv](https://img.shields.io/badge/arXiv-2024.07-b31b1b.svg)](https://arxiv.org/abs/2407.14477)
- TPO: Aligning Large Language Models with Multi-branch & Multi-step Preference Trees [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.12854)
- Step-controlled dpo: Leveraging stepwise error for enhanced mathematical reasoning [![arXiv](https://img.shields.io/badge/arXiv-2024.07-b31b1b.svg)](https://arxiv.org/abs/2407.00782)
- Improving Multi-Step Reasoning Abilities of Large Language Models with Direct Advantage Policy Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.12-b31b1b.svg)](https://arxiv.org/abs/2412.18279)
- Chain of Preference Optimization: Improving Chain-of-Thought Reasoning in LLMs [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.09136)
- Monte Carlo Tree Search Boosts Reasoning via Iterative Preference Learning [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.00451)

#### Preference Granularity - Sentence-Level

- Direct Preference Optimization: Your Language Model is Secretly a Reward Model [![arXiv](https://img.shields.io/badge/arXiv-2023.05-b31b1b.svg)](https://arxiv.org/abs/2305.18290)

- Advancing LLM Reasoning Generalists with Preference Trees [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.02078)
- MAPO: Advancing Multilingual Reasoning through Multilingual-Alignment-as-Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.01-b31b1b.svg)](https://arxiv.org/abs/2401.06838)
- Iterative Reasoning Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.19733)
- FactAlign: Long-form factuality alignment of large language models [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.01691)

#### Preference Granularity - Turn-Level

- SDPO: Segment-Level Direct Preference Optimization for Social Agents [![arXiv](https://img.shields.io/badge/arXiv-2025.01-b31b1b.svg)](https://arxiv.org/abs/2501.01821)
- Agent Q: Advanced Reasoning and Learning for Autonomous AI Agents [![arXiv](https://img.shields.io/badge/arXiv-2024.08-b31b1b.svg)](https://arxiv.org/abs/2408.07199)
- Direct Multi-Turn Preference Optimization for Language Agents [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.14868)
- Trial and Error: Exploration-Based Trajectory Optimization for LLM Agents [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.02502)
- Building Math Agents with Multi-Turn Iterative Preference Learning [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.02392)

### Learning Framework

#### Paradigm - Offline

- sDPO: Don't Use Your Data All at Once [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.192)
- Enhancing Alignment using Curriculum Learning & Ranked Preferences [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.07230)

- Paft: A parallel training paradigm for effective LLM fine-tuning [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.17923)
- Contrastive preference optimization: Pushing the boundaries of LLM performance in machine translation [![arXiv](https://img.shields.io/badge/arXiv-2024.01.08417-b31b1b.svg)](https://arxiv.org/abs/2401.08417)
- ORPO: Monolithic Preference Optimization without Reference Model [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.07691)
- Direct Preference Optimization: Your Language Model is Secretly a Reward Model[![arXiv](https://img.shields.io/badge/arXiv-2023.05-b31b1b.svg)](https://arxiv.org/abs/2305.18290)
- ULMA: Unified Language Model Alignment with Human Demonstration and Point-wise Preference[![arXiv](https://img.shields.io/badge/arXiv-2023.12-b31b1b.svg)](https://arxiv.org/abs/2312.02554)

#### Paradigm - Online

- Mixed Preference Optimization: Reinforcement Learning with Data Selection and Better Reference Model [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.19443)
- ROPO: Robust Preference Optimization for Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.04102)

- Exploratory Preference Optimization: Provably Sample-Efficient Exploration in RLHF with General Function Approximation [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.21046)
- Statistical rejection sampling improves preference optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2309.06657)
- Direct Language Model Alignment from Online AI Feedback [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402...)

- RS-DPO: A Hybrid Rejection Sampling and Direct Preference Optimization Method for Alignment of Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.10038)
- D2PO: Discriminator-Guided DPO with Response Evaluation Models [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.01511)

- Value-Incentivized Preference Optimization: A Unified Approach to Online and Offline RLHF [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.19320)
- The Importance of Online Data: Understanding Preference Fine-tuning via Coverage [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.01462)

- Online DPO: Online Direct Preference Optimization with Fast-Slow Chasing [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.05534)
- BPO: Supercharging Online Preference Learning by Adhering to the Proximity of Behavior LLM [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.12168)

- The Crucial Role of Samplers in Online Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.19605)
- Accelerated Preference Optimization for Large Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.06293)
- SeRA: Self-Review & Alignment with Implicit Reward Margins [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.06293)

- CREAM: Consistency Regularized Self-Rewarding Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.12735)
- Self-training with direct preference optimization improves chain-of-thought reasoning [![arXiv](https://img.shields.io/badge/arXiv-2024.07-b31b1b.svg)](https://arxiv.org/abs/2407.18248)
- Self-Rewarding Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.01-b31b1b.svg)](https://arxiv.org/abs/2401.10020)

- Direct large language model alignment through self-rewarding contrastive prompt distillation [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.11907)
- COMAL: A Convergent Meta-Algorithm for Aligning LLMs with General Preferences [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/pdf/2410.23223)
- OPTune: Efficient Online Preference Tuning [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2406.07657)

- Iterative Preference Learning from Human Feedback: Bridging Theory and Practice for RLHF under KL-constraint [![arXiv](https://img.shields.io/badge/arXiv-2024.12-b31b1b.svg)](https://arxiv.org/abs/2312.11456)
- Some things are more cringe than others: Iterative preference optimization with the pairwise cringe loss [![arXiv](https://img.shields.io/badge/arXiv-2024.12-b31b1b.svg)](https://arxiv.org/abs/2312.16682)

- Self-Exploring Language Models: Active Preference Elicitation for Online Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.19332)

- Iterative Reasoning Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.19733)

- Monte Carlo Tree Search Boosts Reasoning via Iterative Preference Learning [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.00451)

- Trial and Error: Exploration-Based Trajectory Optimization for LLM Agents [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.02502)

- Building Math Agents with Multi-Turn Iterative Preference Learning [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.02392)

#### Paradigm - Active

- Active Preference Learning for Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg  )](https://arxiv.org/abs/2402.08114)
- Reinforcement Learning from Human Feedback with Active Queries [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg  )](https://arxiv.org/abs/2402.09401)
- Active Preference Optimization for Sample Efficient RLHF [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg  )](https://arxiv.org/abs/2402.10500)
- Active Preference Optimization via Maximizing Learning Capacity [[OpenReview]](https://openreview.net/forum?id=bRfVj0Sh88)

#### Objective - Multi-Objective

- Beyond one-preference-fits-all alignment: Multi-objective direct preference optimization [![arXiv](https://img.shields.io/badge/arXiv-2023.10-b31b1b.svg)](https://arxiv.org/abs/2310.03708)
- Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.02-b31b1b.svg)](https://arxiv.org/abs/2402.19085)
- SPO: Multi-Dimensional Preference Sequential Alignment With Implicit Reward Modeling [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.12739)

- Hybrid Preference Optimization: Augmenting Direct Preference Optimization with Auxiliary Objectives [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.17956)
- Simultaneous Reward Distillation and Preference Learning: Get You a Language Model Who Can Do Both [![arXiv](https://img.shields.io/badge/arXiv-2024.10-b31b1b.svg)](https://arxiv.org/abs/2410.08458)

- MOSLIM: Align with diverse preferences in prompts through reward classification [[OpenReview]](https://openreview.net/forum?id=w0MAu8vjwj)

#### Objective - Self-Play

- A minimaximalist approach to reinforcement learning from human feedback [![arXiv](https://img.shields.io/badge/arXiv-2024.01-b31b1b.svg)](https://arxiv.org/abs/2401.04056)
- Nash learning from human feedback [![arXiv](https://img.shields.io/badge/arXiv-2023.12-b31b1b.svg)](https://arxiv.org/abs/2312.00886)
- Self-play fine-tuning converts weak language models to strong language models [![arXiv](https://img.shields.io/badge/arXiv-2024.01-b31b1b.svg)](https://arxiv.org/abs/2401.01335)
- Human Alignment of Large Language Models through Online Preference Optimisation [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.08635)
- BoNBoN Alignment for Large Language Models and the Sweetness of Best-of-n Sampling [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.00832)
- Direct nash optimization: Teaching language models to self-improve with general preferences [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.03715)
- Self-Play Preference Optimization for Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.00675)
- Self-Improving Robust Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.01660)

### Constraint Mechanism

#### Reference - Dynamic

- Enhancing Alignment using Curriculum Learning & Ranked Preferences [![arXiv](https://img.shields.io/badge/arXiv-2403.07230-b31b1b.svg)](https://arxiv.org/abs/2403.07230)
- Mixed Preference Optimization: Reinforcement Learning with Data Selection and Better Reference Model [![arXiv](https://img.shields.io/badge/arXiv-2403.19443-b31b1b.svg)](https://arxiv.org/abs/2403.19443)

- Learn Your Reference Model for Real Good Alignment [![arXiv](https://img.shields.io/badge/arXiv-2404.09656-b31b1b.svg)](https://arxiv.org/abs/2404.09656)

- Building Math Agents with Multi-Turn Iterative Preference Learning [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.02392)

#### Reference - Free

- Understanding reference policies in direct preference optimization [![arXiv](https://img.shields.io/badge/arXiv-2407.13709-b31b1b.svg)](https://arxiv.org/abs/2407.13709)
- SimPER: Simple Preference Fine-Tuning without Hyperparameters by Perplexity Optimization [![arXiv](https://img.shields.io/badge/arXiv-2502.00883-b31b1b.svg)](https://arxiv.org/abs/2502.00883)
- SimPO: Simple Preference Optimization with a Reference-Free Reward [![arXiv](https://img.shields.io/badge/arXiv-2405.14734-b31b1b.svg)](https://arxiv.org/abs/2405.14734)
- Contrastive preference optimization: Pushing the boundaries of LLM performance in machine translation [![arXiv](https://img.shields.io/badge/arXiv-2024.01.08417-b31b1b.svg)](https://arxiv.org/abs/2401.08417)
- ORPO: Monolithic Preference Optimization without Reference Model [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.07691)

#### Divergence - Diversity

- Beyond Reverse KL- Generalizing Direct Preference Optimization with Diverse Divergence Constraints [![arXiv](https://img.shields.io/badge/arXiv-2309.16240-b31b1b.svg)](https://arxiv.org/abs/2309.16240)
- Diverse Preference Learning for Capabilities and Alignment [[OpenReview]](https://openreview.net/forum?id=pOq9vDIYev)

#### Divergence - Generalization

- Diverse Preference Learning for Capabilities and Alignment [[OpenReview]](https://openreview.net/forum?id=pOq9vDIYev)
- SimPO: Simple Preference Optimization with a Reference-Free Reward [![arXiv](https://img.shields.io/badge/arXiv-2405.14734-b31b1b.svg)](https://arxiv.org/abs/2405.14734)

- Soft Preference Optimization: Aligning Language Models to Expert Distributions [![arXiv](https://img.shields.io/badge/arXiv-2405.00747-b31b1b.svg)](https://arxiv.org/abs/2405.00747)
- DPO Kernels: A Semantically-Aware, Kernel-Enhanced, and Divergence-Rich Paradigm for Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2501.03271-b31b1b.svg)](https://arxiv.org/abs/2501.03271)
- Generalized Preference Optimization: A Unified Approach to Offline Alignment [![arXiv](https://img.shields.io/badge/arXiv-2402.05749-b31b1b.svg)](https://arxiv.org/abs/2402.05749)

- FlipGuard: Defending Preference Alignment against Update Regression with Constrained Optimization [![arXiv](https://img.shields.io/badge/arXiv-2410.00508-b31b1b.svg)](https://arxiv.org/abs/2410.00508)
- Correcting the Mythos of KL-Regularization: Direct Alignment without Overoptimization via Chi-Squared Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2407.13399-b31b1b.svg)](https://arxiv.org/abs/2407.13399)

- Improving Conversational Abilities of Quantized Large Language Models via Direct Preference Alignment [![arXiv](https://img.shields.io/badge/arXiv-2407.03051-b31b1b.svg)](https://arxiv.org/abs/2407.03051)

- Direct Preference Optimization Using Sparse Feature-level Constraints [![arXiv](https://img.shields.io/badge/arXiv-2411.07618-b31b1b.svg)](https://arxiv.org/abs/2411.07618)
- Towards Efficient Exact Optimization of Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2402.00856-b31b1b.svg)](https://arxiv.org/abs/2402.00856)

#### Safety

- Backtracking Improves Generation Safety [![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.14586)
- SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety [[OpenReview]](https://openreview.net/forum?id=MoJSnVZ59d)
- Stepwise Alignment for Constrained Language Model Policy Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.04-b31b1b.svg)](https://arxiv.org/abs/2404.11049)

### Model Property

#### Generation - Distribution

- Right Now, Wrong Then: Non-Stationary Direct Preference Optimization under Preference Drift [![arXiv](https://img.shields.io/badge/arXiv-2407.18676-b31b1b.svg)](https://arxiv.org/abs/2407.18676)
- Preference Fine-Tuning of LLMs Should Leverage Suboptimal, On-Policy Data [![arXiv](https://img.shields.io/badge/arXiv-2404.14367-b31b1b.svg)](https://arxiv.org/abs/2404.14367)
- On the limited generalization capability of the implicit reward model induced by direct preference optimization [![arXiv](https://img.shields.io/badge/arXiv-2409.03650-b31b1b.svg)](https://arxiv.org/abs/2409.03650)
- Robust Preference Optimization through Reward Model Distillation [![arXiv](https://img.shields.io/badge/arXiv-2405.19316-b31b1b.svg)](https://arxiv.org/abs/2405.19316)
- Self-Exploring Language Models: Active Preference Elicitation for Online Alignment [![arXiv](https://img.shields.io/badge/arXiv-2024.05-b31b1b.svg)](https://arxiv.org/abs/2405.19332)
- On Extending Direct Preference Optimization to Accommodate Ties[![arXiv](https://img.shields.io/badge/arXiv-2024.09-b31b1b.svg)](https://arxiv.org/abs/2409.17431)
- Self-Improving Robust Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.01660)

#### Generation - Length

- SimPO: Simple Preference Optimization with a Reference-Free Reward [![arXiv](https://img.shields.io/badge/arXiv-2405.14734-b31b1b.svg)](https://arxiv.org/abs/2405.14734)

- Declarative characterizations of direct preference alignment algorithms [![arXiv](https://img.shields.io/badge/arXiv-2412.17696v1-b31b1b.svg)](https://arxiv.org/abs/2412.17696v1)
- A Long Way to Go: Investigating Length Correlations in RLHF [![arXiv](https://img.shields.io/badge/arXiv-2310.03716-b31b1b.svg)](https://arxiv.org/abs/2310.03716)
- Insights into Alignment: Evaluating DPO and its Variants Across Multiple Tasks [![arXiv](https://img.shields.io/badge/arXiv-2404.14723-b31b1b.svg)](https://arxiv.org/abs/2404.14723)

- Disentangling Length from Quality in Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2403.19159-b31b1b.svg)](https://arxiv.org/abs/2403.19159)
- Eliminating Biased Length Reliance of Direct Preference Optimization via Down-Sampled KL Divergence [![arXiv](https://img.shields.io/badge/arXiv-2406.10957-b31b1b.svg)](https://arxiv.org/abs/2406.10957)
- Following length constraints in instructions [![arXiv](https://img.shields.io/badge/arXiv-2406.17744-b31b1b.svg)](https://arxiv.org/abs/2406.17744)

- The Hitchhiker’s Guide to Human Alignment with *PO [![arXiv](https://img.shields.io/badge/arXiv-2407.15229-b31b1b.svg)](https://arxiv.org/abs/2407.15229)
- Length Desensitization in Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2409.06411-b31b1b.svg)](https://arxiv.org/abs/2409.06411)
- LongPO: Long Context Self-Evolution of Large Language Models through Short-to-Long Preference Optimization [[OpenReview]](https://openreview.net/forum?id=qTrEq31Shm)
- Rrhf: Rank responses to align language models with human feedback without tears [![arXiv](https://img.shields.io/badge/arXiv-2304.05302-b31b1b.svg)](https://arxiv.org/abs/2304.05302)
- Earlier Tokens Contribute More: Learning Direct Preference Optimization From Temporal Decay Perspective [![arXiv](https://img.shields.io/badge/arXiv-2024.03-b31b1b.svg)](https://arxiv.org/abs/2403.1234)
- Direct Multi-Turn Preference Optimization for Language Agents [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.14868)

#### Optimization - Likelihood

- Robust Preference Optimization through Reward Model Distillation [![arXiv](https://img.shields.io/badge/arXiv-2405.19316-b31b1b.svg)](https://arxiv.org/abs/2405.19316)

- Anchored Preference Optimization and Contrastive Revisions: Addressing Underspecification in Alignment [![arXiv](https://img.shields.io/badge/arXiv-2408.06266-b31b1b.svg)](https://arxiv.org/abs/2408.06266)
- From r to Q∗: Your Language Model is Secretly a Q-Function [![arXiv](https://img.shields.io/badge/arXiv-2404.12358-b31b1b.svg)](https://arxiv.org/abs/2404.12358)

- Reward Model Learning vs. Direct Policy Optimization: A Comparative Analysis of Learning from Human Preferences [![arXiv](https://img.shields.io/badge/arXiv-2403.01857-b31b1b.svg)](https://arxiv.org/abs/2403.01857)
- Towards Analyzing and Understanding the Limitations of DPO: A Theoretical Perspective [![arXiv](https://img.shields.io/badge/arXiv-2404.04626-b31b1b.svg)](https://arxiv.org/abs/2404.04626)

- 3D-Properties: Identifying Challenges in DPO and Charting a Path Forward [![arXiv](https://img.shields.io/badge/arXiv-2406.07327-b31b1b.svg)](https://arxiv.org/abs/2406.07327)
- Unintentional Unalignment: Likelihood Displacement in Direct Preference Optimization [![arXiv](https://img.shields.io/badge/arXiv-2410.08847-b31b1b.svg)](https://arxiv.org/abs/2410.08847)
- Understanding Likelihood Over-optimisation in Direct Alignment Algorithms [![arXiv](https://img.shields.io/badge/arXiv-2410.11677-b31b1b.svg)](https://arxiv.org/abs/2410.11677)

- Common Pitfalls of Margin-based Preference Optimization in Language Model Alignment [![arXiv](https://img.shields.io/badge/arXiv-2410.13828-b31b1b.svg)](https://arxiv.org/pdf/2410.13828)
- When is RL better than DPO in RLHF? A Representation and Optimization Perspective [[OpenReview]](https://openreview.net/forum?id=lNEFatlsQb)
- Smaug: Fixing Failure Modes of Preference Optimisation with DPO-Positive [![arXiv](https://img.shields.io/badge/arXiv-2402.13228-b31b1b.svg)](https://arxiv.org/abs/2402.13228)

#### Optimization - Alignment

- A Deep Dive into the Trade-Offs of Parameter-Efficient Preference Alignment Techniques [![arXiv](https://img.shields.io/badge/arXiv-2406.04879-b31b1b.svg  )](https://arxiv.org/abs/2406.04879)  
- Preference Learning Algorithms Do Not Learn Preference Rankings [![arXiv](https://img.shields.io/badge/arXiv-2405.19534-b31b1b.svg  )](https://arxiv.org/abs/2405.19534)
- Paft: A parallel training paradigm for effective LLM fine-tuning [![arXiv](https://img.shields.io/badge/arXiv-2024.06-b31b1b.svg)](https://arxiv.org/abs/2406.17923)
- Mitigating the Alignment Tax of RLHF [![arXiv](https://img.shields.io/badge/arXiv-2023.09-b31b1b.svg)](https://arxiv.org/abs/2309.06256)

## Other Surveys



