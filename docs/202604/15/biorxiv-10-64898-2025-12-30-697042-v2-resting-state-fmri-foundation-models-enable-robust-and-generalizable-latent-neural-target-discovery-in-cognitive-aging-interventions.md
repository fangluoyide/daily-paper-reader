---
title: Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions
title_zh: 静息态 fMRI 基础模型助力认知老化干预中鲁棒且可泛化的潜在神经靶点发现
authors: "Zhou, X., Ai, M., Adeli, E., Zhang, Y., Liu, Y. M., Vankee-Lin, F."
date: 2026-04-15
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.30.697042v2.full.pdf"
tags: ["query:cog-eld"]
score: 8.0
evidence: 认知老化干预的fMRI基础模型
tldr: 本研究针对认知老化干预效果的个体差异，评估了基于大规模数据预训练的静息态fMRI基础模型。通过分析轻度认知障碍患者的随机对照试验数据，研究发现基础模型在预测情景记忆变化方面优于传统方法，并能识别出跨研究一致的潜在神经模式，为认知老化研究中的精准神经靶点发现奠定了基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-001.webp\", \"caption\": \"Figure 4. Three-condition framework for identifying robust and generalizable neural patterns in 687 cognitive aging intervention studies. rsfMRI FMs are applied to local intervention studies 688 characterized by small sample sizes and heterogeneous responses. Under Condition 1 (rich 689 spatiotemporal representation), FMs extract latent neural embeddings from BOLD time series that 690 capture distributed dynamics beyond predefined features, enabling robust representation learning 691 and improved prediction of outcomes. Under Condition 2 (behavioral relevance), these 692 embeddings are linked to behavioral metrics through multivariate analysis, yielding latent 693 variables that characterize individual differences in intervention response. These latent 694 representations further support the identification of interpretable neural patterns. Under Condition 695 3 (cross-study robustness), neural patterns are evaluated across independent studies to identify 696 shared structures, distinguish arm-specific effects, and enable cross-study alignment. Together, 697 these steps define an intervention representation atlas that captures both shared and study-698 specific neural signatures. Alternative approaches, including cross-dataset transfer, embedding 699 alignment, and external validation, may provide complementary assessments of generalizability. 700\", \"page\": 18, \"index\": 1, \"width\": 970, \"height\": 334}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-002.webp\", \"caption\": \"Figure 5. Study datasets and implementation of rsfMRI FMs and comparison methods. (a) The 704 ACT and CogTE studies serve as independent intervention cohorts for downstream evaluation 705 and assessment of model generalizability across intervention paradigms and study designs. (b) 706 Domain-adaptive finetuning of BrainLM using the ADNI dataset via LoRA. Supervised finetuning 707 is performed to incorporate aging- and pathology-related brain patterns, yielding the adapted 708 BrainLM-ADNI model that is subsequently used as a frozen feature extractor in all downstream 709 intervention analyses. (c) Linear probing strategy for deploying pretrained rsfMRI FMs in 710 longitudinal intervention studies. The rsfMRI data collected at baseline (T1) and post-intervention 711 (T2) are processed independently through a frozen FM with shared weights, and CLS-token 712 embeddings from each timepoint are concatenated to explicitly encode longitudinal neural change 713 for downstream inference of EM outcomes. (d) Architectures of conventional comparison models. 714 FC features derived from rsfMRI data at T1 and T2 are used to train an SVM, an MLP, and a 715 dual-stream GCN that explicitly models longitudinal brain network changes. NOTE: rsfMRI, 716 resting-state functional magnetic resonance imaging; FM, foundation model; ACT, Aerobic 717 exercise and Cognitive Training study; MLA, mental leisure activity; CogTE, Cognitive Training 718 and Exercise study; ADNI, Alzheimer’s Disease Neuroimaging Initiative; EM, episodic memory; 719 FC, functional connectivity; T1/T2, baseline/post-intervention timepoints; SVM, support vector 720 machine; MLP, multilayer perceptron; GCN, graph convolutional network; LoRA, low-rank 721 adaptation; AD, Alzheimer’s Disease; HC, healthy control. 722\", \"page\": 19, \"index\": 2, \"width\": 972, \"height\": 469}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-003.webp\", \"caption\": \"Figure 3. PLS-derived embedding-brain associations and cross-study spatial patterns. (a-b) ACT 673 (a) and CogTE (b) PLS results. Top: T1; bottom: T2. Left: relationship between embedding scores 674 and brain scores. Middle: group differences in brain scores. Right: group differences in 675 embedding scores. Points are colored by responder status (stable vs. decline). Reported 676 statistics correspond to two-sample t-tests on subject-level PLS scores. For each study and 677 timepoint, the component shown represents the dominant embedding-brain association capturing 678 group differentiation. (c) Cross-study correlations of PLS brain loading patterns across increasing 679 thresholds of top-weighted regions (ranked by absolute loading). (d-e) Cross-study average 680 spatial distribution of top-weighted PLS loadings at baseline (T1; left) and post-intervention (T2; 681 right), shown in standard anatomical views and illustrating shared spatial organization of latent 682 neural patterns across the two intervention studies. 683\", \"page\": 17, \"index\": 3, \"width\": 978, \"height\": 514}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-004.webp\", \"caption\": \"Figure 2. Evaluation of rsfMRI FMs for classifying intervention-related episodic memory 652 response. (a) Benchmark comparison of classification performance between rsfMRI FMs 653 (BrainLM, BrainJEPA) and conventional ML and DL approaches (SVM, MLP, GCN) across two 654 independent intervention cohorts (CogTE and ACT). Models are trained to classify participants as 655 episodic memory responders vs. non-responders, based on pre-post changes in EM, using 656 baseline (T1) and post-intervention (T2) rsfMRI data. ACC and F1-score are reported as mean ± 657 standard deviation across stratified cross-validation folds. (b) Performance of the BrainLM-ADNI 658 under different timepoint combinations. Classification results for T1 + T2, T1-only, and T2 − T1 659 input settings are shown for CogTE and ACT datasets (mean ± standard deviation across cross-660 validation folds). (c) Robustness of the adapted FM to common neuroimaging confounders in the 661 multi-site ACT dataset. Classification performance of BrainLM-ADNI is shown for original data, 662 data after site harmonization, and data after both site harmonization and head-motion regression. 663 (d) Classification performance of BrainLM-ADNI stratified by intervention arm in both CogTE and 664 ACT studies. Chi-square tests indicate no significant association between intervention 665 assignment and classification correctness. NOTE: rsfMRI, resting-state functional magnetic 666 resonance imaging; FM, foundation model; ML, machine learning; DL, deep learning; SVM, 667 support vector machine; MLP, multilayer perceptron; GCN, graph convolutional network; ACT, 668 Aerobic exercise and Cognitive Training study; CogTE, Cognitive Training and Exercise study; 669 ADNI, Alzheimer’s Disease Neuroimaging Initiative; ACC, accuracy. 670\", \"page\": 16, \"index\": 4, \"width\": 899, \"height\": 516}]"
motivation: 传统rsfMRI分析方法难以捕捉认知老化干预中复杂的个体差异和纵向变化，限制了对干预反应神经机制的理解。
method: 系统评估了rsfMRI基础模型在两个独立随机对照试验中的表现，并结合外部阿尔茨海默病队列进行临床适应性调整。
result: "基础模型在预测情景记忆改善方面的准确率高达82%，显著优于传统机器学习方法，且对混杂因素具有极强的鲁棒性。"
conclusion: rsfMRI基础模型能够稳健地提取与干预反应相关的潜在神经模式，为认知老化干预的精准医疗提供了强有力的技术支撑。
---

## 摘要
针对认知老化的干预效果在个体间存在显著差异，这在很大程度上归因于老化相关共病的异质性。因此，有必要鲁棒地识别干预反应背后的神经模式，并测试其在异质队列中的可泛化性。静息态功能磁共振成像（rsfMRI）提供了一条潜在途径，但传统方法依赖预定义的汇总特征，在捕捉个体内的纵向变化和个体间的差异方面能力有限，特别是在样本量较小且具有异质性的研究中。近期在大型观测队列上预训练的 rsfMRI 基础模型通过从时间序列信号中学习可迁移的时空表征，提供了一个极具前景的替代方案。然而，这些模型在局部干预场景中的有效性和可泛化性尚不明确。在本研究中，我们利用两项针对轻度认知障碍老年人的独立随机对照试验数据，系统评估了 rsfMRI 基础模型，测试其能否鲁棒地提取纵向大脑表征，从而跨试验预测干预后情景记忆的变化。结果显示，基础模型在两项试验中的表现均优于传统的机器学习和深度学习方法。利用外部阿尔茨海默病队列进行临床信息适配，进一步提高了模型性能以及对混杂因素（即头动、站点和干预组别）的鲁棒性，准确率高达 82%。对基础模型嵌入进行多变量分解，识别出了与情景记忆变化相关的潜在神经模式；这些模式在基线时具有跨研究的一致性，而在干预后则在空间分布上更加广泛。这些发现表明，rsfMRI 基础模型能够实现对连接纵向大脑动态与个体干预反应的潜在神经模式的鲁棒且可泛化的识别，为认知老化研究中精准驱动的神经靶点发现奠定了基础。

## Abstract
The benefits of interventions targeting cognitive aging vary substantially across individuals, largely owing to heterogeneity in aging-related comorbidities. It is necessary to robustly identify neural patterns underlying intervention response and test their generalizability across heterogeneous cohorts. Resting-state functional MRI (rsfMRI) offers a potential pathway, but relying on predefined summary features with conventional methods has limited capacity to capture both within-individual longitudinal variation and between-individual differences, particularly in small and heterogeneous studies. Recent rsfMRI foundation models pretrained on large observational cohorts present a promising alternative by learning transferable spatiotemporal representations from time-series signals. Yet their validity and generalizability in local intervention settings remain unclear. Here, we systematically evaluated rsfMRI foundation models using data from two independent randomized controlled trials of older adults with mild cognitive impairment, testing whether these models can robustly extract longitudinal brain representations that predict post-intervention changes in episodic memory across trials. Foundation models outperformed conventional machine learning and deep learning approaches across both trials. Clinically informed adaptation using an external Alzheimer's disease cohort further improved performance and robustness to confounders (i.e., head motion, site, and intervention arm), with accuracy up to 82%. Multivariate decomposition of foundation model embeddings identified latent neural patterns associated with episodic memory change with cross-study consistency at baseline that became more spatially distributed at post-intervention. These findings show that rsfMRI foundation models can enable robust and generalizable identification of latent neural patterns linking longitudinal brain dynamics to individual intervention response, laying the foundation for precision-driven neural target discovery in cognitive aging research.

---

## 论文详细总结（自动生成）

这是一份关于论文《Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions》的结构化深入总结：

### 1. 核心问题与研究背景
*   **研究动机**：针对认知老化的干预措施（如运动、认知训练）在个体间表现出极大的效果差异。这种异质性导致许多临床试验结果不一致或失败。
*   **核心挑战**：传统的静息态 fMRI（rsfMRI）分析依赖于预定义的感兴趣区（ROI）或功能连接（FC）汇总特征。这些方法往往会丢失原始信号中的复杂时空动态，且在样本量较小、异质性强的临床研究中容易出现过拟合或敏感性不足的问题。
*   **研究目标**：验证在大规模数据上预训练的“基础模型”（Foundation Models, FMs）是否能比传统方法更有效地提取大脑表征，从而鲁棒地预测个体对干预的反应，并识别跨研究可泛化的潜在神经模式。

### 2. 方法论
*   **核心思想**：利用预训练的 Transformer 架构直接处理原始 rsfMRI 时间序列，学习高阶、非线性的潜在表征，而非依赖静态的连接矩阵。
*   **关键技术细节**：
    *   **基础模型选择**：评估了两种模型：**BrainLM**（基于自回归序列建模，类似语言模型）和 **BrainJEPA**（基于联合嵌入预测架构，强调时空一致性）。
    *   **临床领域适配（Domain Adaptation）**：使用 ADNI 数据集（阿尔茨海默病 vs 健康对照）对 BrainLM 进行微调（采用 **LoRA** 轻量化微调技术），使其捕捉与老化和病理相关的神经变异。
    *   **纵向建模流程**：采用双流架构，分别提取基线（T1）和干预后（T2）的潜在嵌入（Embeddings），拼接后输入轻量级分类器预测情景记忆（EM）的变化。
    *   **潜在模式识别**：使用**偏最小二乘法（PLS）**将高维的基础模型嵌入与全脑低频振幅（ALFF）图关联，从而将“黑盒”表征转化为可解释的空间神经模式。

### 3. 实验设计
*   **数据集**：
    *   **ACT 研究**：多中心随机对照试验（RCT），包含运动、认知训练及其组合，样本异质性高（N=105）。
    *   **CogTE 研究**：单中心 RCT，侧重于认知训练（N=41）。
    *   **ADNI**：用于模型微调的外部独立老化队列。
*   **Benchmark（对比方法）**：
    *   **传统机器学习**：支持向量机（SVM）配合功能连接（FC）特征。
    *   **深度学习**：多层感知机（MLP）和图卷积网络（GCN）。
*   **实验场景**：分类“响应者”（记忆力维持或提升）与“非响应者”（记忆力下降）。

### 4. 资源与算力
*   论文中**未明确说明**具体的 GPU 型号、数量或训练总时长。
*   但文中提到使用了 **LoRA（Low-Rank Adaptation）** 模块，这是一种参数高效的微调方法，通常旨在降低对显存和计算资源的需求，使得在较小规模的算力下也能适配大型基础模型。

### 5. 实验数量与充分性
*   **实验组数**：进行了多维度的评估，包括：
    1.  不同基础模型（BrainLM vs BrainJEPA）的对比。
    2.  基础模型与三种传统/深度学习基准模型的性能对比。
    3.  不同时间点组合（仅 T1、仅 T2、T1+T2）的消融实验。
    4.  针对站点效应、头动伪影、干预组别等混杂因素的鲁棒性测试。
    5.  跨两个独立临床试验（ACT 和 CogTE）的一致性验证。
*   **充分性评价**：实验设计非常充分且严谨。通过跨研究验证和混杂因素控制，证明了结果并非特定于某一数据集或噪声干扰，具有较高的客观性和公平性。

### 6. 主要结论与发现
*   **性能优越性**：基础模型（尤其是 BrainLM）在预测干预反应方面显著优于所有传统方法，在 ACT 试验中准确率提升显著，最高达到 **82%**。
*   **微调的必要性**：经过 ADNI 临床数据微调后的模型（BrainLM-ADNI）表现出更强的泛化能力和对老化相关信号的敏感度。
*   **鲁棒性**：模型对头动、扫描站点和干预方式表现出极强的鲁棒性，证明其捕捉的是核心神经生物学信号。
*   **神经模式发现**：识别出基线时跨研究高度一致的潜在神经模式（主要涉及默认模式网络 DMN、视觉网络和额顶网络），这些模式在干预后变得更加空间弥散，反映了复杂的神经塑性变化。

### 7. 优点
*   **突破小样本瓶颈**：证明了在大规模数据上预训练的模型可以有效迁移到样本量仅为几十人的局部临床研究中。
*   **端到端表征学习**：避免了人工定义特征带来的信息损失，能够捕捉到传统 FC 方法无法发现的细粒度时空动态。
*   **临床实用性**：提供了一个从原始数据到个体化预测，再到神经靶点发现的完整框架。

### 8. 不足与局限
*   **模型选择局限**：虽然测试了两种 FM，但随着领域发展，更多更新的架构（如多模态基础模型）尚未被纳入对比。
*   **生物学解释的间接性**：尽管使用了 PLS 进行映射，但 Transformer 内部表征的直接生物学含义仍具有一定的“黑盒”属性。
*   **认知领域局限**：研究主要集中在情景记忆（Episodic Memory），对于其他认知维度（如执行功能、处理速度）的预测效力尚待验证。

（完）
