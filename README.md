# Awesome Direct Preference Optimization

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![arXiv](https://img.shields.io/badge/arXiv-Coming%20Soon-b31b1b.svg)]()
[![Paper](https://img.shields.io/badge/Paper-215-blue.svg)]()

A list of selected papers in our survey paper titled "[A Survey of Direct Preference Optimization]()" (coming soon).

*If you find a missing paper or a possible mistake in our survey, please feel free to open an issue or pull a request here. I am more than glad to receive your advice. Thanks!*

## 📚 Citation
If you find this survey useful for your research, please consider citing
```bib
@article{chen2025reasoning,
      title={A Survey of Direct Preference Optimization}, 
      author={Shunyu Liu and Wenkai Fang and Zetian Hu and Junjie Zhang and Yang Zhou and Kongcheng Zhang and Rongcheng Tu and Ting-En Lin and Fei Huang and Mingli Song and Yongbin Li and Dacheng Tao},
      year={2025}
}
```

## 🔥 News

- **`[Mar 12, 2025]`** We have uploaded our survey paper titled "[A Survey of Direct Preference Optimization]()" to arXiv (coming soon). Please feel free to cite or open pull requests for your awesome studies.

## ✨ Overview 

In this survey, we introduce a novel taxonomy that categorizes existing DPO works into four key dimensions based on different components of the DPO loss: **data strategy**, **learning framework**, **constraint mechanism**, and **model property**. 

<div align="center">
<img src="https://github.com/liushunyu/awesome-direct-preference-optimization/blob/main/framework.png" width="100%">
</div>

This taxonomy provides a systematic framework for understanding the methodological evolution of DPO and highlights the key distinctions between different variations.

<div align="center">
<img src="https://github.com/liushunyu/awesome-direct-preference-optimization/blob/main/taxonomy.png" width="100%">
</div>

## 📖 Table of Contents

- [A Taxonomy of Direct Preference Optimization](#overview)
  - [Basic](#basic)
  - [Data Strategy](#data-strategy)
    - [Data Quality](#data-quality)
    - [Preference Feedback](#preference-feedback)
    - [Preference Granularity](#preference-granularity)
  - [Learning Framework](#learning-framework)
    - [Learning Paradigm](#learning-paradigm)
    - [Learning Objective](#learning-objective)
  - [Constraint Mechanism](#constraint-mechanism)
    - [Reference Model](#reference-model)
    - [Divergence Constraint](#divergence-constraint)
    - [Safety Constraint](#safety-constraint)
  - [Model Property](#model-property)
    - [Generation Property](#generation-property)
    - [Optimization Property](#optimization-property)
    - [Other Analysis](#other-analysis)
  - [Other Surveys](#other-surveys)


## Basic

- [![arXiv](https://img.shields.io/badge/arXiv-2304.05302-b31b1b.svg)](https://arxiv.org/abs/2304.05302) [![arXiv](https://img.shields.io/badge/NeurIPS-2023-blue.svg)](https://arxiv.org/abs/2304.05302) RRHF: Rank responses to align language models with human feedback without tears
- [![arXiv](https://img.shields.io/badge/arXiv-2305.10425-b31b1b.svg)](https://arxiv.org/abs/2305.10425) SLiC-HF: Sequence Likelihood Calibration with Human Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2305.18290-b31b1b.svg)](https://arxiv.org/abs/2305.18290) [![arXiv](https://img.shields.io/badge/NeurIPS-2023-blue.svg)](https://arxiv.org/abs/2305.18290) Direct Preference Optimization: Your Language Model is Secretly a Reward Model
- [![arXiv](https://img.shields.io/badge/arXiv-2306.17492-b31b1b.svg)](https://arxiv.org/abs/2306.17492) [![arXiv](https://img.shields.io/badge/AAAI-2024-blue.svg)](https://arxiv.org/abs/2306.17492) Preference Ranking Optimization for Human Alignment

## Data Strategy

### Data Quality 

#### Data Heterogeneity
- [![arXiv](https://img.shields.io/badge/arXiv-2405.14953-b31b1b.svg)](https://arxiv.org/abs/2405.14953) MallowsPO: Fine-Tune Your LLM with Preference Dispersions
- [![arXiv](https://img.shields.io/badge/arXiv-2405.15065-b31b1b.svg)](https://arxiv.org/abs/2405.15065) Direct Preference Optimization With Unobserved Preference Heterogeneity
- [![arXiv](https://img.shields.io/badge/arXiv-2405.20304-b31b1b.svg)](https://arxiv.org/abs/2405.20304) Group Robust Preference Optimization in Reward-free RLHF
- [![arXiv](https://img.shields.io/badge/arXiv-2412.20299-b31b1b.svg)](https://arxiv.org/abs/2412.20299) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2412.20299) No Preference Left Behind: Group Distributional Preference Optimization

#### Data Distinguishability
- [![arXiv](https://img.shields.io/badge/arXiv-2402.10571-b31b1b.svg)](https://arxiv.org/abs/2402.10571) [![arXiv](https://img.shields.io/badge/ACL%20Findings-2024-blue.svg)](https://arxiv.org/abs/2402.10571) Direct Preference Optimization with an Offset
- [![arXiv](https://img.shields.io/badge/arXiv-2403.07230-b31b1b.svg)](https://arxiv.org/abs/2403.07230) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2403.07230) Enhancing Alignment using Curriculum Learning & Ranked Preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2403.19270-b31b1b.svg)](https://arxiv.org/abs/2403.19270) sDPO: Don't Use Your Data All at Once
- [![arXiv](https://img.shields.io/badge/arXiv-2403.19443-b31b1b.svg)](https://arxiv.org/abs/2403.19443) Mixed Preference Optimization: Reinforcement Learning with Data Selection and Better Reference Model
- [![arXiv](https://img.shields.io/badge/arXiv-2404.13846-b31b1b.svg)](https://arxiv.org/abs/2404.13846) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2404.13846) Filtered Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2405.21040-b31b1b.svg)](https://arxiv.org/abs/2405.21040) Direct Alignment of Language Models via Quality-Aware Self-Refinement
- [![arXiv](https://img.shields.io/badge/arXiv-2406.02764-b31b1b.svg)](https://arxiv.org/abs/2406.02764) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.02764) Adaptive Preference Scaling for Reinforcement Learning with Human Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2407.08639-b31b1b.svg)](https://arxiv.org/abs/2407.08639) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2407.08639) $\beta$-dpo: Direct preference optimization with dynamic $\beta$
- [![arXiv](https://img.shields.io/badge/arXiv-2408.09385-b31b1b.svg)](https://arxiv.org/abs/2408.09385) [![arXiv](https://img.shields.io/badge/EMNLP%20Findings-2024-blue.svg)](https://arxiv.org/abs/2408.09385) Reward Difference Optimization for Sample Reweighting in Offline RLHF
- [![arXiv](https://img.shields.io/badge/arXiv-2409.06691-b31b1b.svg)](https://arxiv.org/abs/2409.06691) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2409.06691) Geometric-Averaged Preference Optimization for Soft Preference Labels
- [![arXiv](https://img.shields.io/badge/arXiv-2410.10148-b31b1b.svg)](https://arxiv.org/abs/2410.10148) α -DPO: Adaptive Reward Margin is What Direct Preference Optimization Needs
- [![arXiv](https://img.shields.io/badge/arXiv-2412.20996-b31b1b.svg)](https://arxiv.org/abs/2412.20996) Plug-and-Play Training Framework for Preference Optimization
- [![OpenReview](https://img.shields.io/badge/OpenReview-2024-blue)](https://openreview.net/forum?id=N2sN3LESoW) Gap-Aware Preference Optimization: Enhancing Model Alignment with Perception Margin

#### Data Noise
- [![arXiv](https://img.shields.io/badge/arXiv-2403.00409-b31b1b.svg)](https://arxiv.org/abs/2403.00409) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2403.00409) Provably Robust DPO: Aligning Language Models with Noisy Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2404.04102-b31b1b.svg)](https://arxiv.org/abs/2404.04102) ROPO: Robust Preference Optimization for Large Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2404.09824-b31b1b.svg)](https://arxiv.org/abs/2404.09824) [![arXiv](https://img.shields.io/badge/COLM-2024-blue.svg)](https://arxiv.org/abs/2404.09824) Impact of Preference Noise on the Alignment Performance of Generative Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2406.04412-b31b1b.svg)](https://arxiv.org/abs/2406.04412) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2406.04412) Spread Preference Annotation: Direct Preference Judgment for Efficient LLM Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2407.07880-b31b1b.svg)](https://arxiv.org/abs/2407.07880) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2407.07880) Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization
- [![OpenReview](https://img.shields.io/badge/OpenReview-2024-blue)](https://openreview.net/forum?id=H8gLQwg1eC) Understanding Generalization of Preference Optimization Under Noisy Feedback
- [![OpenReview](https://img.shields.io/badge/OpenReview-2024-blue)](https://openreview.net/forum?id=MlxeUVCQgD) Combating inherent noise for direct preference optimization
- [![OpenReview](https://img.shields.io/badge/NeurIPS-2024-blue)](https://openreview.net/forum?id=OUXnnPJzXJ) Perplexity-aware Correction for Robust Alignment with Noisy Preferences

### Preference Feedback

#### Point-Wise Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2312.02554-b31b1b.svg)](https://arxiv.org/abs/2312.02554) ULMA: Unified Language Model Alignment with Human Demonstration and Point-wise Preference
- [![arXiv](https://img.shields.io/badge/arXiv-2402.01306-b31b1b.svg)](https://arxiv.org/abs/2402.01306) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2402.01306) KTO: Model Alignment as Prospect Theoretic Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2402.05369-b31b1b.svg)](https://arxiv.org/abs/2402.05369) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2402.05369) Noise Contrastive Alignment of Language Models with Explicit Rewards
- [![arXiv](https://img.shields.io/badge/arXiv-2404.04656-b31b1b.svg)](https://arxiv.org/abs/2404.04656) Binary Classifier Optimization for Large Language Model Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19107-b31b1b.svg)](https://arxiv.org/abs/2405.19107) Offline Regularised Reinforcement Learning for Large Language Models Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2406.05882-b31b1b.svg)](https://arxiv.org/abs/2406.05882) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.05882) Distributional Preference Alignment of LLMs via Optimal Transport
- [![arXiv](https://img.shields.io/badge/arXiv-2410.02197-b31b1b.svg)](https://arxiv.org/abs/2410.02197) General Preference Modeling with Preference Representations for Aligning Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2412.14516-b31b1b.svg)](https://arxiv.org/abs/2412.14516) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2412.14516) Cal-DPO: Calibrated Direct Preference Optimization for Language Model Alignment

#### Pair-Wise Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2305.18290-b31b1b.svg)](https://arxiv.org/abs/2305.18290) [![arXiv](https://img.shields.io/badge/NeurIPS-2023-blue.svg)](https://arxiv.org/abs/2305.18290) Direct Preference Optimization: Your Language Model is Secretly a Reward Model
- [![arXiv](https://img.shields.io/badge/arXiv-2310.12036-b31b1b.svg)](https://arxiv.org/abs/2310.12036) [![arXiv](https://img.shields.io/badge/AISTATS-2024-blue.svg)](https://arxiv.org/abs/2310.12036) A General Theoretical Paradigm to Understand Learning from Human Preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2403.03419-b31b1b.svg)](https://arxiv.org/abs/2403.03419) Negating negatives: Alignment without human positive samples via distributional dispreference optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2404.05868-b31b1b.svg)](https://arxiv.org/abs/2404.05868) [![arXiv](https://img.shields.io/badge/COLM-2024-blue.svg)](https://arxiv.org/abs/2404.05868) Negative preference optimization: From catastrophic collapse to effective unlearning
- [![arXiv](https://img.shields.io/badge/arXiv-2405.20830-b31b1b.svg)](https://arxiv.org/abs/2405.20830) Self-Augmented Preference Optimization: Off-Policy Paradigms for Language Model Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2408.07471-b31b1b.svg)](https://arxiv.org/abs/2408.07471) Bridging and Modeling Correlations in Pairwise Data for Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2409.17431-b31b1b.svg)](https://arxiv.org/abs/2409.17431) On Extending Direct Preference Optimization to Accommodate Ties
- [![arXiv](https://img.shields.io/badge/arXiv-2410.04166-b31b1b.svg)](https://arxiv.org/abs/2410.04166) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2410.04166) Preference Optimization as Probabilistic Inference
- [![arXiv](https://img.shields.io/badge/arXiv-2410.07163-b31b1b.svg)](https://arxiv.org/abs/2410.07163) Simplicity Prevails: Rethinking Negative Preference Optimization for LLM Unlearning
- [![arXiv](https://img.shields.io/badge/arXiv-2411.06208-b31b1b.svg)](https://arxiv.org/abs/2411.06208) IOPO: Empowering LLMs with Complex Instruction Following via Input-Output Preference Optimization

#### List-Wise Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2402.01878-b31b1b.svg)](https://arxiv.org/abs/2402.01878) LiPO: Listwise Preference Optimization through Learning-to-Rank
- [![arXiv](https://img.shields.io/badge/arXiv-2402.02030-b31b1b.svg)](https://arxiv.org/abs/2402.02030) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2402.02030) Panacea: Pareto Alignment via Preference Adaptation for LLMs
- [![arXiv](https://img.shields.io/badge/arXiv-2402.10958-b31b1b.svg)](https://arxiv.org/abs/2402.10958) Relative Preference Optimization: Enhancing LLM Alignment through Contrasting Responses across Identical and Diverse Prompts
- [![arXiv](https://img.shields.io/badge/arXiv-2405.13516-b31b1b.svg)](https://arxiv.org/abs/2405.13516) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2405.13516) LIRE: listwise reward enhancement for preference alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2410.04346-b31b1b.svg)](https://arxiv.org/abs/2410.04346) Ordinal Preference Optimization: Aligning Human Preferences via NDCG
- [![arXiv](https://img.shields.io/badge/arXiv-2410.12138-b31b1b.svg)](https://arxiv.org/abs/2410.12138) Preference Optimization with Multi-Sample Comparisons
- [![arXiv](https://img.shields.io/badge/arXiv-2410.18127-b31b1b.svg)](https://arxiv.org/abs/2410.18127) Optimizing Preference Alignment with Differentiable NDCG Ranking
- [![arXiv](https://img.shields.io/badge/arXiv-2411.02442-b31b1b.svg)](https://arxiv.org/abs/2411.02442) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2411.02442) TODO: Enhancing LLM Alignment with Ternary Preferences

### Preference Granularity

#### Token-Level Granularity
- [![arXiv](https://img.shields.io/badge/arXiv-2404.11999-b31b1b.svg)](https://arxiv.org/abs/2404.11999) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2404.11999) Token-level Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2404.12358-b31b1b.svg)](https://arxiv.org/abs/2404.12358) [![arXiv](https://img.shields.io/badge/COLM-2024-blue.svg)](https://arxiv.org/abs/2404.12358) From r to Q∗: Your Language Model is Secretly a Q-Function
- [![arXiv](https://img.shields.io/badge/arXiv-2404.18922-b31b1b.svg)](https://arxiv.org/abs/2404.18922) DPO Meets PPO: Reinforced Token Optimization for RLHF
- [![arXiv](https://img.shields.io/badge/arXiv-2408.13518-b31b1b.svg)](https://arxiv.org/abs/2408.13518) Selective Preference Optimization via Token-Level Reward Function Estimation
- [![arXiv](https://img.shields.io/badge/arXiv-2408.16090-b31b1b.svg)](https://arxiv.org/abs/2408.16090) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2408.16090) EPO: Hierarchical LLM Agents with Environment Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2410.04350-b31b1b.svg)](https://arxiv.org/abs/2410.04350) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2410.04350) TIS-DPO: Token-level Importance Sampling for Direct Preference Optimization With Estimated Weights
- [![arXiv](https://img.shields.io/badge/arXiv-2410.05102-b31b1b.svg)](https://arxiv.org/abs/2410.05102) SparsePO: Controlling Preference Alignment of LLMs via Sparse Token Masks
- [![arXiv](https://img.shields.io/badge/arXiv-2502.14340-b31b1b.svg)](https://arxiv.org/abs/2502.14340) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2502.14340) Earlier Tokens Contribute More: Learning Direct Preference Optimization From Temporal Decay Perspective

#### Step-Level Granularity
- [![arXiv](https://img.shields.io/badge/arXiv-2405.00451-b31b1b.svg)](https://arxiv.org/abs/2405.00451) Monte Carlo Tree Search Boosts Reasoning via Iterative Preference Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2406.09136-b31b1b.svg)](https://arxiv.org/abs/2406.09136) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.09136) Chain of Preference Optimization: Improving Chain-of-Thought Reasoning in LLMs
- [![arXiv](https://img.shields.io/badge/arXiv-2406.18629-b31b1b.svg)](https://arxiv.org/abs/2406.18629) Step-DPO: Step-wise Preference Optimization for Long-chain Reasoning of LLMs
- [![arXiv](https://img.shields.io/badge/arXiv-2407.00782-b31b1b.svg)](https://arxiv.org/abs/2407.00782) Step-controlled dpo: Leveraging stepwise error for enhanced mathematical reasoning
- [![arXiv](https://img.shields.io/badge/arXiv-2407.14477-b31b1b.svg)](https://arxiv.org/abs/2407.14477) Data-Centric Human Preference Optimization with Rationales
- [![arXiv](https://img.shields.io/badge/arXiv-2410.12854-b31b1b.svg)](https://arxiv.org/abs/2410.12854) TPO: Aligning Large Language Models with Multi-branch & Multi-step Preference Trees
- [![arXiv](https://img.shields.io/badge/arXiv-2412.18279-b31b1b.svg)](https://arxiv.org/abs/2412.18279) Improving Multi-Step Reasoning Abilities of Large Language Models with Direct Advantage Policy Optimization

#### Sentence-Level Granularity
- [![arXiv](https://img.shields.io/badge/arXiv-2305.18290-b31b1b.svg)](https://arxiv.org/abs/2305.18290) [![arXiv](https://img.shields.io/badge/NeurIPS-2023-blue.svg)](https://arxiv.org/abs/2305.18290) Direct Preference Optimization: Your Language Model is Secretly a Reward Model
- [![arXiv](https://img.shields.io/badge/arXiv-2401.06838-b31b1b.svg)](https://arxiv.org/abs/2401.06838) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2401.06838) MAPO: Advancing Multilingual Reasoning through Multilingual-Alignment-as-Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2404.02078-b31b1b.svg)](https://arxiv.org/abs/2404.02078) Advancing LLM Reasoning Generalists with Preference Trees
- [![arXiv](https://img.shields.io/badge/arXiv-2404.19733-b31b1b.svg)](https://arxiv.org/abs/2404.19733) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2404.19733) Iterative Reasoning Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2410.01691-b31b1b.svg)](https://arxiv.org/abs/2410.01691) FactAlign: Long-form factuality alignment of large language models

#### Turn-Level Granularity
- [![arXiv](https://img.shields.io/badge/arXiv-2403.02502-b31b1b.svg)](https://arxiv.org/abs/2403.02502) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2403.02502) Trial and Error: Exploration-Based Trajectory Optimization for LLM Agents
- [![arXiv](https://img.shields.io/badge/arXiv-2406.14868-b31b1b.svg)](https://arxiv.org/abs/2406.14868) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2406.14868) Direct Multi-Turn Preference Optimization for Language Agents
- [![arXiv](https://img.shields.io/badge/arXiv-2408.07199-b31b1b.svg)](https://arxiv.org/abs/2408.07199) Agent Q: Advanced Reasoning and Learning for Autonomous AI Agents
- [![arXiv](https://img.shields.io/badge/arXiv-2409.02392-b31b1b.svg)](https://arxiv.org/abs/2409.02392) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2409.02392) Building Math Agents with Multi-Turn Iterative Preference Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2501.01821-b31b1b.svg)](https://arxiv.org/abs/2501.01821) SDPO: Segment-Level Direct Preference Optimization for Social Agents

## Learning Framework

### Learning Paradigm

#### Offline Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2305.18290-b31b1b.svg)](https://arxiv.org/abs/2305.18290) [![arXiv](https://img.shields.io/badge/NeurIPS-2023-blue.svg)](https://arxiv.org/abs/2305.18290) Direct Preference Optimization: Your Language Model is Secretly a Reward Model
- [![arXiv](https://img.shields.io/badge/arXiv-2312.02554-b31b1b.svg)](https://arxiv.org/abs/2312.02554) ULMA: Unified Language Model Alignment with Human Demonstration and Point-wise Preference
- [![arXiv](https://img.shields.io/badge/arXiv-2401.08417-b31b1b.svg)](https://arxiv.org/abs/2401.08417) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.08417) Contrastive preference optimization: Pushing the boundaries of LLM performance in machine translation
- [![arXiv](https://img.shields.io/badge/arXiv-2401.11458-b31b1b.svg)](https://arxiv.org/abs/2401.11458) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.11458) Linear Alignment: A Closed-form Solution for Aligning Human Preferences without Tuning and Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2402.09320-b31b1b.svg)](https://arxiv.org/abs/2402.09320) ICDPO: Effectively Borrowing Alignment Capability of Others via In-context Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2403.07230-b31b1b.svg)](https://arxiv.org/abs/2403.07230) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2403.07230) Enhancing Alignment using Curriculum Learning & Ranked Preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2403.07691-b31b1b.svg)](https://arxiv.org/abs/2403.07691) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2403.07691) ORPO: Monolithic Preference Optimization without Reference Model
- [![arXiv](https://img.shields.io/badge/arXiv-2403.19270-b31b1b.svg)](https://arxiv.org/abs/2403.19270) sDPO: Don't Use Your Data All at Once
- [![arXiv](https://img.shields.io/badge/arXiv-2406.17923-b31b1b.svg)](https://arxiv.org/abs/2406.17923) Paft: A parallel training paradigm for effective LLM fine-tuning

#### Online Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2309.06657-b31b1b.svg)](https://arxiv.org/abs/2309.06657) [![arXiv](https://img.shields.io/badge/ICLR-2024-blue.svg)](https://arxiv.org/abs/2309.06657) Statistical rejection sampling improves preference optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2312.11456-b31b1b.svg)](https://arxiv.org/abs/2312.11456) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2312.11456) Iterative Preference Learning from Human Feedback: Bridging Theory and Practice for RLHF under KL-constraint
- [![arXiv](https://img.shields.io/badge/arXiv-2312.16682-b31b1b.svg)](https://arxiv.org/abs/2312.16682) Some things are more cringe than others: Iterative preference optimization with the pairwise cringe loss
- [![arXiv](https://img.shields.io/badge/arXiv-2401.10020-b31b1b.svg)](https://arxiv.org/abs/2401.10020) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.10020) Self-Rewarding Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2402.04792-b31b1b.svg)](https://arxiv.org/abs/2402.04792) Direct Language Model Alignment from Online AI Feedback 
- [![arXiv](https://img.shields.io/badge/arXiv-2402.10038-b31b1b.svg)](https://arxiv.org/abs/2402.10038) [![arXiv](https://img.shields.io/badge/NAACL-2024-blue.svg)](https://arxiv.org/abs/2402.10038) RS-DPO: A Hybrid Rejection Sampling and Direct Preference Optimization Method for Alignment of Large Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2402.11907-b31b1b.svg)](https://arxiv.org/abs/2402.11907) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2402.11907) Direct large language model alignment through self-rewarding contrastive prompt distillation
- [![arXiv](https://img.shields.io/badge/arXiv-2403.02502-b31b1b.svg)](https://arxiv.org/abs/2403.02502) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2403.02502) Trial and Error: Exploration-Based Trajectory Optimization for LLM Agents
- [![arXiv](https://img.shields.io/badge/arXiv-2403.19443-b31b1b.svg)](https://arxiv.org/abs/2403.19443) Mixed Preference Optimization: Reinforcement Learning with Data Selection and Better Reference Model
- [![arXiv](https://img.shields.io/badge/arXiv-2404.04102-b31b1b.svg)](https://arxiv.org/abs/2404.04102) ROPO: Robust Preference Optimization for Large Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2404.10719-b31b1b.svg)](https://arxiv.org/abs/2404.10719) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2404.10719) Is DPO Superior to PPO for LLM Alignment? A Comprehensive Study
- [![arXiv](https://img.shields.io/badge/arXiv-2404.19733-b31b1b.svg)](https://arxiv.org/abs/2404.19733) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2404.19733) Iterative Reasoning Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2405.00451-b31b1b.svg)](https://arxiv.org/abs/2405.00451) Monte Carlo Tree Search Boosts Reasoning via Iterative Preference Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2405.01511-b31b1b.svg)](https://arxiv.org/abs/2405.01511) [![arXiv](https://img.shields.io/badge/COLM-2024-blue.svg)](https://arxiv.org/abs/2405.01511) D2PO: Discriminator-Guided DPO with Response Evaluation Models
- [![arXiv](https://img.shields.io/badge/arXiv-2405.08448-b31b1b.svg)](https://arxiv.org/abs/2405.08448) Understanding the performance gap between online and offline alignment algorithms 
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19320-b31b1b.svg)](https://arxiv.org/abs/2405.19320) Value-Incentivized Preference Optimization: A Unified Approach to Online and Offline RLHF
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19332-b31b1b.svg)](https://arxiv.org/abs/2405.19332) Self-Exploring Language Models: Active Preference Elicitation for Online Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2405.21046-b31b1b.svg)](https://arxiv.org/abs/2405.21046) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2405.21046) Exploratory Preference Optimization: Provably Sample-Efficient Exploration in RLHF with General Function Approximation
- [![arXiv](https://img.shields.io/badge/arXiv-2406.01462-b31b1b.svg)](https://arxiv.org/abs/2406.01462) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.01462) The Importance of Online Data: Understanding Preference Fine-tuning via Coverage
- [![arXiv](https://img.shields.io/badge/arXiv-2406.05534-b31b1b.svg)](https://arxiv.org/abs/2406.05534) Online DPO: Online Direct Preference Optimization with Fast-Slow Chasing
- [![arXiv](https://img.shields.io/badge/arXiv-2406.07657-b31b1b.svg)](https://arxiv.org/abs/2406.07657) OPTune: Efficient Online Preference Tuning
- [![arXiv](https://img.shields.io/badge/arXiv-2406.12168-b31b1b.svg)](https://arxiv.org/abs/2406.12168) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2406.12168) BPO: Supercharging Online Preference Learning by Adhering to the Proximity of Behavior LLM
- [![arXiv](https://img.shields.io/badge/arXiv-2407.18248-b31b1b.svg)](https://arxiv.org/abs/2407.18248) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2407.18248) Self-training with direct preference optimization improves chain-of-thought reasoning
- [![arXiv](https://img.shields.io/badge/arXiv-2409.02392-b31b1b.svg)](https://arxiv.org/abs/2409.02392) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2409.02392) Building Math Agents with Multi-Turn Iterative Preference Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2409.08845-b31b1b.svg)](https://arxiv.org/abs/2409.08845) AIPO: Improving Training Objective for Iterative Preference Optimization 
- [![arXiv](https://img.shields.io/badge/arXiv-2409.19605-b31b1b.svg)](https://arxiv.org/abs/2409.19605) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2409.19605) The Crucial Role of Samplers in Online Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2410.06293-b31b1b.svg)](https://arxiv.org/abs/2410.06293) Accelerated Preference Optimization for Large Language Model Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2410.06293-b31b1b.svg)](https://arxiv.org/abs/2410.06293) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2410.06293) SeRA: Self-Review & Alignment with Implicit Reward Margins
- [![arXiv](https://img.shields.io/badge/arXiv-2410.12735-b31b1b.svg)](https://arxiv.org/abs/2410.12735) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2410.12735) CREAM: Consistency Regularized Self-Rewarding Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2410.23223-b31b1b.svg)](https://arxiv.org/abs/2410.23223) COMAL: A Convergent Meta-Algorithm for Aligning LLMs with General Preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2501.12735-b31b1b.svg)](https://arxiv.org/abs/2501.12735) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2501.12735) Online Preference Alignment for Language Models via Count-based Exploration


#### Active Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2402.08114-b31b1b.svg)](https://arxiv.org/abs/2402.08114) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2402.08114) Active Preference Learning for Large Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2402.09401-b31b1b.svg)](https://arxiv.org/abs/2402.09401) Reinforcement Learning from Human Feedback with Active Queries 
- [![arXiv](https://img.shields.io/badge/arXiv-2402.10500-b31b1b.svg)](https://arxiv.org/abs/2402.10500) Active Preference Optimization for Sample Efficient RLHF 
- [![OpenReview](https://img.shields.io/badge/OpenReview-2024-blue)](https://openreview.net/forum?id=bRfVj0Sh88) Active Preference Optimization via Maximizing Learning Capacity

### Learning Objective

#### Multi-Objective Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2310.03708-b31b1b.svg)](https://arxiv.org/abs/2310.03708) [![arXiv](https://img.shields.io/badge/ACL%20Findings-2024-blue.svg)](https://arxiv.org/abs/2310.03708) Beyond one-preference-fits-all alignment: Multi-objective direct preference optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2402.19085-b31b1b.svg)](https://arxiv.org/abs/2402.19085) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2402.19085) Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2405.12739-b31b1b.svg)](https://arxiv.org/abs/2405.12739) SPO: Multi-Dimensional Preference Sequential Alignment With Implicit Reward Modeling
- [![arXiv](https://img.shields.io/badge/arXiv-2405.17956-b31b1b.svg)](https://arxiv.org/abs/2405.17956) Hybrid Preference Optimization: Augmenting Direct Preference Optimization with Auxiliary Objectives
- [![arXiv](https://img.shields.io/badge/arXiv-2410.08458-b31b1b.svg)](https://arxiv.org/abs/2410.08458) Simultaneous Reward Distillation and Preference Learning: Get You a Language Model Who Can Do Both
- [![OpenReview](https://img.shields.io/badge/OpenReview-2024-blue)](https://openreview.net/forum?id=w0MAu8vjwj) MOSLIM: Align with diverse preferences in prompts through reward classification

#### Self-Play Learning
- [![arXiv](https://img.shields.io/badge/arXiv-2312.00886-b31b1b.svg)](https://arxiv.org/abs/2312.00886) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2312.00886) Nash learning from human feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2401.01335-b31b1b.svg)](https://arxiv.org/abs/2401.01335) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.01335) Self-play fine-tuning converts weak language models to strong language models
- [![arXiv](https://img.shields.io/badge/arXiv-2401.04056-b31b1b.svg)](https://arxiv.org/abs/2401.04056) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.04056) A minimaximalist approach to reinforcement learning from human feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2403.08635-b31b1b.svg)](https://arxiv.org/abs/2403.08635) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2403.08635) Human Alignment of Large Language Models through Online Preference Optimisation
- [![arXiv](https://img.shields.io/badge/arXiv-2404.03715-b31b1b.svg)](https://arxiv.org/abs/2404.03715) Direct nash optimization: Teaching language models to self-improve with general preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2405.00675-b31b1b.svg)](https://arxiv.org/abs/2405.00675) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2405.00675) Self-Play Preference Optimization for Language Model Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2406.00832-b31b1b.svg)](https://arxiv.org/abs/2406.00832) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.00832) BoNBoN Alignment for Large Language Models and the Sweetness of Best-of-n Sampling
- [![arXiv](https://img.shields.io/badge/arXiv-2406.01660-b31b1b.svg)](https://arxiv.org/abs/2406.01660) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2406.01660) Self-Improving Robust Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2502.05400-b31b1b.svg)](https://arxiv.org/abs/2502.05400) Dynamic Noise Preference Optimization for LLM Self-Improvement via Synthetic Data 

## Constraint Mechanism

### Reference Model

#### Reference-Free DPO
- [![arXiv](https://img.shields.io/badge/arXiv-2401.08417-b31b1b.svg)](https://arxiv.org/abs/2401.08417) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.08417) Contrastive preference optimization: Pushing the boundaries of LLM performance in machine translation
- [![arXiv](https://img.shields.io/badge/arXiv-2403.07691-b31b1b.svg)](https://arxiv.org/abs/2403.07691) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2403.07691) ORPO: Monolithic Preference Optimization without Reference Model
- [![arXiv](https://img.shields.io/badge/arXiv-2405.14734-b31b1b.svg)](https://arxiv.org/abs/2405.14734) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2405.14734) SimPO: Simple Preference Optimization with a Reference-Free Reward
- [![arXiv](https://img.shields.io/badge/arXiv-2407.13709-b31b1b.svg)](https://arxiv.org/abs/2407.13709) Understanding reference policies in direct preference optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2502.00883-b31b1b.svg)](https://arxiv.org/abs/2502.00883) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2502.00883) SimPER: Simple Preference Fine-Tuning without Hyperparameters by Perplexity Optimization

#### Dynamic-Reference DPO
- [![arXiv](https://img.shields.io/badge/arXiv-2403.07230-b31b1b.svg)](https://arxiv.org/abs/2403.07230) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2403.07230) Enhancing Alignment using Curriculum Learning & Ranked Preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2403.19443-b31b1b.svg)](https://arxiv.org/abs/2403.19443) Mixed Preference Optimization: Reinforcement Learning with Data Selection and Better Reference Model
- [![arXiv](https://img.shields.io/badge/arXiv-2404.09656-b31b1b.svg)](https://arxiv.org/abs/2404.09656) Learn Your Reference Model for Real Good Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2409.02392-b31b1b.svg)](https://arxiv.org/abs/2409.02392) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2409.02392) Building Math Agents with Multi-Turn Iterative Preference Learning



### Divergence Constraint

#### Diversity
- [![arXiv](https://img.shields.io/badge/arXiv-2309.16240-b31b1b.svg)](https://arxiv.org/abs/2309.16240) [![arXiv](https://img.shields.io/badge/ICLR-2024-blue.svg)](https://arxiv.org/abs/2309.16240) Beyond Reverse KL- Generalizing Direct Preference Optimization with Diverse Divergence Constraints
- [![OpenReview](https://img.shields.io/badge/ICLR-2025-blue)](https://openreview.net/forum?id=pOq9vDIYev) Diverse Preference Learning for Capabilities and Alignment

#### Generalization
- [![arXiv](https://img.shields.io/badge/arXiv-2402.00856-b31b1b.svg)](https://arxiv.org/abs/2402.00856) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2402.00856) Towards Efficient Exact Optimization of Language Model Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2402.05749-b31b1b.svg)](https://arxiv.org/abs/2402.05749) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2402.05749) Generalized Preference Optimization: A Unified Approach to Offline Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2405.00747-b31b1b.svg)](https://arxiv.org/abs/2405.00747) Soft Preference Optimization: Aligning Language Models to Expert Distributions
- [![arXiv](https://img.shields.io/badge/arXiv-2407.03051-b31b1b.svg)](https://arxiv.org/abs/2407.03051) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2407.03051) Improving Conversational Abilities of Quantized Large Language Models via Direct Preference Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2407.13399-b31b1b.svg)](https://arxiv.org/abs/2407.13399) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2407.13399) Correcting the Mythos of KL-Regularization: Direct Alignment without Overoptimization via Chi-Squared Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2410.00508-b31b1b.svg)](https://arxiv.org/abs/2410.00508) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2410.00508) FlipGuard: Defending Preference Alignment against Update Regression with Constrained Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2411.07618-b31b1b.svg)](https://arxiv.org/abs/2411.07618) Direct Preference Optimization Using Sparse Feature-level Constraints
- [![arXiv](https://img.shields.io/badge/arXiv-2501.03271-b31b1b.svg)](https://arxiv.org/abs/2501.03271) DPO Kernels: A Semantically-Aware, Kernel-Enhanced, and Divergence-Rich Paradigm for Direct Preference Optimization

### Safety Constraint
- [![arXiv](https://img.shields.io/badge/arXiv-2401.01967-b31b1b.svg)](https://arxiv.org/abs/2401.01967) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2401.01967) A Mechanistic Understanding of Alignment Algorithms: A Case Study on DPO and Toxicity
- [![arXiv](https://img.shields.io/badge/arXiv-2404.11049-b31b1b.svg)](https://arxiv.org/abs/2404.11049) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2404.11049) Stepwise Alignment for Constrained Language Model Policy Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2403.02475-b31b1b.svg)](https://arxiv.org/abs/2403.02475) Enhancing LLM Safety via Constrained Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2405.12900-b31b1b.svg)](https://arxiv.org/abs/2405.12900) Adversarial DPO: Harnessing Harmful Data for Reducing Toxicity with Minimal Impact on Coherence and Evasiveness in Dialogue Agents
- [![arXiv](https://img.shields.io/badge/arXiv-2409.14586-b31b1b.svg)](https://arxiv.org/abs/2409.14586) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2409.14586) Backtracking Improves Generation Safety
- [![OpenReview](https://img.shields.io/badge/OpenReview-2024-blue)](https://openreview.net/forum?id=MoJSnVZ59d) SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety


## Model Property

### Generation Property

#### Distribution Shift
- [![arXiv](https://img.shields.io/badge/arXiv-2404.14367-b31b1b.svg)](https://arxiv.org/abs/2404.14367) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2404.14367) Preference Fine-Tuning of LLMs Should Leverage Suboptimal, On-Policy Data
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19316-b31b1b.svg)](https://arxiv.org/abs/2405.19316) Robust Preference Optimization through Reward Model Distillation
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19332-b31b1b.svg)](https://arxiv.org/abs/2405.19332) Self-Exploring Language Models: Active Preference Elicitation for Online Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2406.01660-b31b1b.svg)](https://arxiv.org/abs/2406.01660) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2406.01660) Self-Improving Robust Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2407.18676-b31b1b.svg)](https://arxiv.org/abs/2407.18676) Right Now, Wrong Then: Non-Stationary Direct Preference Optimization under Preference Drift
- [![arXiv](https://img.shields.io/badge/arXiv-2409.03650-b31b1b.svg)](https://arxiv.org/abs/2409.03650) [![arXiv](https://img.shields.io/badge/EMNLP%20Findings-2024-blue.svg)](https://arxiv.org/abs/2409.03650) On the limited generalization capability of the implicit reward model induced by direct preference optimization

#### Length Bias
- [![arXiv](https://img.shields.io/badge/arXiv-2304.05302-b31b1b.svg)](https://arxiv.org/abs/2304.05302) [![arXiv](https://img.shields.io/badge/NeurIPS-2023-blue.svg)](https://arxiv.org/abs/2304.05302) RRHF: Rank responses to align language models with human feedback without tears
- [![arXiv](https://img.shields.io/badge/arXiv-2310.03716-b31b1b.svg)](https://arxiv.org/abs/2310.03716) [![arXiv](https://img.shields.io/badge/COLM-2024-blue.svg)](https://arxiv.org/abs/2310.03716) A Long Way to Go: Investigating Length Correlations in RLHF
- [![arXiv](https://img.shields.io/badge/arXiv-2403.19159-b31b1b.svg)](https://arxiv.org/abs/2403.19159) [![arXiv](https://img.shields.io/badge/ACL%20Findings-2024-blue.svg)](https://arxiv.org/abs/2403.19159) Disentangling Length from Quality in Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2405.14734-b31b1b.svg)](https://arxiv.org/abs/2405.14734) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2405.14734) SimPO: Simple Preference Optimization with a Reference-Free Reward
- [![arXiv](https://img.shields.io/badge/arXiv-2406.10957-b31b1b.svg)](https://arxiv.org/abs/2406.10957) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2406.10957) Eliminating Biased Length Reliance of Direct Preference Optimization via Down-Sampled KL Divergence
- [![arXiv](https://img.shields.io/badge/arXiv-2406.14868-b31b1b.svg)](https://arxiv.org/abs/2406.14868) [![arXiv](https://img.shields.io/badge/EMNLP-2024-blue.svg)](https://arxiv.org/abs/2406.14868) Direct Multi-Turn Preference Optimization for Language Agents
- [![arXiv](https://img.shields.io/badge/arXiv-2406.17744-b31b1b.svg)](https://arxiv.org/abs/2406.17744) Following length constraints in instructions
- [![arXiv](https://img.shields.io/badge/arXiv-2407.15229-b31b1b.svg)](https://arxiv.org/abs/2407.15229) The Hitchhiker’s Guide to Human Alignment with *PO
- [![arXiv](https://img.shields.io/badge/arXiv-2409.06411-b31b1b.svg)](https://arxiv.org/abs/2409.06411) Length Desensitization in Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2412.17696-b31b1b.svg)](https://arxiv.org/abs/2412.17696) Understanding the Logic of Direct Preference Alignment through Logic
- [![arXiv](https://img.shields.io/badge/arXiv-2502.13922-b31b1b.svg)](https://arxiv.org/abs/2502.13922) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue)](https://arxiv.org/abs/2502.13922) LongPO: Long Context Self-Evolution of Large Language Models through Short-to-Long Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2502.14340-b31b1b.svg)](https://arxiv.org/abs/2502.14340) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2502.14340) Earlier Tokens Contribute More: Learning Direct Preference Optimization From Temporal Decay Perspective


### Optimization Property

#### Likelihood Collapse
- [![arXiv](https://img.shields.io/badge/arXiv-2402.13228-b31b1b.svg)](https://arxiv.org/abs/2402.13228) Smaug: Fixing Failure Modes of Preference Optimisation with DPO-Positive
- [![arXiv](https://img.shields.io/badge/arXiv-2404.04626-b31b1b.svg)](https://arxiv.org/abs/2404.04626) Towards Analyzing and Understanding the Limitations of DPO: A Theoretical Perspective
- [![arXiv](https://img.shields.io/badge/arXiv-2404.12358-b31b1b.svg)](https://arxiv.org/abs/2404.12358) [![arXiv](https://img.shields.io/badge/COLM-2024-blue.svg)](https://arxiv.org/abs/2404.12358) From r to Q∗: Your Language Model is Secretly a Q-Function
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19316-b31b1b.svg)](https://arxiv.org/abs/2405.19316) Robust Preference Optimization through Reward Model Distillation
- [![arXiv](https://img.shields.io/badge/arXiv-2406.07327-b31b1b.svg)](https://arxiv.org/abs/2406.07327) 3D-Properties: Identifying Challenges in DPO and Charting a Path Forward
- [![arXiv](https://img.shields.io/badge/arXiv-2408.06266-b31b1b.svg)](https://arxiv.org/abs/2408.06266) Anchored Preference Optimization and Contrastive Revisions: Addressing Underspecification in Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2410.08847-b31b1b.svg)](https://arxiv.org/abs/2410.08847) Unintentional Unalignment: Likelihood Displacement in Direct Preference Optimization
- [![arXiv](https://img.shields.io/badge/arXiv-2410.11677-b31b1b.svg)](https://arxiv.org/abs/2410.11677) Understanding Likelihood Over-optimisation in Direct Alignment Algorithms
- [![arXiv](https://img.shields.io/badge/arXiv-2410.13828-b31b1b.svg)](https://arxiv.org/abs/2410.13828) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2410.13828) A Common Pitfall of Margin-based Language Model Alignment: Gradient Entanglement


#### Alignment Tax
- [![arXiv](https://img.shields.io/badge/arXiv-2309.06256-b31b1b.svg)](https://arxiv.org/abs/2309.06256) Mitigating the Alignment Tax of RLHF
- [![arXiv](https://img.shields.io/badge/arXiv-2405.17931-b31b1b.svg)](https://arxiv.org/abs/2405.17931) Online Merging Optimizers for Boosting Rewards and Mitigating Tax in Alignment
- [![arXiv](https://img.shields.io/badge/arXiv-2405.19534-b31b1b.svg)](https://arxiv.org/abs/2405.19534) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2405.19534) Preference Learning Algorithms Do Not Learn Preference Rankings
- [![arXiv](https://img.shields.io/badge/arXiv-2406.04879-b31b1b.svg)](https://arxiv.org/abs/2406.04879) [![arXiv](https://img.shields.io/badge/ACL-2024-blue.svg)](https://arxiv.org/abs/2406.04879) A Deep Dive into the Trade-Offs of Parameter-Efficient Preference Alignment Techniques
- [![arXiv](https://img.shields.io/badge/arXiv-2406.17923-b31b1b.svg)](https://arxiv.org/abs/2406.17923) PAFT: A Parallel Training Paradigm for Effective LLM Fine-Tuning


### Other Analysis
- [![arXiv](https://img.shields.io/badge/arXiv-2403.01857-b31b1b.svg)](https://arxiv.org/abs/2403.01857) [![arXiv](https://img.shields.io/badge/ICML-2024-blue.svg)](https://arxiv.org/abs/2403.01857) Reward Model Learning vs. Direct Policy Optimization: A Comparative Analysis of Learning from Human Preferences
- [![arXiv](https://img.shields.io/badge/arXiv-2404.14723-b31b1b.svg)](https://arxiv.org/abs/2404.14723) Insights into Alignment: Evaluating DPO and its Variants Across Multiple Tasks
- [![arXiv](https://img.shields.io/badge/arXiv-2406.08414-b31b1b.svg)](https://arxiv.org/abs/2406.08414) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.08414) Discovering Preference Optimization Algorithms with and for Large Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2406.09279-b31b1b.svg)](https://arxiv.org/abs/2406.09279) [![arXiv](https://img.shields.io/badge/NeurIPS-2024-blue.svg)](https://arxiv.org/abs/2406.09279) Unpacking DPO and PPO: Disentangling Best Practices for Learning from Preference Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2410.04203-b31b1b.svg)](https://arxiv.org/abs/2410.04203) [![arXiv](https://img.shields.io/badge/ICLR-2025-blue.svg)](https://arxiv.org/abs/2410.04203) RainbowPO: A Unified Framework for Combining Improvements in Preference Optimization
- [![OpenReview](https://img.shields.io/badge/ICLR%20Tiny%20Papers-2024-blue)](https://openreview.net/forum?id=lNEFatlsQb) When is RL better than DPO in RLHF? A Representation and Optimization Perspective




## Other Surveys

- [![JMLR](https://img.shields.io/badge/JMLR-2017-blue)](https://www.jmlr.org/papers/v18/16-634.html) A Survey of Preference-Based Reinforcement Learning Methods
- [![arXiv](https://img.shields.io/badge/arXiv-2305.00955-b31b1b.svg)](https://arxiv.org/abs/2305.00955) Bridging the Gap: A Survey on Integrating (Human) Feedback for Natural Language Generation
- [![arXiv](https://img.shields.io/badge/arXiv-2307.12966-b31b1b.svg)](https://arxiv.org/abs/2307.12966) Aligning Large Language Models with Human: A Survey
- [![arXiv](https://img.shields.io/badge/arXiv-2309.15025-b31b1b.svg)](https://arxiv.org/abs/2309.15025) Large Language Model Alignment: A Survey
- [![arXiv](https://img.shields.io/badge/arXiv-2310.07629-b31b1b.svg)](https://arxiv.org/abs/2310.07629) The Past, Present and Better Future of Feedback Learning in Large Language Models for Subjective Human Preferences and Values
- [![arXiv](https://img.shields.io/badge/arXiv-2310.19852-b31b1b.svg)](https://arxiv.org/abs/2310.19852) AI Alignment: A Comprehensive Survey
- [![arXiv](https://img.shields.io/badge/arXiv-2312.14925-b31b1b.svg)](https://arxiv.org/abs/2312.14925) A Survey of Reinforcement Learning from Human Feedback
- [![arXiv](https://img.shields.io/badge/arXiv-2403.04204-b31b1b.svg)](https://arxiv.org/abs/2403.04204) On the Essence and Prospect: An Investigation of Alignment Approaches for Big Models
- [![arXiv](https://img.shields.io/badge/arXiv-2406.11191-b31b1b.svg)](https://arxiv.org/abs/2406.11191) A Survey on Human Preference Learning for Large Language Models
- [![arXiv](https://img.shields.io/badge/arXiv-2407.16216-b31b1b.svg)](https://arxiv.org/abs/2407.16216) A Comprehensive Survey of LLM Alignment Techniques: RLHF, RLAIF, PPO, DPO and More
- [![arXiv](https://img.shields.io/badge/arXiv-2409.02795-b31b1b.svg)](https://arxiv.org/abs/2409.02795) Towards a Unified View of Preference Learning for Large Language Models: A Survey
- [![arXiv](https://img.shields.io/badge/arXiv-2409.11564-b31b1b.svg)](https://arxiv.org/abs/2409.11564) Preference Tuning with Human Feedback on Language, Speech, and Vision Tasks: A Survey
- [![arXiv](https://img.shields.io/badge/arXiv-2410.15595-b31b1b.svg)](https://arxiv.org/abs/2410.15595) A Comprehensive Survey of Direct Preference Optimization: Datasets, Theories, Variants, and Applications

