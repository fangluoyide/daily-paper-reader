---
title: Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions
title_zh: 静息态 fMRI 基础模型助力认知衰老干预中鲁棒且可泛化的潜在神经靶点发现
authors: "Zhou, X., Ai, M., Adeli, E., Zhang, Y., Liu, Y. M., Vankee-Lin, F."
date: 2026-04-15
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.30.697042v2.full.pdf"
tags: ["query:cog-eld"]
score: 8.0
evidence: 认知老化干预中的神经模式
tldr: 本研究针对认知衰老干预效果的个体差异问题，利用在大规模数据集上预训练的静息态fMRI（rsfMRI）基础模型，识别与干预反应相关的潜在神经模式。通过在两个独立轻度认知障碍临床试验中进行验证，该方法成功预测了情景记忆的改善情况，其表现优于传统机器学习方法，为认知衰老研究中的精准神经靶点发现提供了新途径。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-001.webp\", \"caption\": \"Figure 4. Three-condition framework for identifying robust and generalizable neural patterns in 687 cognitive aging intervention studies. rsfMRI FMs are applied to local intervention studies 688 characterized by small sample sizes and heterogeneous responses. Under Condition 1 (rich 689 spatiotemporal representation), FMs extract latent neural embeddings from BOLD time series that 690 capture distributed dynamics beyond predefined features, enabling robust representation learning 691 and improved prediction of outcomes. Under Condition 2 (behavioral relevance), these 692 embeddings are linked to behavioral metrics through multivariate analysis, yielding latent 693 variables that characterize individual differences in intervention response. These latent 694 representations further support the identification of interpretable neural patterns. Under Condition 695 3 (cross-study robustness), neural patterns are evaluated across independent studies to identify 696 shared structures, distinguish arm-specific effects, and enable cross-study alignment. Together, 697 these steps define an intervention representation atlas that captures both shared and study-698 specific neural signatures. Alternative approaches, including cross-dataset transfer, embedding 699 alignment, and external validation, may provide complementary assessments of generalizability. 700\", \"page\": 18, \"index\": 1, \"width\": 970, \"height\": 334}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-002.webp\", \"caption\": \"Figure 5. Study datasets and implementation of rsfMRI FMs and comparison methods. (a) The 704 ACT and CogTE studies serve as independent intervention cohorts for downstream evaluation 705 and assessment of model generalizability across intervention paradigms and study designs. (b) 706 Domain-adaptive finetuning of BrainLM using the ADNI dataset via LoRA. Supervised finetuning 707 is performed to incorporate aging- and pathology-related brain patterns, yielding the adapted 708 BrainLM-ADNI model that is subsequently used as a frozen feature extractor in all downstream 709 intervention analyses. (c) Linear probing strategy for deploying pretrained rsfMRI FMs in 710 longitudinal intervention studies. The rsfMRI data collected at baseline (T1) and post-intervention 711 (T2) are processed independently through a frozen FM with shared weights, and CLS-token 712 embeddings from each timepoint are concatenated to explicitly encode longitudinal neural change 713 for downstream inference of EM outcomes. (d) Architectures of conventional comparison models. 714 FC features derived from rsfMRI data at T1 and T2 are used to train an SVM, an MLP, and a 715 dual-stream GCN that explicitly models longitudinal brain network changes. NOTE: rsfMRI, 716 resting-state functional magnetic resonance imaging; FM, foundation model; ACT, Aerobic 717 exercise and Cognitive Training study; MLA, mental leisure activity; CogTE, Cognitive Training 718 and Exercise study; ADNI, Alzheimer’s Disease Neuroimaging Initiative; EM, episodic memory; 719 FC, functional connectivity; T1/T2, baseline/post-intervention timepoints; SVM, support vector 720 machine; MLP, multilayer perceptron; GCN, graph convolutional network; LoRA, low-rank 721 adaptation; AD, Alzheimer’s Disease; HC, healthy control. 722\", \"page\": 19, \"index\": 2, \"width\": 972, \"height\": 469}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-003.webp\", \"caption\": \"Figure 3. PLS-derived embedding-brain associations and cross-study spatial patterns. (a-b) ACT 673 (a) and CogTE (b) PLS results. Top: T1; bottom: T2. Left: relationship between embedding scores 674 and brain scores. Middle: group differences in brain scores. Right: group differences in 675 embedding scores. Points are colored by responder status (stable vs. decline). Reported 676 statistics correspond to two-sample t-tests on subject-level PLS scores. For each study and 677 timepoint, the component shown represents the dominant embedding-brain association capturing 678 group differentiation. (c) Cross-study correlations of PLS brain loading patterns across increasing 679 thresholds of top-weighted regions (ranked by absolute loading). (d-e) Cross-study average 680 spatial distribution of top-weighted PLS loadings at baseline (T1; left) and post-intervention (T2; 681 right), shown in standard anatomical views and illustrating shared spatial organization of latent 682 neural patterns across the two intervention studies. 683\", \"page\": 17, \"index\": 3, \"width\": 978, \"height\": 514}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-004.webp\", \"caption\": \"Figure 2. Evaluation of rsfMRI FMs for classifying intervention-related episodic memory 652 response. (a) Benchmark comparison of classification performance between rsfMRI FMs 653 (BrainLM, BrainJEPA) and conventional ML and DL approaches (SVM, MLP, GCN) across two 654 independent intervention cohorts (CogTE and ACT). Models are trained to classify participants as 655 episodic memory responders vs. non-responders, based on pre-post changes in EM, using 656 baseline (T1) and post-intervention (T2) rsfMRI data. ACC and F1-score are reported as mean ± 657 standard deviation across stratified cross-validation folds. (b) Performance of the BrainLM-ADNI 658 under different timepoint combinations. Classification results for T1 + T2, T1-only, and T2 − T1 659 input settings are shown for CogTE and ACT datasets (mean ± standard deviation across cross-660 validation folds). (c) Robustness of the adapted FM to common neuroimaging confounders in the 661 multi-site ACT dataset. Classification performance of BrainLM-ADNI is shown for original data, 662 data after site harmonization, and data after both site harmonization and head-motion regression. 663 (d) Classification performance of BrainLM-ADNI stratified by intervention arm in both CogTE and 664 ACT studies. Chi-square tests indicate no significant association between intervention 665 assignment and classification correctness. NOTE: rsfMRI, resting-state functional magnetic 666 resonance imaging; FM, foundation model; ML, machine learning; DL, deep learning; SVM, 667 support vector machine; MLP, multilayer perceptron; GCN, graph convolutional network; ACT, 668 Aerobic exercise and Cognitive Training study; CogTE, Cognitive Training and Exercise study; 669 ADNI, Alzheimer’s Disease Neuroimaging Initiative; ACC, accuracy. 670\", \"page\": 16, \"index\": 4, \"width\": 899, \"height\": 516}]"
motivation: 传统的rsfMRI分析方法难以捕捉复杂的个体差异和纵向变化，限制了对认知衰老干预反应的准确预测。
method: 研究者采用在大规模队列上预训练的rsfMRI基础模型，并结合阿尔茨海默病临床数据进行领域自适应微调，以提取预测情景记忆变化的纵向脑表征。
result: "基础模型在两个独立试验中均优于传统模型，预测准确率高达82%，且对头动、站点和干预分组等干扰因素具有较强的鲁棒性。"
conclusion: rsfMRI基础模型能够稳健且可泛化地识别连接大脑动态与干预反应的潜在神经模式，为老龄化人群的精准干预策略奠定了基础。
---

## 摘要
针对认知衰老的干预效果在个体间存在显著差异，这在很大程度上归因于衰老相关共病的异质性。因此，有必要稳健地识别干预反应背后的神经模式，并测试其在异质队列中的可泛化性。静息态功能磁共振成像（rsfMRI）提供了一条潜在途径，但传统方法依赖预定义的汇总特征，在捕捉个体内的纵向变化和个体间的差异方面能力有限，特别是在样本量较小且具有异质性的研究中。最近在大型观察性队列上预训练的 rsfMRI 基础模型通过从时间序列信号中学习可迁移的时空表征，提供了一个极具前景的替代方案。然而，它们在局部干预环境中的有效性和可泛化性仍不明确。在本研究中，我们利用两项针对轻度认知障碍老年人的独立随机对照试验数据，系统评估了 rsfMRI 基础模型，测试这些模型能否稳健地提取纵向大脑表征，从而预测跨试验的干预后情景记忆变化。在两项试验中，基础模型的表现均优于传统的机器学习和深度学习方法。利用外部阿尔茨海默病队列进行的临床信息适配进一步提高了性能以及对混杂因素（即头动、中心和干预组别）的鲁棒性，准确率高达 82%。对基础模型嵌入进行的多元分解识别出了与情景记忆变化相关的潜在神经模式，这些模式在基线时具有跨研究的一致性，而在干预后在空间分布上变得更加广泛。这些研究结果表明，rsfMRI 基础模型能够稳健且可泛化地识别将纵向大脑动态与个体干预反应联系起来的潜在神经模式，为认知衰老研究中精准驱动的神经靶点发现奠定了基础。

意义声明：认知衰老的干预措施在不同个体间表现出高度变异的结果，限制了其临床有效性。本研究引入了一种基于基础模型的方法，利用静息态 fMRI 识别干预反应个体差异背后的潜在神经模式。通过利用预训练模型和领域自适应微调，我们证明了跨独立试验对认知改善的稳健且可泛化的预测。我们的研究结果表明，潜在的大脑表征而非预定义的特征，为针对老年群体的精准驱动干预策略提供了一条可扩展的途径。

## Abstract
The benefits of interventions targeting cognitive aging vary substantially across individuals, largely owing to heterogeneity in aging-related comorbidities. It is necessary to robustly identify neural patterns underlying intervention response and test their generalizability across heterogeneous cohorts. Resting-state functional MRI (rsfMRI) offers a potential pathway, but relying on predefined summary features with conventional methods has limited capacity to capture both within-individual longitudinal variation and between-individual differences, particularly in small and heterogeneous studies. Recent rsfMRI foundation models pretrained on large observational cohorts present a promising alternative by learning transferable spatiotemporal representations from time-series signals. Yet their validity and generalizability in local intervention settings remain unclear. Here, we systematically evaluated rsfMRI foundation models using data from two independent randomized controlled trials of older adults with mild cognitive impairment, testing whether these models can robustly extract longitudinal brain representations that predict post-intervention changes in episodic memory across trials. Foundation models outperformed conventional machine learning and deep learning approaches across both trials. Clinically informed adaptation using an external Alzheimers disease cohort further improved performance and robustness to confounders (i.e., head motion, site, and intervention arm), with accuracy up to 82%. Multivariate decomposition of foundation model embeddings identified latent neural patterns associated with episodic memory change with cross-study consistency at baseline that became more spatially distributed at post-intervention. These findings show that rsfMRI foundation models can enable robust and generalizable identification of latent neural patterns linking longitudinal brain dynamics to individual intervention response, laying the foundation for precision-driven neural target discovery in cognitive aging research.

Significance StatementInterventions for cognitive aging show highly variable outcomes across individuals, limiting their clinical effectiveness. This study introduces a foundation model-based approach to identify latent neural patterns underlying individual differences in intervention response using resting-state fMRI. By leveraging pretrained models and domain-adaptive fine-tuning, we demonstrate robust and generalizable prediction of cognitive improvement across independent trials. Our findings suggest that latent brain representations, rather than predefined features, provide a scalable pathway toward precision-driven intervention strategies for aging populations.

---

## 论文详细总结（自动生成）

### 论文总结：静息态 fMRI 基础模型助力认知衰老干预中鲁棒且可泛化的潜在神经靶点发现

#### 1. 论文的核心问题与整体含义
*   **研究背景**：针对认知衰老（如轻度认知障碍 MCI）的干预措施（如运动、认知训练）在个体间表现出高度的疗效差异。
*   **核心问题**：传统的静息态 fMRI（rsfMRI）分析方法（如基于预定义脑区的连接组学）难以捕捉复杂的时空动态，且在样本量较小、异质性强的临床试验数据中往往缺乏鲁棒性和跨研究的泛化能力。
*   **整体含义**：本研究旨在探索在大规模观察性数据上预训练的 **rsfMRI 基础模型（Foundation Models, FMs）** 是否能比传统方法更有效地提取纵向神经表征，从而精准预测干预后的认知改善情况，并识别通用的神经靶点。

#### 2. 论文提出的方法论
*   **核心思想**：利用预训练模型强大的特征提取能力，通过“领域自适应”将通用脑活动模式迁移到特定的认知衰老干预场景中。
*   **关键技术细节**：
    *   **基础模型选择**：采用了 **BrainLM**（基于掩码自编码器）和 **BrainJEPA**（基于联合嵌入预测架构）两种主流 rsfMRI 基础模型。
    *   **领域自适应微调（Domain-adaptive Finetuning）**：使用来自 ADNI（阿尔茨海默病神经影像学倡议）的临床数据，通过 **LoRA（低秩自适应）** 技术对 BrainLM 进行微调，使其学习与衰老和病理相关的脑模式。
    *   **特征提取与纵向建模**：将模型作为冻结的特征提取器，提取基线（T1）和干预后（T2）的潜层嵌入（Latent Embeddings），通过拼接（Concatenation）方式捕捉纵向神经变化。
    *   **下游预测**：采用线性探测（Linear Probing）策略，利用提取的嵌入特征预测情景记忆（Episodic Memory）的改善（Responder vs. Non-responder）。
    *   **可解释性分析**：使用偏最小二乘法（PLS）将高维嵌入映射回解剖空间，识别与认知变化相关的空间神经模式。

#### 3. 实验设计
*   **数据集**：
    *   **ACT 研究**：多中心随机对照试验（n=124），包含有氧运动和认知训练。
    *   **CogTE 研究**：独立干预队列（n=44），包含认知训练和运动。
    *   **ADNI**：用于领域自适应微调的外部临床数据集。
*   **Benchmark（基准）**：
    *   **传统机器学习**：支持向量机（SVM）。
    *   **深度学习**：多层感知器（MLP）、图卷积网络（GCN）。
*   **对比特征**：传统方法使用基于全脑分区（如 Schaefer 400 模板）计算的功能连接（FC）矩阵作为输入。

#### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的 GPU 型号、数量或训练总时长。但提到了使用 LoRA 进行高效微调，这通常意味着对显存和计算资源的要求低于全参数微调。

#### 5. 实验数量与充分性
*   **实验规模**：
    *   在两个独立的临床试验（ACT 和 CogTE）上进行了交叉验证。
    *   进行了**消融实验**，对比了不同时间点组合（仅 T1、仅 T2、T1+T2、T2-T1）对预测性能的影响。
    *   进行了**鲁棒性分析**，测试了模型对头动（Head Motion）、扫描站点（Site）和干预组别（Intervention Arm）等混杂因素的敏感度。
*   **充分性评价**：实验设计非常充分且客观。通过跨研究验证（Cross-study validation）证明了模型的泛化性，而非仅仅在单一数据集上过拟合。

#### 6. 主要结论与发现
*   **性能优越性**：基础模型（尤其是经过 ADNI 微调后的 BrainLM-ADNI）在预测认知改善方面显著优于传统 FC 方法，准确率最高达到 **82%**。
*   **鲁棒性**：FM 提取的特征对头动和站点效应具有天然的抵抗力，无需复杂的后期去噪处理即可保持高性能。
*   **神经靶点发现**：识别出了跨研究一致的神经模式。基线时，预测因子集中在默认网络（DMN）和额顶网络；干预后，相关的神经模式在空间上变得更加广泛，反映了干预引起的脑网络重组。
*   **领域自适应的重要性**：引入临床相关的先验知识（通过 ADNI 微调）能显著提升模型在老年群体中的表现。

#### 7. 优点
*   **范式创新**：将“预训练+微调”的基础模型范式引入小样本、高异质性的临床干预研究，解决了传统方法特征工程受限的问题。
*   **跨研究验证**：在两个独立的 RCT 试验中验证了结果，增强了结论的生物学可信度和临床应用潜力。
*   **端到端解释性**：不仅关注预测精度，还通过 PLS 框架将抽象的潜层向量转化为可理解的大脑空间图谱。

#### 8. 不足与局限
*   **样本量限制**：虽然在临床试验中算大样本，但对于深度学习模型而言，总样本量（约 170 人）仍然较小，可能限制了模型复杂能力的完全释放。
*   **干预特异性**：研究主要关注通用的认知改善，未深入探讨不同干预类型（如单纯运动 vs. 单纯认知训练）之间是否存在特异性的神经表征差异。
*   **计算成本**：尽管使用了 LoRA，但相比于简单的线性模型，基础模型的部署和推理仍需要更高的计算门槛。

（完）
