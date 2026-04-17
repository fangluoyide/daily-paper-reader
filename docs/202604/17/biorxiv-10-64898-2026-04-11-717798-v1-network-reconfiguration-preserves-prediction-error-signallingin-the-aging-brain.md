---
title: Network reconfiguration preserves prediction error signallingin the aging brain
title_zh: 网络重构维持了老龄化大脑中的预测误差信号传导
authors: "Andersen, M. H., Fernandez-Rubio, G., Quiroga-Martinez, D. R., Rosso, M., Klarlund, M., Larsen, K. M., Siebner, H. R., Kringelbach, M. L., Vuust, P., Bonetti, L."
date: 2026-04-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.11.717798v1.full.pdf"
tags: ["query:cog-eld"]
score: 8.0
evidence: 老年大脑中的预测机制
tldr: 本研究挑战了认知老化导致大脑预测机制全面衰退的传统观点。通过对77名受试者的脑磁图数据进行网络分解，研究发现老化对预测子系统具有选择性影响：虽然注意重定向和上下文处理减弱，但感觉预测误差信号在特定网络中反而增强。这表明大脑在衰老过程中通过重新配置网络资源，在维持预测误差信号传导的同时，实现了预测功能的重新分配。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-001.webp\", \"caption\": \"\", \"page\": 6, \"index\": 1, \"width\": 886, \"height\": 309}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-002.webp\", \"caption\": \"\", \"page\": 6, \"index\": 2, \"width\": 886, \"height\": 309}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-003.webp\", \"caption\": \"\", \"page\": 9, \"index\": 3, \"width\": 713, \"height\": 458}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-004.webp\", \"caption\": \"\", \"page\": 9, \"index\": 4, \"width\": 713, \"height\": 458}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-005.webp\", \"caption\": \"\", \"page\": 11, \"index\": 5, \"width\": 862, \"height\": 436}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-006.webp\", \"caption\": \"\", \"page\": 11, \"index\": 6, \"width\": 862, \"height\": 436}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-007.webp\", \"caption\": \"\", \"page\": 11, \"index\": 7, \"width\": 862, \"height\": 435}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-008.webp\", \"caption\": \"\", \"page\": 14, \"index\": 8, \"width\": 883, \"height\": 466}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-009.webp\", \"caption\": \"\", \"page\": 14, \"index\": 9, \"width\": 883, \"height\": 465}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-010.webp\", \"caption\": \"\", \"page\": 16, \"index\": 10, \"width\": 884, \"height\": 333}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-011.webp\", \"caption\": \"\", \"page\": 19, \"index\": 11, \"width\": 884, \"height\": 379}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-012.webp\", \"caption\": \"\", \"page\": 19, \"index\": 12, \"width\": 884, \"height\": 379}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-11-717798-v1/fig-013.webp\", \"caption\": \"\", \"page\": 19, \"index\": 13, \"width\": 884, \"height\": 379}]"
motivation: 旨在探究认知老化是否普遍削弱大脑的预测处理机制，并厘清不同预测子系统在老化过程中的演变规律。
method: 利用脑磁图记录年轻和老年组在执行听觉局部-全局范式时的脑电活动，并采用源空间重建和网络分解技术分析预测处理过程。
result: 研究发现老化增强了感觉预测误差网络，但削弱了与注意重定向和上下文模式处理相关的网络，且整体多元递归水平在老化中得以保持。
conclusion: 大脑在衰老过程中并非简单的预测能力下降，而是通过网络重构重新分配了预测资源，强化了感觉层面的处理并削弱了高认知要求的机制。
---

## 摘要
认知老化通常与大脑预测机制的逐渐减弱相关。这一观点得到了数十年电生理学研究的支持，这些研究报告了老年人中失配响应（mismatch responses）的减弱。然而，现有文献仍存在不一致之处，表明衰老可能并不会一致地削弱预测加工。一种可能性是，多个预测子系统在同时运行，但很少被区分开来。在本研究中，我们通过分离 77 名执行听觉局部-全局范式（auditory local-global paradigm）的青年人和老年人的源重建脑磁图（MEG）数据中预测加工背后的全脑网络，探讨了这一问题。网络分解揭示了三个在时间上重叠且具有不同功能特征的预测子系统。衰老对这些网络产生了选择性影响。在连接听觉皮层与内侧扣带回区域的网络中，感官预测误差响应有所增强；而在老年人中，与注意力重定向和上下文模式加工相关的响应则有所减弱。这些网络间的多元递归（multivariate recurrency）水平在衰老过程中得以保留，而两组受试者中，感官违背（sensory violations）的加工相对于上下文违背诱发了更多的递归和更少的发散。这些发现挑战了预测加工随年龄增长而单纯下降的流行观点。相反，衰老在不同的神经系统中重新分配了预测资源，增强了基于感官的过程，同时削弱了对认知要求更高的预测机制。

## Abstract
Cognitive aging is widely associated with a progressive weakening of predictive brain mechanisms. This view is supported by decades of electrophysiological studies reporting attenuated mismatch responses in older adults. Yet the literature remains inconsistent, suggesting that aging may not uniformly attenuate predictive processing. One possibility is that multiple predictive subsystems operate concurrently but have rarely been disentangled. Here we address this question by separating whole-brain networks underlying predictive processing in source-reconstructed magnetoencephalography (MEG) data from 77 younger and older adults performing the auditory local-global paradigm. Network decomposition revealed three temporally overlapping predictive subsystems with distinct functional profiles. Aging exerted selective effects across these networks. Sensory prediction error responses were enhanced within a network linking auditory cortices with medial cingulate regions, whereas responses associated with reorientation of attention and contextual pattern processing were attenuated in older adults. The level of multivariate recurrency across these networks was preserved with aging, while the processing of sensory violations induced more recurrency and less divergence relative to contextual violations in both groups. These findings challenge the prevailing view that predictive processing simply declines with age. Instead, aging redistributes predictive resources across distinct neural systems, amplifying sensory-based processes while weakening more cognitively demanding predictive mechanisms.

---

## 论文详细总结（自动生成）

这篇论文题为《网络重构维持了老龄化大脑中的预测误差信号传导》（Network reconfiguration preserves prediction error signalling in the aging brain），发表于 2026 年（预印本标注日期）。以下是对该论文的结构化深入总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：认知老化是否普遍且一致地削弱了大脑的“预测编码”（Predictive Coding）机制？
*   **研究背景**：传统观点认为，随着年龄增长，大脑对感官违背的预测误差信号（如失配负波 MMN）会逐渐减弱。然而，现有研究结果存在矛盾，且大多局限于头皮电位分析，未能区分同时运行的多个预测子系统。
*   **研究动机**：通过全脑网络分解技术，探究衰老如何差异化地影响“局部感官预测”与“全局上下文模式预测”，并分析这些过程背后的神经动力学变化。

### 2. 论文提出的方法论
*   **核心思想**：采用 **BROAD-NESS**（基于源分离的宽带网络估计）框架，从源重建的脑磁图（MEG）数据中分离出正交的全脑功能网络。
*   **关键技术细节**：
    *   **源重建**：利用单层球壳前向模型和线性约束最小方差（LCMV）波束形成器（Beamforming），将 MEG 信号映射到 3,559 个 8mm 的脑体素上。
    *   **网络分解（PCA）**：对体素时间序列进行主成分分析（PCA），提取解释方差最大的前三个主网络。
    *   **动力学分析**：将提取的网络时间序列嵌入低维**相空间（Phase Space）**，并应用**递归量化分析（RQA）**。通过计算递归率、确定性、熵和发散度等指标，量化脑网络状态的稳定性和复杂性。
    *   **空间梯度嵌入**：利用 k-means 聚类分析体素在不同主成分上的权重，识别出功能重叠或特异的解剖区域。

### 3. 实验设计
*   **受试者与场景**：
    *   **样本**：77 名健康受试者，分为青年组（37 人，18-25 岁）和老年组（40 人，60-81 岁）。
    *   **范式**：听觉“局部-全局”范式（Auditory Local-Global Paradigm）。通过改变序列中第五个音调的频率（局部违背）或改变序列出现的概率（全局违背）来诱发不同层级的预测误差。
*   **对比方法与 Benchmark**：
    *   对比青年组与老年组的差异。
    *   对比局部违背（感官层级）与全局违背（认知层级）的神经响应。
    *   将网络分析结果与传统的事件相关场（ERF）响应（如 MMN, P3a, RON）进行关联。

### 4. 资源与算力
*   **算力说明**：论文未明确提及具体的 GPU 型号、数量或训练时长。
*   **工具链**：使用了 MATLAB 环境下的 OSL (Oxford Centre for Human Brain Activity Software Library)、SPM12、FieldTrip 和 FSL 等神经科学专用工具包。

### 5. 实验数量与充分性
*   **实验规模**：N=77 的样本量在 MEG 研究中具有较好的统计效力。
*   **充分性验证**：
    *   进行了**有效维度（Effective Dimensionality, ED）**分析，验证了网络参与的广度。
    *   实施了**稳健性检查**：分别在全样本平均数据和组别/条件分离的数据上运行 PCA，结果保持高度一致。
    *   采用了基于聚类的置换检验（Cluster-based Permutation Tests）来控制多重比较的错误率。
*   **客观性**：实验设计考虑了老年人的听力补偿，并使用了非参数统计方法，确保了结果的客观性。

### 6. 主要结论与发现
*   **衰老的选择性影响**：衰老并非简单地削弱所有预测过程。在连接听觉皮层与内侧扣带回的网络中，老年人的**感官预测误差响应（MMN/P3a）反而增强**。
*   **高阶功能减弱**：老年人在**注意重定向（RON）**和**全局模式处理**相关的网络响应上表现出明显的衰减。
*   **动力学特征**：
    *   局部违背诱发了更具递归性（Recurrent）和确定性的网络轨迹。
    *   全局违背则表现出更高的发散性（Divergence）和探索性动态。
    *   这些动力学特征在不同年龄组间基本保持稳定。
*   **网络重构**：老年人表现出更强的双侧听觉皮层招募（符合 HAROLD 模型），这被视为一种维持感官处理的补偿性重构。

### 7. 优点
*   **视角新颖**：挑战了“老化即衰退”的传统叙事，提出了资源重新分配的观点。
*   **技术先进**：BROAD-NESS 框架能够同时处理空间、时间和动力学维度，比传统的单传感器分析更深入。
*   **多维度量化**：结合了线性（PCA）与非线性（RQA）分析方法，提供了关于大脑如何随时间切换状态的丰富信息。

### 8. 不足与局限
*   **横断研究限制**：由于是横断研究而非纵向追踪，无法完全排除代际差异（Cohort effects）对结果的影响。
*   **适应性混淆（SSA）**：老年人早期响应的增强可能部分归因于“刺激特异性适应”能力的下降，而非纯粹的预测增强，这一点在文中虽有讨论但难以完全剥离。
*   **频率信息缺失**：研究主要关注宽带信号，未深入探讨特定频段（如 Gamma 或 Beta 振荡）在预测编码中的角色。

（完）
