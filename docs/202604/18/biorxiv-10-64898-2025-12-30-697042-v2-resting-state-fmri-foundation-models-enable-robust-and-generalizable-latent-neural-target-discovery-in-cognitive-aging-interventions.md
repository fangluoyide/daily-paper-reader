---
title: Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions
title_zh: 静息态 fMRI 基础模型助力认知衰老干预中稳健且可泛化的潜在神经靶点发现
authors: "Zhou, X., Ai, M., Adeli, E., Zhang, Y., Liu, Y. M., Vankee-Lin, F."
date: 2026-04-15
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.30.697042v2.full.pdf"
tags: ["query:cog-eld"]
score: 9.0
evidence: 认知老化干预中的神经目标发现
tldr: "本研究针对认知老化干预效果个体差异大且传统rsfMRI分析方法泛化性不足的问题，提出利用在大规模数据上预训练的基础模型来识别干预反应的潜在神经模式。通过在两个轻度认知障碍临床试验中进行验证，该模型结合临床适应性微调，成功实现了对情景记忆改善的跨研究稳健预测，准确率达82%，为老龄化研究中的精准神经靶点发现提供了新途径。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-001.webp\", \"caption\": \"Figure 4. Three-condition framework for identifying robust and generalizable neural patterns in 687 cognitive aging intervention studies. rsfMRI FMs are applied to local intervention studies 688 characterized by small sample sizes and heterogeneous responses. Under Condition 1 (rich 689 spatiotemporal representation), FMs extract latent neural embeddings from BOLD time series that 690 capture distributed dynamics beyond predefined features, enabling robust representation learning 691 and improved prediction of outcomes. Under Condition 2 (behavioral relevance), these 692 embeddings are linked to behavioral metrics through multivariate analysis, yielding latent 693 variables that characterize individual differences in intervention response. These latent 694 representations further support the identification of interpretable neural patterns. Under Condition 695 3 (cross-study robustness), neural patterns are evaluated across independent studies to identify 696 shared structures, distinguish arm-specific effects, and enable cross-study alignment. Together, 697 these steps define an intervention representation atlas that captures both shared and study-698 specific neural signatures. Alternative approaches, including cross-dataset transfer, embedding 699 alignment, and external validation, may provide complementary assessments of generalizability. 700\", \"page\": 18, \"index\": 1, \"width\": 970, \"height\": 334}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-002.webp\", \"caption\": \"Figure 5. Study datasets and implementation of rsfMRI FMs and comparison methods. (a) The 704 ACT and CogTE studies serve as independent intervention cohorts for downstream evaluation 705 and assessment of model generalizability across intervention paradigms and study designs. (b) 706 Domain-adaptive finetuning of BrainLM using the ADNI dataset via LoRA. Supervised finetuning 707 is performed to incorporate aging- and pathology-related brain patterns, yielding the adapted 708 BrainLM-ADNI model that is subsequently used as a frozen feature extractor in all downstream 709 intervention analyses. (c) Linear probing strategy for deploying pretrained rsfMRI FMs in 710 longitudinal intervention studies. The rsfMRI data collected at baseline (T1) and post-intervention 711 (T2) are processed independently through a frozen FM with shared weights, and CLS-token 712 embeddings from each timepoint are concatenated to explicitly encode longitudinal neural change 713 for downstream inference of EM outcomes. (d) Architectures of conventional comparison models. 714 FC features derived from rsfMRI data at T1 and T2 are used to train an SVM, an MLP, and a 715 dual-stream GCN that explicitly models longitudinal brain network changes. NOTE: rsfMRI, 716 resting-state functional magnetic resonance imaging; FM, foundation model; ACT, Aerobic 717 exercise and Cognitive Training study; MLA, mental leisure activity; CogTE, Cognitive Training 718 and Exercise study; ADNI, Alzheimer’s Disease Neuroimaging Initiative; EM, episodic memory; 719 FC, functional connectivity; T1/T2, baseline/post-intervention timepoints; SVM, support vector 720 machine; MLP, multilayer perceptron; GCN, graph convolutional network; LoRA, low-rank 721 adaptation; AD, Alzheimer’s Disease; HC, healthy control. 722\", \"page\": 19, \"index\": 2, \"width\": 972, \"height\": 469}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-003.webp\", \"caption\": \"Figure 3. PLS-derived embedding-brain associations and cross-study spatial patterns. (a-b) ACT 673 (a) and CogTE (b) PLS results. Top: T1; bottom: T2. Left: relationship between embedding scores 674 and brain scores. Middle: group differences in brain scores. Right: group differences in 675 embedding scores. Points are colored by responder status (stable vs. decline). Reported 676 statistics correspond to two-sample t-tests on subject-level PLS scores. For each study and 677 timepoint, the component shown represents the dominant embedding-brain association capturing 678 group differentiation. (c) Cross-study correlations of PLS brain loading patterns across increasing 679 thresholds of top-weighted regions (ranked by absolute loading). (d-e) Cross-study average 680 spatial distribution of top-weighted PLS loadings at baseline (T1; left) and post-intervention (T2; 681 right), shown in standard anatomical views and illustrating shared spatial organization of latent 682 neural patterns across the two intervention studies. 683\", \"page\": 17, \"index\": 3, \"width\": 978, \"height\": 514}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-004.webp\", \"caption\": \"Figure 2. Evaluation of rsfMRI FMs for classifying intervention-related episodic memory 652 response. (a) Benchmark comparison of classification performance between rsfMRI FMs 653 (BrainLM, BrainJEPA) and conventional ML and DL approaches (SVM, MLP, GCN) across two 654 independent intervention cohorts (CogTE and ACT). Models are trained to classify participants as 655 episodic memory responders vs. non-responders, based on pre-post changes in EM, using 656 baseline (T1) and post-intervention (T2) rsfMRI data. ACC and F1-score are reported as mean ± 657 standard deviation across stratified cross-validation folds. (b) Performance of the BrainLM-ADNI 658 under different timepoint combinations. Classification results for T1 + T2, T1-only, and T2 − T1 659 input settings are shown for CogTE and ACT datasets (mean ± standard deviation across cross-660 validation folds). (c) Robustness of the adapted FM to common neuroimaging confounders in the 661 multi-site ACT dataset. Classification performance of BrainLM-ADNI is shown for original data, 662 data after site harmonization, and data after both site harmonization and head-motion regression. 663 (d) Classification performance of BrainLM-ADNI stratified by intervention arm in both CogTE and 664 ACT studies. Chi-square tests indicate no significant association between intervention 665 assignment and classification correctness. NOTE: rsfMRI, resting-state functional magnetic 666 resonance imaging; FM, foundation model; ML, machine learning; DL, deep learning; SVM, 667 support vector machine; MLP, multilayer perceptron; GCN, graph convolutional network; ACT, 668 Aerobic exercise and Cognitive Training study; CogTE, Cognitive Training and Exercise study; 669 ADNI, Alzheimer’s Disease Neuroimaging Initiative; ACC, accuracy. 670\", \"page\": 16, \"index\": 4, \"width\": 899, \"height\": 516}]"
motivation: 旨在解决传统rsfMRI特征提取方法难以捕捉认知老化干预中复杂的个体差异及纵向变化，从而提升干预反应预测的泛化性。
method: 采用在大规模观测队列上预训练的rsfMRI基础模型，并结合外部阿尔茨海默病队列进行临床适应性微调，以提取时空神经表征。
result: "基础模型在预测情景记忆变化方面显著优于传统机器学习方法，实现了高达82%的预测准确率，并展现出跨研究的一致性和对混杂因素的鲁棒性。"
conclusion: rsfMRI基础模型能够稳健地识别与干预反应相关的潜在神经模式，为实现认知老化干预的精准化和规模化提供了重要技术支撑。
---

## 摘要
针对认知衰老的干预措施的获益在个体间存在显著差异，这在很大程度上归因于衰老相关共病的异质性。因此，有必要稳健地识别干预反应背后的神经模式，并测试其在异质队列中的可泛化性。静息态功能磁共振成像（rsfMRI）提供了一条潜在路径，但传统方法依赖预定义的汇总特征，在捕捉个体内的纵向变化和个体间的差异方面能力有限，特别是在小型且具有异质性的研究中。最近在大型观察性队列上预训练的 rsfMRI 基础模型通过从时间序列信号中学习可迁移的时空表征，提供了一个极具前景的替代方案。然而，它们在局部干预环境中的有效性和可泛化性仍不明确。在本研究中，我们利用两项针对轻度认知障碍老年人的独立随机对照试验数据，系统评估了 rsfMRI 基础模型，测试这些模型能否稳健地提取纵向大脑表征，以预测跨试验的干预后情景记忆变化。在两项试验中，基础模型的表现均优于传统的机器学习和深度学习方法。利用外部阿尔茨海默病队列进行的临床信息适配进一步提高了性能以及对混杂因素（即头动、站点和干预组别）的鲁棒性，准确率高达 82%。对基础模型嵌入进行的多元分解识别出了与情景记忆变化相关的潜在神经模式，这些模式在基线时具有跨研究的一致性，而在干预后在空间分布上变得更加广泛。这些研究结果表明，rsfMRI 基础模型能够稳健且可泛化地识别将纵向大脑动态与个体干预反应联系起来的潜在神经模式，为认知衰老研究中精准驱动的神经靶点发现奠定了基础。

意义声明：认知衰老的干预措施在不同个体间表现出高度多变的结局，限制了其临床有效性。本研究引入了一种基于基础模型的方法，利用静息态 fMRI 识别干预反应个体差异背后的潜在神经模式。通过利用预训练模型和领域自适应微调，我们证明了跨独立试验对认知改善的稳健且可泛化的预测。我们的研究结果表明，潜在的大脑表征而非预定义的特征，为针对老年群体的精准驱动干预策略提供了一条可扩展的路径。

## Abstract
The benefits of interventions targeting cognitive aging vary substantially across individuals, largely owing to heterogeneity in aging-related comorbidities. It is necessary to robustly identify neural patterns underlying intervention response and test their generalizability across heterogeneous cohorts. Resting-state functional MRI (rsfMRI) offers a potential pathway, but relying on predefined summary features with conventional methods has limited capacity to capture both within-individual longitudinal variation and between-individual differences, particularly in small and heterogeneous studies. Recent rsfMRI foundation models pretrained on large observational cohorts present a promising alternative by learning transferable spatiotemporal representations from time-series signals. Yet their validity and generalizability in local intervention settings remain unclear. Here, we systematically evaluated rsfMRI foundation models using data from two independent randomized controlled trials of older adults with mild cognitive impairment, testing whether these models can robustly extract longitudinal brain representations that predict post-intervention changes in episodic memory across trials. Foundation models outperformed conventional machine learning and deep learning approaches across both trials. Clinically informed adaptation using an external Alzheimers disease cohort further improved performance and robustness to confounders (i.e., head motion, site, and intervention arm), with accuracy up to 82%. Multivariate decomposition of foundation model embeddings identified latent neural patterns associated with episodic memory change with cross-study consistency at baseline that became more spatially distributed at post-intervention. These findings show that rsfMRI foundation models can enable robust and generalizable identification of latent neural patterns linking longitudinal brain dynamics to individual intervention response, laying the foundation for precision-driven neural target discovery in cognitive aging research.

Significance StatementInterventions for cognitive aging show highly variable outcomes across individuals, limiting their clinical effectiveness. This study introduces a foundation model-based approach to identify latent neural patterns underlying individual differences in intervention response using resting-state fMRI. By leveraging pretrained models and domain-adaptive fine-tuning, we demonstrate robust and generalizable prediction of cognitive improvement across independent trials. Our findings suggest that latent brain representations, rather than predefined features, provide a scalable pathway toward precision-driven intervention strategies for aging populations.

---

## 论文详细总结（自动生成）

这篇论文探讨了如何利用静息态磁共振成像（rsfMRI）基础模型来解决认知衰老干预研究中的个体差异和泛化性难题。以下是对该研究的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：针对认知衰老（如轻度认知障碍，MCI）的干预措施（如运动、认知训练）效果在个体间存在巨大差异。传统的 rsfMRI 分析方法依赖于预定义的特征（如功能连接 FC），难以捕捉复杂的时空动态变化，且在样本量较小的临床试验中往往缺乏泛化性，难以识别稳健的神经靶点。
*   **整体含义**：本研究旨在验证在大规模数据上预训练的 **rsfMRI 基础模型（Foundation Models, FMs）** 是否能比传统方法更有效地提取具有生物学意义的潜在表征，从而精准预测干预后的认知改善（情景记忆），并实现跨研究的稳健应用。

### 2. 提出方法论
*   **核心思想**：利用预训练模型捕捉大脑原始信号中的非线性、动态特征，而非依赖人工设计的汇总统计量。
*   **关键技术细节**：
    *   **基础模型选择**：采用了 **BrainLM**（基于掩码自编码器）和 **BrainJEPA**（基于联合嵌入预测架构）两种主流 rsfMRI 基础模型。
    *   **领域自适应微调（Domain-adaptive Finetuning）**：使用 **ADNI（阿尔茨海默病神经影像学倡议）** 数据集，通过 **LoRA（低秩自适应）** 技术对模型进行微调。这一步至关重要，它使模型能够学习到与衰老和病理相关的特定大脑模式。
    *   **纵向特征提取**：采用“线性探测（Linear Probing）”策略。将基线（T1）和干预后（T2）的 rsfMRI 数据分别输入冻结权重的模型，提取 CLS 标记嵌入（Embeddings），并将其拼接以编码纵向神经变化。
    *   **多元分解（PLS）**：使用偏最小二乘法（Partial Least Squares）将高维嵌入与行为得分关联，识别出可解释的潜在神经模式。

### 3. 实验设计
*   **数据集**：
    *   **ACT 研究**：有氧运动与认知训练试验（多中心，样本量较大）。
    *   **CogTE 研究**：认知训练与运动试验（单中心）。
    *   **ADNI**：用于临床适应性微调的外部数据集。
*   **Benchmark（基准）与对比方法**：
    *   **传统机器学习**：支持向量机（SVM）、多层感知器（MLP）。
    *   **深度学习**：双流图卷积网络（GCN），专门用于建模纵向脑网络变化。
    *   **特征输入**：传统方法使用基于脑图谱的功能连接（FC）矩阵。
*   **任务**：分类情景记忆（EM）的“反应者”（改善者）与“非反应者”。

### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的 GPU 型号、数量或总训练时长。但提到了使用 LoRA 进行微调，这是一种参数高效的微调方法，通常比全参数微调显著降低算力需求。

### 5. 实验数量与充分性
*   **实验规模**：
    *   在两个独立的临床试验数据集（ACT 和 CogTE）上进行了验证。
    *   进行了**消融实验**，对比了仅使用 T1、仅使用 T2 以及 T1+T2 组合的效果。
    *   进行了**鲁棒性测试**，评估了模型对头动（Head Motion）、扫描站点（Site）和干预组别（Intervention Arm）的敏感性。
*   **充分性评价**：实验设计较为充分且客观。通过跨研究验证（Cross-study validation）证明了模型的泛化能力，这在神经影像学研究中是极具挑战性的。

### 6. 主要结论与发现
*   **性能卓越**：基础模型（尤其是经过 ADNI 微调后的 BrainLM-ADNI）在预测情景记忆改善方面显著优于所有传统方法，准确率达到 **82%**。
*   **跨研究一致性**：模型识别出的潜在神经模式在两个独立研究中表现出高度的空间一致性，尤其是在基线时期。
*   **鲁棒性强**：模型表现不受头动或扫描站点的干扰，且能准确捕捉不同干预方式（如单纯运动 vs. 联合训练）下的共同神经反应。
*   **时空演变**：干预后的神经模式比基线时在空间分布上更广泛，反映了干预诱导的大脑可塑性。

### 7. 优点（亮点）
*   **范式转移**：从“人工定义特征”转向“学习潜在表征”，克服了传统 FC 分析的信息损失问题。
*   **临床适配**：巧妙地利用外部病理数据集（ADNI）进行微调，增强了模型在特定临床群体（MCI 老年人）中的敏感度。
*   **高泛化性**：在异质性很强的多中心数据上依然保持稳健，证明了基础模型在临床转化中的潜力。

### 8. 不足与局限
*   **样本量限制**：虽然在临床试验中算大样本，但对于深度学习模型而言，数百人的规模仍可能存在过拟合风险（尽管使用了预训练模型缓解）。
*   **黑盒性质**：尽管使用了 PLS 进行了解释，但基础模型提取的嵌入向量（Embeddings）其具体的生物学含义仍不如传统的解剖区域连接那样直观。
*   **认知维度单一**：研究重点主要放在情景记忆上，对于其他认知域（如执行功能、注意力）的覆盖不足。
*   **应用限制**：目前仅针对 MCI 群体，其结论是否能推广到健康老化或其他神经退行性疾病尚需验证。

（完）
