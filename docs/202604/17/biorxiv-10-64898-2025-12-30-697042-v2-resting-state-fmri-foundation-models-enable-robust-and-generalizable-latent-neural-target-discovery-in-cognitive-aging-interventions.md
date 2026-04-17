---
title: Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions
title_zh: 静息态 fMRI 基础模型助力认知老化干预中稳健且可泛化的潜在神经靶点发现
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
针对认知老化的干预效果在个体间存在显著差异，这在很大程度上归因于与老化相关的共病异质性。因此，有必要稳健地识别干预反应背后的神经模式，并测试其在异质性队列中的可泛化性。静息态功能磁共振成像（rsfMRI）提供了一条潜在途径，但传统方法依赖预定义的汇总特征，在捕捉个体内的纵向变化和个体间的差异方面能力有限，特别是在样本量较小且具有异质性的研究中。近期在大型观测队列上预训练的 rsfMRI 基础模型通过从时间序列信号中学习可迁移的时空表征，提供了一个极具前景的替代方案。然而，这些模型在局部干预场景中的有效性和可泛化性仍不明确。在本研究中，我们利用两项针对轻度认知障碍老年人的独立随机对照试验数据，系统评估了 rsfMRI 基础模型，测试这些模型能否稳健地提取纵向大脑表征，从而跨试验预测干预后情景记忆的变化。结果显示，在两项试验中，基础模型的表现均优于传统的机器学习和深度学习方法。利用外部阿尔茨海默病队列进行的临床信息适配进一步提高了性能以及对混杂因素（即头动、站点和干预组别）的鲁棒性，准确率高达 82%。对基础模型嵌入进行的多元分解识别出了与情景记忆变化相关的潜在神经模式；这些模式在基线时具有跨研究的一致性，而在干预后则在空间分布上变得更加广泛。这些发现表明，rsfMRI 基础模型能够稳健且可泛化地识别将纵向大脑动态与个体干预反应联系起来的潜在神经模式，为认知老化研究中精准驱动的神经靶点发现奠定了基础。

## Abstract
The benefits of interventions targeting cognitive aging vary substantially across individuals, largely owing to heterogeneity in aging-related comorbidities. It is necessary to robustly identify neural patterns underlying intervention response and test their generalizability across heterogeneous cohorts. Resting-state functional MRI (rsfMRI) offers a potential pathway, but relying on predefined summary features with conventional methods has limited capacity to capture both within-individual longitudinal variation and between-individual differences, particularly in small and heterogeneous studies. Recent rsfMRI foundation models pretrained on large observational cohorts present a promising alternative by learning transferable spatiotemporal representations from time-series signals. Yet their validity and generalizability in local intervention settings remain unclear. Here, we systematically evaluated rsfMRI foundation models using data from two independent randomized controlled trials of older adults with mild cognitive impairment, testing whether these models can robustly extract longitudinal brain representations that predict post-intervention changes in episodic memory across trials. Foundation models outperformed conventional machine learning and deep learning approaches across both trials. Clinically informed adaptation using an external Alzheimer's disease cohort further improved performance and robustness to confounders (i.e., head motion, site, and intervention arm), with accuracy up to 82%. Multivariate decomposition of foundation model embeddings identified latent neural patterns associated with episodic memory change with cross-study consistency at baseline that became more spatially distributed at post-intervention. These findings show that rsfMRI foundation models can enable robust and generalizable identification of latent neural patterns linking longitudinal brain dynamics to individual intervention response, laying the foundation for precision-driven neural target discovery in cognitive aging research.

---

## 论文详细总结（自动生成）

这篇论文探讨了如何利用静息态功能磁共振成像（rsfMRI）基础模型，在认知老化干预研究中识别稳健且可泛化的神经靶点。以下是对该论文的结构化总结：

### 1. 核心问题与研究动机
*   **核心问题**：针对认知老化的干预措施（如运动、认知训练）在个体间效果差异巨大，且传统的 rsfMRI 分析方法（依赖预定义的感兴趣区 ROI 或静态功能连接 FC）难以捕捉复杂的、异质性的纵向神经变化，导致在小样本临床试验中难以识别可靠的神经机制。
*   **研究动机**：利用在大规模数据上预训练的基础模型（Foundation Models, FMs）学习大脑的时空表征，探索其是否能比传统方法更有效地预测个体干预反应，并识别出跨研究一致的潜在神经模式。

### 2. 方法论
*   **核心思想**：采用“预训练 + 领域自适应微调 + 线性探测”的架构。
*   **关键技术细节**：
    *   **基础模型选择**：评估了两种模型：**BrainLM**（基于掩码自编码的自回归序列建模）和 **BrainJEPA**（基于联合嵌入预测架构）。
    *   **领域自适应（Domain Adaptation）**：使用 ADNI 数据集（包含健康老人和阿尔茨海默病患者）对 BrainLM 进行微调，使其学习与老化和病理相关的神经特征。
    *   **纵向建模**：采用双流架构处理基线（T1）和干预后（T2）的 rsfMRI 数据，提取 CLS token 嵌入并拼接，以捕捉纵向神经动态。
    *   **潜在模式识别**：利用偏最小二乘法（PLS）将高维的基础模型嵌入映射到低维潜在变量，并与行为结果（情景记忆变化 $\Delta EM$）关联。
*   **算法流程**：原始 BOLD 时间序列 $\rightarrow$ 基础模型特征提取 $\rightarrow$ 拼接 T1/T2 嵌入 $\rightarrow$ 轻量级分类器预测 $\rightarrow$ PLS 分解识别空间模式。

### 3. 实验设计
*   **数据集**：
    *   **微调集**：ADNI（用于临床适应性调整）。
    *   **测试集（独立 RCT）**：**ACT 研究**（多中心，6个月运动+认知训练）和 **CogTE 研究**（单中心，6周认知训练）。
*   **Benchmark（对比方法）**：
    *   **传统机器学习**：支持向量机（SVM）。
    *   **深度学习**：多层感知器（MLP）和图卷积网络（GCN）。
    *   *注：对比方法均使用预定义的节点间功能连接（FC）作为输入。*
*   **评估指标**：准确率（ACC）、F1 分数、AUC、敏感性和特异性。

### 4. 资源与算力
*   **算力说明**：论文提到了使用 **LoRA（低秩自适应）** 技术进行轻量化微调，以降低计算成本并防止过拟合。
*   **明确性**：文中**未明确列出**具体的 GPU 型号、数量或具体的训练时长。但提到使用了 BrainLM（13M 参数版本）和 BrainJEPA（22M 参数版本）的公开预训练权重。

### 5. 实验数量与充分性
*   **实验规模**：
    *   进行了跨两个独立临床试验的验证（ACT 和 CogTE）。
    *   执行了消融实验（如 T1、T2、T2-T1 不同输入组合的对比）。
    *   进行了鲁棒性测试（针对站点差异、头动参数、干预组别的混杂因素分析）。
*   **充分性与客观性**：实验设计较为充分，采用了分层五折交叉验证，确保了结果的客观性。通过在两个设计迥异的试验中获得一致结论，增强了研究的说服力。

### 6. 主要结论与发现
*   **性能优越性**：基础模型（尤其是经过 ADNI 微调的 BrainLM-ADNI）在预测干预反应方面显著优于 SVM、MLP 和 GCN，准确率最高达 **82%**。
*   **领域适配的重要性**：在老化相关的临床数据上进行微调，显著提升了模型在干预研究中的表现。
*   **纵向信息价值**：同时使用 T1 和 T2 数据比仅使用单一时间点或简单的差值信号效果更好。
*   **神经模式一致性**：识别出的潜在神经模式在基线时表现出跨研究的高度一致性（集中在后内侧皮层等核心区域），而干预后的变化模式则更具空间分布性和上下文相关性。

### 7. 优点（亮点）
*   **突破预定义限制**：不再依赖人工定义的 FC 特征，而是直接从原始 BOLD 时间序列中学习特征。
*   **强泛化性**：在两个完全独立的干预研究中证明了模型的有效性，这在神经影像学研究中非常难得。
*   **鲁棒性强**：证明了模型对头动和多中心站点差异等常见噪声具有天然的抵抗力。
*   **三条件框架**：提出了建立稳健潜在神经模式的三个必要条件（表征丰富性、行为相关性、跨研究一致性），具有理论指导意义。

### 8. 不足与局限
*   **样本量限制**：尽管使用了基础模型，但下游干预研究的样本量（ACT 和 CogTE）相对较小，可能限制了对更复杂模式的挖掘。
*   **模型架构差异**：BrainLM 表现优于 BrainJEPA，说明不同基础模型的预训练目标对特定临床任务的适用性存在差异，需进一步探索。
*   **解释性挑战**：虽然使用了 PLS 进行可视化，但深度学习模型的黑盒性质使得将潜在嵌入完全对应到具体生物学机制仍有难度。
*   **应用范围**：目前仅验证了情景记忆这一指标，其他认知领域（如执行功能）的适用性尚待验证。

（完）
