---
title: Latent brain state dynamics predict early amyloid accumulation and cognitive impairment
title_zh: 潜在脑状态动力学预测早期淀粉样蛋白积累与认知障碍
authors: "Gao, Z., Young, C. B., Lee, B., Roush, R. E., Kotulsky, J., Cisneros, G., Mormino, E., Cohen, A. D., Menon, V., Cai, W."
date: 2026-04-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.31.715655v1.full.pdf"
tags: ["query:cog-eld"]
score: 8.0
evidence: 预测病理性老化中的认知损伤
tldr: 本研究探讨了淀粉样蛋白（Aβ）早期积累对认知的影响，利用贝叶斯切换动态系统（BSDS）模型分析了116名老年人在N-back任务中的高分辨率fMRI数据。研究发现，相比于单纯的Aβ水平，潜在的大脑状态动态性对早期Aβ负担和认知受损更为敏感，能有效预测工作记忆表现及临床症状。这一发现为识别认知衰退高风险个体提供了新的神经标志物和预测框架。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-001.webp\", \"caption\": \"Figure 2. Regional SUVRs in the brain. ACC, anterior cingulate cortex; VentStriatum, ventral striatum; LateralTemporal, lateral temporal lobe; Orbitofrontal, orbital frontal cortex; PCC, posterior cingulate cortex; SuperFrontal, superior frontal gyrus.\", \"page\": 25, \"index\": 1, \"width\": 860, \"height\": 422}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-002.webp\", \"caption\": \"Figure 3. Latent brain state dynamics (mean lifetime) during WM and their relationship to task performance. A. Key regions implicated in cognitive control: frontal-parietal network: bilateral middle frontal gyrus (MFG), frontal eye field (FEF), inferior parietal lobe (IPL); salience network (SN): bilateral anterior insular (AI), dorsal medial frontal cortex (dmPFC); and default mode network (DMN): ventral medial frontal cortex (vmPFC) and posterior cingulate cortex (PCC), as well as visual selective areas in both hemispheres: face fusiform area (FFA), place parahippocampus area (PPA), extrastriate body area (EBA), and tool selective area in middle temporal gyrus (MTG). B. BSDS model: Bayesian switching dynamics states model. C. Latent brain state dynamics were modulated by working memory load. D. Correlation between latent brain state dynamics and task performance in CN and MCI after accounting for age, gender, and head motion. Under 0-back condition, occupancy rate of state S2 was positively associated with efficiency; S4 was negatively associated with efficiency in cognitively normal participants but not MCI. Under 2-back condition, occupancy rate of S2 and S4 did not show significant association with behavior efficiency in both groups. E. Group differences in brain state– behavior coupling in 0-back and 2-back tasks. S2 and S4 occupancy rates show stronger coupling with efficiency in CN than MCI during the 0-back task. * indicates p < 0.05, *** indicates p < 0.001.\", \"page\": 26, \"index\": 2, \"width\": 976, \"height\": 737}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-003.webp\", \"caption\": \"Table 3. Behavioral performance (fMRI + behavior sample)\", \"page\": 29, \"index\": 3, \"width\": 860, \"height\": 294}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-004.webp\", \"caption\": \"Table 1. Demographics (fMRI sample)\", \"page\": 29, \"index\": 4, \"width\": 860, \"height\": 202}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-005.webp\", \"caption\": \"Table 2. Demographics (fMRI + behavior sample)\", \"page\": 29, \"index\": 5, \"width\": 860, \"height\": 202}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-006.webp\", \"caption\": \"Figure 5. Predicting MoCA Scores with Brain Dynamics. A Lasso regression model using brain\", \"page\": 28, \"index\": 6, \"width\": 606, \"height\": 531}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-007.webp\", \"caption\": \"Figure 4. Latent brain state dynamics predict Aβ accumulation. A. Canonical correlation between latent brain state dynamics and regional SUVRs. B. Canonical loading factors. ACC, anterior cingulate cortex; VentStriatum, ventral striatum; LateralTemporal, lateral temporal lobe; Orbitofrontal, orbital frontal cortex; PCC, posterior cingulate cortex; SuperFrontal, superior frontal gyrus.\", \"page\": 27, \"index\": 7, \"width\": 976, \"height\": 311}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715655-v1/fig-008.webp\", \"caption\": \"Figure 1. Reduced behavioral efficiency, accuracy, mean reactive time, and response stability (standard deviation of reaction time) in individuals with MCI. * indicates p < 0.05, *** indicates p < 0.001.\", \"page\": 24, \"index\": 8, \"width\": 976, \"height\": 577}]"
motivation: 旨在探究大脑状态动态性是否能作为早期淀粉样蛋白积累及其引起认知功能下降的敏感神经标志物。
method: 采用贝叶斯切换动态系统模型分析116名受试者在执行工作记忆任务时的高时间分辨率fMRI数据，识别出四种潜在的大脑状态。
result: 大脑状态动态性与早期Aβ负担显著相关，并能成功预测工作记忆表现和认知障碍，而单纯的Aβ水平在这些预测上表现不足。
conclusion: 大脑状态动态性是早期病理变化和认知受损的敏感指标，为开发预测未来认知衰退风险的模型提供了新途径。
---

## 摘要
β-淀粉样蛋白（Aβ）积累是病理性衰老的核心持续过程，在认知障碍出现前数十年便已开始。虽然阈值下 Aβ 水平与未来的认知控制下降有关，但连接这种早期积累及其神经认知影响的神经机制尚不清楚。脑回路动力学对认知功能至关重要，可能为观察这些初始病理变化提供敏感的视角。在本研究中，我们测试了在 Aβ 负荷早期阶段，脑状态动力学是否可以作为认知障碍的敏感标志物。利用贝叶斯切换动态系统（BSDS）模型，我们从 116 名老年人（包括 72 名认知正常 [CN] 个体和 44 名轻度认知障碍 [MCI] 患者）在执行 N-back 工作记忆任务期间获取的高时间分辨率（800 ms）fMRI 数据中，识别出 4 种不同的潜在脑状态。我们采用维度方法，研究了潜在脑状态动力学与早期淀粉样蛋白负荷、认知表现及临床症状之间的关系。虽然 Aβ 水平未能区分临床群体或预测临床症状和任务表现，但潜在脑状态的动力学被证明对早期 Aβ 积累和认知都高度敏感。典型相关分析揭示了脑状态动力学与早期 Aβ 负荷之间存在显著关系。此外，脑状态的时间特性对 CN 个体的工作记忆表现具有显著的预测作用，而这种关系在 MCI 组中被选择性地破坏了。脑动力学特征还能成功预测认知障碍。我们的研究结果确立了脑状态动力学作为初始 Aβ 积累和早期认知障碍的敏感神经标志物，为开发预测模型以识别具有未来认知下降风险的个体提供了新框架。

## Abstract
Amyloid-{beta} (A{beta}) accumulation is a continuous process central to pathological aging that begins decades before cognitive impairment emerges. While subthreshold A{beta} levels have been linked to future decline in cognitive control, the neural mechanisms connecting this early accumulation to its neurocognitive impact are poorly understood. Brain circuit dynamics, which are essential for cognitive function, may offer a sensitive lens into these initial pathological changes. Here, we tested whether brain state dynamics could serve as sensitive markers for cognitive impairment at an early stage of A{beta} burden. Using the Bayesian Switching Dynamic System (BSDS) model, we identified 4 distinct latent brain states from high-temporal-resolution (800 ms) fMRI data acquired from 116 older adults, including 72 cognitively normal (CN) individuals and 44 with mild cognitive impairment (MCI), during an N-back working-memory task. Adopting a dimensional approach, we examined how latent brain state dynamics relate to early amyloid burden, cognitive performance, and clinical symptoms. While A{beta} levels failed to differentiate clinical groups or predict clinical symptoms and task performance, the dynamics of latent brain states proved highly sensitive to both early A{beta} accumulation and cognition. Canonical correlation analysis revealed a significant relationship between brain state dynamics and early A{beta} burden. Furthermore, the temporal properties of brain states were significantly predictive of working memory performance in CN individuals, a relationship that was selectively disrupted in the MCI group. The features of brain dynamics can also successfully predict cognitive impairment. Our findings establish brain state dynamics as sensitive neural markers of initial A{beta} accumulation and early cognitive impairment, offering a new framework for developing predictive models to identify individuals at risk for future cognitive decline.

---

## 论文详细总结（自动生成）

这篇论文题为《潜在脑状态动力学预测早期淀粉样蛋白积累与认知障碍》，由斯坦福大学等机构的研究团队完成。以下是对该论文的结构化深入总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心挑战**：阿尔茨海默病（AD）的病理变化（如β-淀粉样蛋白 Aβ 的积累）在临床症状出现前数十年就已开始。然而，在“阈值下”积累阶段，传统的静态神经影像指标和临床评估往往难以捕捉到细微的脑功能变化。
*   **研究动机**：探索比静态脑激活更敏感的指标。研究者假设，大脑在执行认知任务时的**动态状态切换（Brain State Dynamics）**能够更早地反映出 Aβ 积累对神经回路的影响，并能预测从认知正常（CN）到轻度认知障碍（MCI）的演变。
*   **整体含义**：本研究试图建立“早期病理 -> 脑动力学异常 -> 认知受损”的机械连接，为早期筛查提供新的功能性神经标志物。

### 2. 论文提出的方法论
*   **核心思想**：利用状态空间模型将连续的 fMRI 信号分解为有限个具有特定空间激活和连接模式的“潜在脑状态”，并量化这些状态随时间的演变特征。
*   **关键技术细节**：
    *   **BSDS 模型**：采用**贝叶斯切换动态系统（Bayesian Switching Dynamic System）**。这是一种生成式模型，通过隐藏马尔可夫链（Hidden Markov Chain）建模状态切换。
    *   **高时间分辨率**：使用 TR=800ms 的超快 fMRI 采样，以捕捉快速的脑状态转换。
    *   **动力学指标**：提取两个关键参数：
        1.  **占用率（Occupancy Rate）**：个体处于某一特定状态的时间比例。
        2.  **平均寿命（Mean Lifetime）**：某一状态在切换前持续的平均时长。
    *   **维度分析法**：不局限于简单的组间对比，而是通过典型相关分析（CCA）和 Lasso 回归，在连续维度上考察 Aβ 负荷、脑动力学与认知得分的关系。

### 3. 实验设计
*   **数据集**：来自 HCP-CBA（人类连接组计划-大脑老化与痴呆）研究，包含 116 名老年受试者（72 名 CN，44 名 MCI）。
*   **实验场景**：受试者在扫描仪内执行 **N-back 工作记忆任务**（包含 0-back 低负荷和 2-back 高负荷条件）。
*   **Benchmark 与对比方法**：
    *   **对比指标**：静态单变量 GLM 脑激活、PET 测量的区域及全局 Aβ SUVR（标准化摄取值比值）。
    *   **行为评估**：MoCA（蒙特利尔认知评估量表）得分、任务准确率、反应时间（RT）及效率。
*   **验证方式**：使用留一交叉验证（LOOCV）评估预测模型的泛化能力。

### 4. 资源与算力
*   **算力说明**：论文中**未明确提及**具体的 GPU 型号、数量或具体的训练时长。
*   **计算复杂度**：作者在讨论中提到，BSDS 模型的计算成本随节点数量呈非线性增长，因此本研究将分析限制在 19 个关键网络节点（涉及前额叶、顶叶、显著网络和视觉区），而非全脑分析。

### 5. 实验数量与充分性
*   **实验规模**：
    *   识别出 4 种潜在脑状态（S1-S4）。
    *   进行了行为学差异分析、Aβ 与行为的相关性分析、Aβ 与静态激活的相关性分析。
    *   核心实验包括：脑动力学与 Aβ 的 CCA 分析、脑动力学与行为的组间相关性对比、基于 Lasso 的 MoCA 得分预测。
*   **充分性评价**：实验设计较为充分，涵盖了从行为、病理到功能的多个维度。通过对比发现 Aβ 本身无法预测症状而动力学可以，增强了结论的说服力。但受限于临床样本获取难度，116 人的样本量在机器学习预测层面仍属于中小规模。

### 6. 主要结论与发现
*   **Aβ 的局限性**：在早期阶段，Aβ 负荷无法区分 CN 和 MCI，也无法预测任务表现或静态脑激活。
*   **动力学的敏感性**：脑状态动力学（尤其是状态 S2 和 S4 的占用率）与早期 Aβ 积累显著相关。
*   **脑-行为耦合断裂**：在 CN 组中，脑状态的动态特征能显著预测工作记忆表现；但在 MCI 组中，这种“脑-行为”耦合消失了，表明 MCI 患者虽然能进入相关状态，但无法有效利用这些状态来支持认知。
*   **临床预测**：仅凭脑动力学特征即可成功预测个体的 MoCA 临床评分。

### 7. 优点
*   **动态视角**：克服了传统滑动窗口法（Sliding Window）边界模糊和参数主观的缺点，提供了更精准的时间动力学刻画。
*   **早期预警**：证明了在 Aβ 达到阳性阈值之前，脑功能动力学已经发生了可检测的改变。
*   **多模态整合**：成功将 PET 病理数据、任务态 fMRI 动态数据与临床认知评估整合在一个分析框架内。

### 8. 不足与局限
*   **样本异质性**：MCI 组中 Aβ 阳性率较低，意味着部分 MCI 患者的病因可能非阿尔茨海默病（如血管性因素），这可能干扰对 AD 特异性病理的解释。
*   **空间分辨率受限**：由于计算成本限制，仅分析了 19 个 ROI，可能遗漏了其他脑区的关键动态信息。
*   **横断面设计**：研究是横断面的，无法直接证明脑动力学异常能预测个体未来几年的实际认知下降轨迹（需纵向研究验证）。
*   **因果关系不明**：尚不清楚是 Aβ 导致了动力学异常，还是动力学异常是更广泛神经退行性变的副产品。

（完）
