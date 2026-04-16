---
title: Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions
title_zh: 静息态 fMRI 基础模型助力认知老化干预中鲁棒且可泛化的潜在神经靶点发现
authors: "Zhou, X., Ai, M., Adeli, E., Zhang, Y., Liu, Y. M., Vankee-Lin, F."
date: 2026-04-15
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.30.697042v2.full.pdf"
tags: ["query:cog-eld"]
score: 8.0
evidence: 认知老化干预中的神经靶点发现
tldr: 本研究针对认知老化干预效果的个体差异，评估了基于大规模数据预训练的静息态fMRI基础模型。通过分析轻度认知障碍患者的随机对照试验数据，研究发现基础模型在预测情景记忆变化方面优于传统方法，并能识别出跨研究一致的潜在神经模式，为认知老化研究中的精准神经靶点发现奠定了基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-001.webp\", \"caption\": \"Figure 4. Three-condition framework for identifying robust and generalizable neural patterns in 687 cognitive aging intervention studies. rsfMRI FMs are applied to local intervention studies 688 characterized by small sample sizes and heterogeneous responses. Under Condition 1 (rich 689 spatiotemporal representation), FMs extract latent neural embeddings from BOLD time series that 690 capture distributed dynamics beyond predefined features, enabling robust representation learning 691 and improved prediction of outcomes. Under Condition 2 (behavioral relevance), these 692 embeddings are linked to behavioral metrics through multivariate analysis, yielding latent 693 variables that characterize individual differences in intervention response. These latent 694 representations further support the identification of interpretable neural patterns. Under Condition 695 3 (cross-study robustness), neural patterns are evaluated across independent studies to identify 696 shared structures, distinguish arm-specific effects, and enable cross-study alignment. Together, 697 these steps define an intervention representation atlas that captures both shared and study-698 specific neural signatures. Alternative approaches, including cross-dataset transfer, embedding 699 alignment, and external validation, may provide complementary assessments of generalizability. 700\", \"page\": 18, \"index\": 1, \"width\": 970, \"height\": 334}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-002.webp\", \"caption\": \"Figure 5. Study datasets and implementation of rsfMRI FMs and comparison methods. (a) The 704 ACT and CogTE studies serve as independent intervention cohorts for downstream evaluation 705 and assessment of model generalizability across intervention paradigms and study designs. (b) 706 Domain-adaptive finetuning of BrainLM using the ADNI dataset via LoRA. Supervised finetuning 707 is performed to incorporate aging- and pathology-related brain patterns, yielding the adapted 708 BrainLM-ADNI model that is subsequently used as a frozen feature extractor in all downstream 709 intervention analyses. (c) Linear probing strategy for deploying pretrained rsfMRI FMs in 710 longitudinal intervention studies. The rsfMRI data collected at baseline (T1) and post-intervention 711 (T2) are processed independently through a frozen FM with shared weights, and CLS-token 712 embeddings from each timepoint are concatenated to explicitly encode longitudinal neural change 713 for downstream inference of EM outcomes. (d) Architectures of conventional comparison models. 714 FC features derived from rsfMRI data at T1 and T2 are used to train an SVM, an MLP, and a 715 dual-stream GCN that explicitly models longitudinal brain network changes. NOTE: rsfMRI, 716 resting-state functional magnetic resonance imaging; FM, foundation model; ACT, Aerobic 717 exercise and Cognitive Training study; MLA, mental leisure activity; CogTE, Cognitive Training 718 and Exercise study; ADNI, Alzheimer’s Disease Neuroimaging Initiative; EM, episodic memory; 719 FC, functional connectivity; T1/T2, baseline/post-intervention timepoints; SVM, support vector 720 machine; MLP, multilayer perceptron; GCN, graph convolutional network; LoRA, low-rank 721 adaptation; AD, Alzheimer’s Disease; HC, healthy control. 722\", \"page\": 19, \"index\": 2, \"width\": 972, \"height\": 469}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-003.webp\", \"caption\": \"Figure 3. PLS-derived embedding-brain associations and cross-study spatial patterns. (a-b) ACT 673 (a) and CogTE (b) PLS results. Top: T1; bottom: T2. Left: relationship between embedding scores 674 and brain scores. Middle: group differences in brain scores. Right: group differences in 675 embedding scores. Points are colored by responder status (stable vs. decline). Reported 676 statistics correspond to two-sample t-tests on subject-level PLS scores. For each study and 677 timepoint, the component shown represents the dominant embedding-brain association capturing 678 group differentiation. (c) Cross-study correlations of PLS brain loading patterns across increasing 679 thresholds of top-weighted regions (ranked by absolute loading). (d-e) Cross-study average 680 spatial distribution of top-weighted PLS loadings at baseline (T1; left) and post-intervention (T2; 681 right), shown in standard anatomical views and illustrating shared spatial organization of latent 682 neural patterns across the two intervention studies. 683\", \"page\": 17, \"index\": 3, \"width\": 978, \"height\": 514}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-004.webp\", \"caption\": \"Figure 2. Evaluation of rsfMRI FMs for classifying intervention-related episodic memory 652 response. (a) Benchmark comparison of classification performance between rsfMRI FMs 653 (BrainLM, BrainJEPA) and conventional ML and DL approaches (SVM, MLP, GCN) across two 654 independent intervention cohorts (CogTE and ACT). Models are trained to classify participants as 655 episodic memory responders vs. non-responders, based on pre-post changes in EM, using 656 baseline (T1) and post-intervention (T2) rsfMRI data. ACC and F1-score are reported as mean ± 657 standard deviation across stratified cross-validation folds. (b) Performance of the BrainLM-ADNI 658 under different timepoint combinations. Classification results for T1 + T2, T1-only, and T2 − T1 659 input settings are shown for CogTE and ACT datasets (mean ± standard deviation across cross-660 validation folds). (c) Robustness of the adapted FM to common neuroimaging confounders in the 661 multi-site ACT dataset. Classification performance of BrainLM-ADNI is shown for original data, 662 data after site harmonization, and data after both site harmonization and head-motion regression. 663 (d) Classification performance of BrainLM-ADNI stratified by intervention arm in both CogTE and 664 ACT studies. Chi-square tests indicate no significant association between intervention 665 assignment and classification correctness. NOTE: rsfMRI, resting-state functional magnetic 666 resonance imaging; FM, foundation model; ML, machine learning; DL, deep learning; SVM, 667 support vector machine; MLP, multilayer perceptron; GCN, graph convolutional network; ACT, 668 Aerobic exercise and Cognitive Training study; CogTE, Cognitive Training and Exercise study; 669 ADNI, Alzheimer’s Disease Neuroimaging Initiative; ACC, accuracy. 670\", \"page\": 16, \"index\": 4, \"width\": 899, \"height\": 516}]"
motivation: 传统rsfMRI分析方法难以捕捉认知老化干预中复杂的个体差异和纵向变化，限制了对干预反应神经机制的理解。
method: 系统评估了rsfMRI基础模型在两个独立随机对照试验中的表现，并结合外部阿尔茨海默病队列进行临床适应性调整。
result: "基础模型在预测情景记忆改善方面的准确率高达82%，显著优于传统机器学习方法，且对混杂因素具有更强的鲁棒性。"
conclusion: rsfMRI基础模型能够稳健地提取与干预反应相关的潜在神经模式，为认知老化干预的精准医疗提供了强有力的工具。
---

## 摘要
针对认知老化的干预效果在个体间存在显著差异，这在很大程度上归因于老化相关共病的异质性。因此，有必要鲁棒地识别干预反应背后的神经模式，并测试其在异质队列中的可泛化性。静息态功能磁共振成像（rsfMRI）提供了一条潜在途径，但传统方法依赖预定义的汇总特征，在捕捉个体内的纵向变化和个体间的差异方面能力有限，特别是在样本量较小且具有异质性的研究中。近期在大型观测队列上预训练的 rsfMRI 基础模型通过从时间序列信号中学习可迁移的时空表征，提供了一个极具前景的替代方案。然而，这些模型在局部干预场景中的有效性和可泛化性尚不明确。在本研究中，我们利用两项针对轻度认知障碍老年人的独立随机对照试验数据，系统评估了 rsfMRI 基础模型，测试其能否鲁棒地提取纵向大脑表征，从而跨试验预测干预后情景记忆的变化。结果显示，基础模型在两项试验中的表现均优于传统的机器学习和深度学习方法。利用外部阿尔茨海默病队列进行临床信息适配，进一步提高了模型性能以及对混杂因素（即头动、站点和干预组别）的鲁棒性，准确率高达 82%。对基础模型嵌入进行多变量分解，识别出了与情景记忆变化相关的潜在神经模式；这些模式在基线时具有跨研究的一致性，而在干预后则在空间分布上更加广泛。这些发现表明，rsfMRI 基础模型能够实现对连接纵向大脑动态与个体干预反应的潜在神经模式的鲁棒且可泛化的识别，为认知老化研究中精准驱动的神经靶点发现奠定了基础。

## Abstract
The benefits of interventions targeting cognitive aging vary substantially across individuals, largely owing to heterogeneity in aging-related comorbidities. It is necessary to robustly identify neural patterns underlying intervention response and test their generalizability across heterogeneous cohorts. Resting-state functional MRI (rsfMRI) offers a potential pathway, but relying on predefined summary features with conventional methods has limited capacity to capture both within-individual longitudinal variation and between-individual differences, particularly in small and heterogeneous studies. Recent rsfMRI foundation models pretrained on large observational cohorts present a promising alternative by learning transferable spatiotemporal representations from time-series signals. Yet their validity and generalizability in local intervention settings remain unclear. Here, we systematically evaluated rsfMRI foundation models using data from two independent randomized controlled trials of older adults with mild cognitive impairment, testing whether these models can robustly extract longitudinal brain representations that predict post-intervention changes in episodic memory across trials. Foundation models outperformed conventional machine learning and deep learning approaches across both trials. Clinically informed adaptation using an external Alzheimer's disease cohort further improved performance and robustness to confounders (i.e., head motion, site, and intervention arm), with accuracy up to 82%. Multivariate decomposition of foundation model embeddings identified latent neural patterns associated with episodic memory change with cross-study consistency at baseline that became more spatially distributed at post-intervention. These findings show that rsfMRI foundation models can enable robust and generalizable identification of latent neural patterns linking longitudinal brain dynamics to individual intervention response, laying the foundation for precision-driven neural target discovery in cognitive aging research.

---

## 论文详细总结（自动生成）

这是一份关于论文《Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions》的结构化深入分析报告：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：针对认知老化的干预措施（如运动、认知训练）在个体间表现出极大的效果差异。传统的静息态 fMRI（rsfMRI）分析方法依赖于预定义的感兴趣区（ROI）或静态的功能连接（FC），难以捕捉复杂的、非线性的、且具有高度个体差异的神经塑性变化。
*   **研究背景**：虽然深度学习在神经影像领域展现了潜力，但在样本量较小的临床干预研究中容易过拟合。新兴的“基础模型”（Foundation Models, FMs）通过在海量数据上预训练，学习通用的脑活动时空表征，为解决小样本、高异质性临床数据的分析提供了新途径。本研究旨在验证这些模型能否在真实的认知老化干预试验中，鲁棒地识别出与认知改善相关的潜在神经模式。

### 2. 论文提出的方法论
*   **核心思想**：利用在大规模健康人群数据上预训练的 rsfMRI 基础模型作为特征提取器，通过“领域自适应微调”和“线性探测”策略，提取纵向脑动态表征，并将其与行为结果（情景记忆变化）关联。
*   **关键技术细节**：
    *   **基础模型选择**：评估了两种架构：**BrainLM**（基于掩码自编码器的生成式模型，擅长捕捉长程时间依赖）和 **BrainJEPA**（基于联合嵌入预测架构，强调时空一致性）。
    *   **领域自适应（Domain Adaptation）**：使用 ADNI 数据集（阿尔茨海默病 vs. 健康对照分类任务）对 BrainLM 进行微调。采用 **LoRA（低秩自适应）** 技术，仅更新极少数参数，使模型在保留通用表征的同时，学习老化相关的病理特征。
    *   **纵向建模**：采用双流架构处理基线（T1）和干预后（T2）的扫描数据，将提取的嵌入向量（Embeddings）拼接，以捕捉干预诱导的神经变化。
    *   **潜在模式识别**：使用 **偏最小二乘法（PLS）** 将高维的基础模型嵌入映射回低维的脑空间（如 ALFF 载荷图），从而识别出具有生物学解释性的神经靶点。

### 3. 实验设计
*   **数据集**：
    *   **ADNI**：用于临床领域自适应微调。
    *   **ACT 试验**：多中心随机对照试验（N=105），包含运动、认知训练及其组合。
    *   **CogTE 试验**：单中心随机对照试验（N=58），侧重于认知训练。
*   **Benchmark（对比方法）**：
    *   **传统机器学习**：支持向量机（SVM）基于功能连接（FC）特征。
    *   **深度学习**：多层感知器（MLP）和图卷积网络（GCN）。
*   **评估指标**：分类准确率（ACC）、F1 分数、AUC、敏感性和特异性。

### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的 GPU 型号、数量或具体的训练时长。但考虑到使用了 13M 参数量的 BrainLM 模型及 LoRA 微调技术，这类实验通常在单张消费级显卡（如 RTX 3090/4090）或中等规模的计算集群上即可完成。

### 5. 实验数量与充分性
*   **实验规模**：研究在两个独立的干预试验（ACT 和 CogTE）上进行了验证，这在临床干预研究中属于较为严谨的外部验证。
*   **充分性与客观性**：
    *   执行了**分层五折交叉验证**，平衡了结果标签、干预组别和站点。
    *   进行了**消融实验**，对比了仅基线（T1）、仅变化量（T2-T1）及联合建模（T1+T2）的效果。
    *   进行了**鲁棒性分析**，验证了模型对头动、扫描站点和干预方案的敏感度。
    *   实验设计客观，通过跨研究的一致性分析（PLS 载荷相关性）证明了发现的神经模式并非研究特异性的伪影。

### 6. 主要结论与发现
*   **性能优越性**：基础模型（尤其是 BrainLM）在预测情景记忆改善方面显著优于传统 ML 和 GCN 方法。
*   **微调的重要性**：经过 ADNI 临床数据微调后的 BrainLM-ADNI 性能提升最显著，在 ACT 试验中准确率达到 72.6%，在 CogTE 中达到 81.6%。
*   **神经模式发现**：
    *   **基线一致性**：在干预前，响应者与非响应者在默认模式网络（DMN）、视觉网络和额顶网络（如前部扣带回、内侧前额叶）表现出跨研究一致的差异。
    *   **干预后分布性**：干预后的神经模式变得更加空间弥散，反映了干预效果的复杂性和上下文依赖性。
*   **鲁棒性**：模型对头动和站点差异具有很强的抵抗力，无需复杂的显式去噪即可保持稳定性能。

### 7. 优点（亮点）
*   **范式创新**：提出了一种“三条件框架”（丰富表征、行为相关、跨研究鲁棒），为临床神经影像研究利用大模型提供了标准化路径。
*   **临床实用性**：证明了在不需要海量局部数据的情况下，通过迁移学习可以显著提升小规模临床试验的分析效力。
*   **可解释性**：通过 PLS 将黑盒模型的嵌入向量转化为可直观理解的脑图，弥合了深度学习与神经科学解释之间的鸿沟。

### 8. 不足与局限
*   **模型覆盖有限**：仅测试了 BrainLM 和 BrainJEPA 两种模型，且受限于公开权重，未能测试更大规模（如 650M 参数）的变体。
*   **样本量瓶颈**：虽然跨两个试验验证，但总样本量（N<200）对于深度学习而言仍偏小，可能限制了模型学习更细微神经动态的能力。
*   **干预特异性不足**：研究主要关注通用的“响应者”特征，尚未深入探讨不同干预方式（如纯运动 vs. 纯认知训练）之间特有的神经机制差异。
*   **应用限制**：目前仍处于事后分析阶段，将其转化为预测个体未来干预收益的临床工具仍需前瞻性验证。

（完）
