---
title: "Neonatal sensory networks at birth predict cognitive, language, and motor outcomes at 18 months"
title_zh: 出生时的新生儿感觉网络可预测18个月时的认知、语言和运动表现
authors: "Zou, M., Bokde, A."
date: 2026-04-05
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.04.716445v1.full.pdf"
tags: ["query:q1"]
score: 8.0
evidence: 预测婴儿的认知发育结果
tldr: 本研究利用402名新生儿的脑连接数据，探讨了出生时脑活动模式与18个月大时认知、语言及运动发育的关系。研究提出了一种受ROI约束的连接组预测模型（CPM），通过筛选高连接度区域提升预测鲁棒性。结果发现，视觉和听觉等早期感觉网络是预测发育结局的关键生物标志物，且足月儿与早产儿的预测特征存在显著差异。该研究为早期神经发育预测提供了新方法和重要证据。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-001.webp\", \"caption\": \"Figure 7 Negative networks: receptive language and gross motor predictive anatomy(term cohort). (A,C) Connections plotted as the number of edges within and between each pair of canonical networks for receptive language score and gross motor score respectively(left to right). (B,D) High-degree ROIs for the same models. Only ROIs with a degree ≥ one-sixth of the highest ROI are displayed; node size is proportional to degree.\", \"page\": 38, \"index\": 1, \"width\": 1713, \"height\": 1307}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-002.webp\", \"caption\": \"Table 2 Statistics of permutation and independent validation\", \"page\": 42, \"index\": 2, \"width\": 1823, \"height\": 1959}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-003.webp\", \"caption\": \"Figure 2. Cohort-specific predictive networks for cognition.\", \"page\": 33, \"index\": 3, \"width\": 1748, \"height\": 299}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-004.webp\", \"caption\": \"Figure 4. Predictive networks for language across cohorts and subscales.\", \"page\": 35, \"index\": 4, \"width\": 1897, \"height\": 1855}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-005.webp\", \"caption\": \"Figure 9. Inter-/intra-hemispheric connectivity patterns in term and preterm cohorts.\", \"page\": 40, \"index\": 5, \"width\": 1721, \"height\": 215}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-006.webp\", \"caption\": \"Figure 1. ROI-constrained CPM pipeline with ROI-constrained feature selection and independent validation. (a) Stage-2 — ROI ranking: ROIs were sorted by iteratively removing the highest-degree ROI to define a high-to-low ROI degree order. No Stage-1 edges were carried forward as features; only the ROI order 𝑅 was passed to Stage 3. (b) Stage-3 — ROI-constrained CPM : For each ROI-set size (n = 1…|R|), edges that survived p<0.05 and connected to at least one of the top-n ROIs were selected via LOO to calculate prediction accuracy. SNR was also computed for each prefix n by dividing the summed occurrence counts of signal edges (occurred in ≥ 90% of LOO iterations) by those of noise edges (occurred in ≥ 90% of LOO iterations);(c) Stage-4 — SNR analysis: As progressively lower-degree ROIs were added, SNR steadily decreased(c2), mirroring the decline in predictive accuracy(c1). And SNR and prediction accuracy were strongly correlated (r = 0.96, p < 0.0001). We conducted a permutation test to confirm that the observed weighted average prediction performance (weighted by degree of each ROI) across all ROI-set sizes n exceeded chance; (d) Independent validation: For each ROI-set size (n = 1…|R|), validation subjects’ network strength—sums of signal edges incident on the top-n ROIs—were correlated with\", \"page\": 32, \"index\": 6, \"width\": 1891, \"height\": 263}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716445-v1/fig-007.webp\", \"caption\": \"Table 1 Research participants\", \"page\": 41, \"index\": 7, \"width\": 1588, \"height\": 1294}]"
motivation: 传统的全脑连接分析往往因包含低信噪比特征而难以稳定预测婴儿后期的认知发育。
method: 采用受ROI约束且基于区域度引导特征选择的连接组预测模型（CPM），分析了402名新生儿的脑功能连接与18个月Bayley-III评分的关系。
result: 模型成功预测了多项发育指标，发现足月儿的预测特征集中在视听交互，而早产儿则侧重于听觉与颞顶网络及跨半球连接。
conclusion: 早期感觉中心（尤其是视觉和听觉区域）是预测后期神经发育的重要生物标志物，且ROI约束的预测方法优于传统全连接组方法。
---

## 摘要
新生儿脑活动模式与后期认知发展之间的关系已成为发育神经科学的核心课题。解决这一问题需要全脑分析方法，以识别哪些大规模功能系统携带稳定且可推广的预测信号。然而，现有的大多数研究仍集中在特定的脑区或局部功能回路上，例如丘脑-皮层通路和以杏仁核为中心的情绪网络。虽然这些针对特定区域的研究提供了重要的见解，但它们在鲁棒性和跨样本泛化性方面存在固有的局限性。因此，关于哪些大规模功能系统能可靠地支持稳定且可推广的预测信号，目前仍缺乏系统性的证据。因此，克服传统全脑分析范式的方法学限制，已成为深入理解早期脑活动模式与后续认知发展关系的瓶颈。在本研究中，我们利用来自“发育中人类连接组项目”（developing Human Connectome Project，包含278名足月儿和124名早产儿）的402名婴儿数据，引入了一种受感兴趣区（ROI）约束的连接组预测模型（CPM）变体。该模型结合了基于ROI度（degree）引导的特征选择，用于预测18个月时的贝利婴幼儿发展量表第三版（Bayley-III）的认知、语言和运动表现。随着逐渐纳入度较低的区域，模型性能有所下降，这表明传统的全连接组CPM可能因纳入低信噪比（SNR）特征而掩盖了鲁棒的预测信号。我们的模型稳健地预测了18个月时的认知、语言和运动表现。研究发现了特定队列的连接模式：在足月儿中，主要的预测特征集中在视听交互，以及视觉和听觉网络与其他皮层区域之间的连接，且半球间与半球内连接的贡献比例大致相等；相比之下，在早产儿中，预测特征主要集中在涉及听觉和颞顶网络的连接中，其中半球间连接的数量约为半球内连接的两倍。全队列模型（足月儿+早产儿）反映了足月儿和早产儿相关连接模式的共同贡献。预测结果在贝利量表的综合得分和子量表得分上均具有泛化性，并得到了置换检验和留出验证的支持。这些发现表明，早期感觉枢纽（特别是视觉和听觉区域）是预测后期神经发育表现的有前景的早期生物标志物。此外，研究证明了受ROI约束的CPM可以揭示传统全连接组方法可能掩盖的有意义的预测信号。

## Abstract
The relationship between neonatal brain activity patterns and later cognitive development has become a central topic in developmental neuroscience. Addressing this question requires whole-brain analytical approaches capable of identifying which large-scale functional systems carry stable and generalizable predictive signals. However, most existing studies remain focused on specific brain regions or localized functional circuits, such as thalamocortical pathways and amygdala-centered emotional networks. While these region-specific investigations have provided important insights, they are inherently limited in terms of robustness and cross-sample generalizability. As a result, systematic evidence identifying which large-scale functional systems reliably support stable and generalizable predictive signals remains scarce. Overcoming the methodological constraints of conventional whole-brain analytical paradigms has therefore become a key bottleneck in advancing our understanding of how early brain activity patterns relate to subsequent cognitive development.

Here, using data from 402 infants in the developing Human Connectome Project (278 term-born; 124 preterm-born), we introduce a region-of-interest (ROI)-constrained variant of Connectome-Based Predictive Modeling (CPM) that incorporates ROI-degree-guided feature selection to predict 18-month Bayley-III cognitive, language, and motor outcomes. Model performance declined as progressively lower-degree regions were included, indicating that conventional whole-connectome CPM may obscure robust predictive signals by incorporating low signal-to-noise (SNR) features.

Our models robustly predicted cognitive, language, and motor outcomes at 18 months of age. Cohort-specific connectivity patterns emerged. In term-born infants, dominant predictive features were concentrated in visual-auditory interactions, as well as connections between visual and auditory networks and other cortical regions. Interhemispheric and intrahemispheric connections contributed in roughly equal proportions. In contrast, among preterm infants, predictive features were primarily concentrated in connectivity involving auditory and temporoparietal networks, with interhemispheric connections comprising approximately twice the number of intrahemispheric connections. The whole-cohort model (term + preterm) reflected the combined contributions of both term- and preterm-associated connectivity patterns.

Predictions generalized across Bayley composite and subscale scores and were supported by permutation testing and held-out validation. These findings identify early sensory hubs--particularly visual and auditory regions--as promising early biomarkers for later neurodevelopmental outcomes. Furthermore, they demonstrate that ROI-constrained CPM can reveal meaningful predictive signals that may be obscured by conventional connectome-wide approaches.

---

## 论文详细总结（自动生成）

以下是对论文《Neonatal sensory networks at birth predict cognitive, language, and motor outcomes at 18 months》的结构化深入总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
本研究探讨了**新生儿出生时的脑功能连接模式是否能预测其 18 个月大时的认知、语言和运动发育表现**。
*   **研究动机**：尽管已知早期脑发育对后期功能至关重要，但传统全脑连接分析（如 CPM）在预测婴儿发育时常面临“信噪比（SNR）低”的问题。全脑数万个连接中，许多是冗余或带有噪声的，这掩盖了真正的预测信号。
*   **核心意义**：研究旨在识别出哪些大规模功能系统（如感觉、运动或高级认知网络）携带最稳定的预测信号，并对比足月儿与早产儿在预测特征上的差异，为早期神经发育障碍的干预提供生物标志物。

### 2. 论文提出的方法论：ROI 约束的 CPM
研究提出了一种**受感兴趣区（ROI）约束的连接组预测模型（ROI-constrained CPM）**，其核心思想是通过“度（Degree）引导”的特征选择来提升模型性能。
*   **核心思想**：假设在功能连接网络中，连接度（Degree）较高的 ROI 包含更稳定的生物学信号。通过优先选择这些“枢纽”区域的连接，可以过滤掉低信噪比的特征。
*   **算法流程**：
    1.  **ROI 排序**：计算每个 ROI 在群体水平上的平均连接度，并按从高到低排序。
    2.  **迭代特征选择**：从度最高的 ROI 开始，逐步增加 ROI 的数量（n=1, 2...|R|）。对于每个规模的 ROI 集合，仅提取与这些 ROI 相关的连接（Edges）。
    3.  **模型训练与验证**：在每个 ROI 集合规模下，利用留一交叉验证（LOO）进行 CPM 预测，计算预测值与实际 Bayley-III 评分的相关性。
    4.  **SNR 分析**：通过计算“信号边”（在迭代中频繁出现的边）与“噪声边”的比值，量化不同 ROI 规模下的信噪比变化。

### 3. 实验设计
*   **数据集**：使用了**发育中人类连接组项目（dHCP）**的数据，包含 **402 名新生儿**（278 名足月儿，124 名早产儿）。
*   **评估指标（Label）**：18 个月时的贝利婴幼儿发展量表第三版（Bayley-III）评分，包括认知、语言（接受性/表达性）和运动（粗大/精细）五个维度。
*   **Benchmark 与对比**：
    *   对比了**传统全连接组 CPM**（即不进行 ROI 约束，使用全脑所有连接）。
    *   对比了**不同队列**（足月儿、早产儿、全队列）的预测表现。
    *   使用了**置换检验（Permutation Testing）**来验证预测结果是否显著优于随机水平。

### 4. 资源与算力
论文中**未明确说明**具体的硬件配置（如 GPU 型号、数量）或训练时长。由于该研究主要涉及静息态功能磁共振成像（rs-fMRI）的预处理和基于线性回归的 CPM 模型，此类计算通常在高性能计算集群（HPC）的 CPU 节点上完成，对实时算力的要求低于深度学习大模型。

### 5. 实验数量与充分性
*   **实验规模**：样本量（N=402）在新生儿神经影像研究中属于较大规模。
*   **实验设计充分性**：
    *   **多维度预测**：涵盖了认知、语言、运动等多个发育领域。
    *   **消融与验证**：通过逐步增加低度 ROI 观察模型性能下降，证明了高连接度区域的重要性。
    *   **独立验证**：除了内部交叉验证，还进行了置换检验以确保结果的客观性。
    *   **公平性**：分别对足月儿和早产儿建模，考虑了出生胎龄这一关键混杂因素。

### 6. 论文的主要结论与发现
*   **感觉网络是核心预测因子**：出生时的**视觉网络和听觉网络**是预测 18 个月发育结局的最强生物标志物。
*   **队列差异显著**：
    *   **足月儿**：预测特征集中在视听交互，半球内和半球间连接贡献均衡。
    *   **早产儿**：预测特征侧重于听觉和颞顶网络，且**半球间连接（Interhemispheric）**的数量是半球内的两倍，显示出早产儿独特的代偿或发育路径。
*   **方法学优势**：ROI 约束模型显著优于全连接组模型。随着低度 ROI 的加入，模型信噪比（SNR）和预测准确率同步下降，证实了全脑分析中存在大量干扰噪声。

### 7. 优点（亮点）
*   **创新性方法**：引入 ROI 约束机制解决了婴儿影像数据噪声大的痛点，提升了 CPM 的鲁棒性。
*   **发育生物学洞察**：明确了“感觉优先”的预测模式，即早期感觉系统的整合水平决定了后期高级认知功能的基础。
*   **临床相关性**：为早产儿等高风险群体提供了可量化的早期筛查工具。

### 8. 不足与局限
*   **预测时效性**：仅预测了 18 个月时的表现，更长期的（如学龄期）认知结局是否仍由这些感觉网络决定尚不清楚。
*   **因果关系**：作为相关性研究，无法确定感觉网络的发育异常是导致认知落后的原因，还是某种更深层神经发育障碍的共同表现。
*   **外部验证**：虽然在 dHCP 内部做了验证，但仍需在其他独立的新生儿队列（如不同扫描仪、不同种族）中验证模型的泛化性。

（完）
