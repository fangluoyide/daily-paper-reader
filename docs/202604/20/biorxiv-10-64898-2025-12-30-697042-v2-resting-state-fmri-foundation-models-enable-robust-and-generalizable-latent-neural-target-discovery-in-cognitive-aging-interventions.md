---
title: Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions
title_zh: 静息态 fMRI 基础模型助力认知衰老干预中鲁棒且可泛化的潜在神经靶点发现
authors: "Zhou, X., Ai, M., Adeli, E., Zhang, Y., Liu, Y. M., Vankee-Lin, F."
date: 2026-04-15
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.30.697042v2.full.pdf"
tags: ["query:cog-eld"]
score: 9.0
evidence: 用于识别认知老化干预中神经目标的 fMRI 基础模型
tldr: 本研究针对认知衰老干预效果的个体差异问题，利用在大规模数据集上预训练的静息态磁共振（rsfMRI）基础模型，识别与干预反应相关的潜在神经模式。通过在两个独立轻度认知障碍临床试验中进行验证，该模型成功预测了干预后情景记忆的变化，其表现优于传统机器学习方法，为认知衰老研究中的精准神经靶点发现提供了新途径。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-001.webp\", \"caption\": \"Figure 4. Three-condition framework for identifying robust and generalizable neural patterns in 687 cognitive aging intervention studies. rsfMRI FMs are applied to local intervention studies 688 characterized by small sample sizes and heterogeneous responses. Under Condition 1 (rich 689 spatiotemporal representation), FMs extract latent neural embeddings from BOLD time series that 690 capture distributed dynamics beyond predefined features, enabling robust representation learning 691 and improved prediction of outcomes. Under Condition 2 (behavioral relevance), these 692 embeddings are linked to behavioral metrics through multivariate analysis, yielding latent 693 variables that characterize individual differences in intervention response. These latent 694 representations further support the identification of interpretable neural patterns. Under Condition 695 3 (cross-study robustness), neural patterns are evaluated across independent studies to identify 696 shared structures, distinguish arm-specific effects, and enable cross-study alignment. Together, 697 these steps define an intervention representation atlas that captures both shared and study-698 specific neural signatures. Alternative approaches, including cross-dataset transfer, embedding 699 alignment, and external validation, may provide complementary assessments of generalizability. 700\", \"page\": 18, \"index\": 1, \"width\": 970, \"height\": 334}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-002.webp\", \"caption\": \"Figure 5. Study datasets and implementation of rsfMRI FMs and comparison methods. (a) The 704 ACT and CogTE studies serve as independent intervention cohorts for downstream evaluation 705 and assessment of model generalizability across intervention paradigms and study designs. (b) 706 Domain-adaptive finetuning of BrainLM using the ADNI dataset via LoRA. Supervised finetuning 707 is performed to incorporate aging- and pathology-related brain patterns, yielding the adapted 708 BrainLM-ADNI model that is subsequently used as a frozen feature extractor in all downstream 709 intervention analyses. (c) Linear probing strategy for deploying pretrained rsfMRI FMs in 710 longitudinal intervention studies. The rsfMRI data collected at baseline (T1) and post-intervention 711 (T2) are processed independently through a frozen FM with shared weights, and CLS-token 712 embeddings from each timepoint are concatenated to explicitly encode longitudinal neural change 713 for downstream inference of EM outcomes. (d) Architectures of conventional comparison models. 714 FC features derived from rsfMRI data at T1 and T2 are used to train an SVM, an MLP, and a 715 dual-stream GCN that explicitly models longitudinal brain network changes. NOTE: rsfMRI, 716 resting-state functional magnetic resonance imaging; FM, foundation model; ACT, Aerobic 717 exercise and Cognitive Training study; MLA, mental leisure activity; CogTE, Cognitive Training 718 and Exercise study; ADNI, Alzheimer’s Disease Neuroimaging Initiative; EM, episodic memory; 719 FC, functional connectivity; T1/T2, baseline/post-intervention timepoints; SVM, support vector 720 machine; MLP, multilayer perceptron; GCN, graph convolutional network; LoRA, low-rank 721 adaptation; AD, Alzheimer’s Disease; HC, healthy control. 722\", \"page\": 19, \"index\": 2, \"width\": 972, \"height\": 469}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-003.webp\", \"caption\": \"Figure 3. PLS-derived embedding-brain associations and cross-study spatial patterns. (a-b) ACT 673 (a) and CogTE (b) PLS results. Top: T1; bottom: T2. Left: relationship between embedding scores 674 and brain scores. Middle: group differences in brain scores. Right: group differences in 675 embedding scores. Points are colored by responder status (stable vs. decline). Reported 676 statistics correspond to two-sample t-tests on subject-level PLS scores. For each study and 677 timepoint, the component shown represents the dominant embedding-brain association capturing 678 group differentiation. (c) Cross-study correlations of PLS brain loading patterns across increasing 679 thresholds of top-weighted regions (ranked by absolute loading). (d-e) Cross-study average 680 spatial distribution of top-weighted PLS loadings at baseline (T1; left) and post-intervention (T2; 681 right), shown in standard anatomical views and illustrating shared spatial organization of latent 682 neural patterns across the two intervention studies. 683\", \"page\": 17, \"index\": 3, \"width\": 978, \"height\": 514}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-30-697042-v2/fig-004.webp\", \"caption\": \"Figure 2. Evaluation of rsfMRI FMs for classifying intervention-related episodic memory 652 response. (a) Benchmark comparison of classification performance between rsfMRI FMs 653 (BrainLM, BrainJEPA) and conventional ML and DL approaches (SVM, MLP, GCN) across two 654 independent intervention cohorts (CogTE and ACT). Models are trained to classify participants as 655 episodic memory responders vs. non-responders, based on pre-post changes in EM, using 656 baseline (T1) and post-intervention (T2) rsfMRI data. ACC and F1-score are reported as mean ± 657 standard deviation across stratified cross-validation folds. (b) Performance of the BrainLM-ADNI 658 under different timepoint combinations. Classification results for T1 + T2, T1-only, and T2 − T1 659 input settings are shown for CogTE and ACT datasets (mean ± standard deviation across cross-660 validation folds). (c) Robustness of the adapted FM to common neuroimaging confounders in the 661 multi-site ACT dataset. Classification performance of BrainLM-ADNI is shown for original data, 662 data after site harmonization, and data after both site harmonization and head-motion regression. 663 (d) Classification performance of BrainLM-ADNI stratified by intervention arm in both CogTE and 664 ACT studies. Chi-square tests indicate no significant association between intervention 665 assignment and classification correctness. NOTE: rsfMRI, resting-state functional magnetic 666 resonance imaging; FM, foundation model; ML, machine learning; DL, deep learning; SVM, 667 support vector machine; MLP, multilayer perceptron; GCN, graph convolutional network; ACT, 668 Aerobic exercise and Cognitive Training study; CogTE, Cognitive Training and Exercise study; 669 ADNI, Alzheimer’s Disease Neuroimaging Initiative; ACC, accuracy. 670\", \"page\": 16, \"index\": 4, \"width\": 899, \"height\": 516}]"
motivation: 传统rsfMRI分析方法难以捕捉复杂的个体差异和纵向变化，限制了对认知衰老干预反应异质性的理解和预测。
method: 系统评估了在大规模队列上预训练的rsfMRI基础模型，并结合阿尔茨海默病临床数据进行领域自适应微调，以提取预测记忆变化的纵向脑表征。
result: "基础模型在跨试验预测中表现优于传统方法，准确率高达82%，且对头动、站点和干预分组等混杂因素具有较强的鲁棒性。"
conclusion: rsfMRI基础模型能够稳健且可推广地识别连接大脑动态与干预反应的潜在神经模式，为老龄化人群的精准干预策略奠定了基础。
---

## 摘要
针对认知衰老的干预效果在个体间存在显著差异，这在很大程度上归因于衰老相关共病的异质性。因此，有必要稳健地识别干预反应背后的神经模式，并测试其在异质队列中的可泛化性。静息态功能磁共振成像（rsfMRI）提供了一条潜在途径，但传统方法依赖预定义的汇总特征，在捕捉个体内的纵向变化和个体间的差异方面能力有限，特别是在样本量较小且具有异质性的研究中。最近在大型观察性队列上预训练的 rsfMRI 基础模型通过从时间序列信号中学习可迁移的时空表征，提供了一个极具前景的替代方案。然而，它们在局部干预环境中的有效性和可泛化性仍不明确。在本研究中，我们利用两项针对轻度认知障碍老年人的独立随机对照试验数据，系统评估了 rsfMRI 基础模型，测试这些模型能否稳健地提取纵向大脑表征，从而预测跨试验的干预后情景记忆变化。在两项试验中，基础模型的表现均优于传统的机器学习和深度学习方法。利用外部阿尔茨海默病队列进行的临床信息适配进一步提高了性能以及对混杂因素（即头动、中心和干预组别）的鲁棒性，准确率高达 82%。对基础模型嵌入进行的多元分解识别出了与情景记忆变化相关的潜在神经模式，这些模式在基线时具有跨研究的一致性，而在干预后在空间分布上变得更加广泛。这些研究结果表明，rsfMRI 基础模型能够稳健且可泛化地识别将纵向大脑动态与个体干预反应联系起来的潜在神经模式，为认知衰老研究中精准驱动的神经靶点发现奠定了基础。

意义声明：认知衰老的干预措施在不同个体间表现出高度变异的结果，限制了其临床有效性。本研究引入了一种基于基础模型的方法，利用静息态 fMRI 识别干预反应个体差异背后的潜在神经模式。通过利用预训练模型和领域自适应微调，我们证明了跨独立试验对认知改善的稳健且可泛化的预测。我们的研究结果表明，潜在的大脑表征而非预定义的特征，为针对老年群体的精准驱动干预策略提供了一条可扩展的途径。

## Abstract
The benefits of interventions targeting cognitive aging vary substantially across individuals, largely owing to heterogeneity in aging-related comorbidities. It is necessary to robustly identify neural patterns underlying intervention response and test their generalizability across heterogeneous cohorts. Resting-state functional MRI (rsfMRI) offers a potential pathway, but relying on predefined summary features with conventional methods has limited capacity to capture both within-individual longitudinal variation and between-individual differences, particularly in small and heterogeneous studies. Recent rsfMRI foundation models pretrained on large observational cohorts present a promising alternative by learning transferable spatiotemporal representations from time-series signals. Yet their validity and generalizability in local intervention settings remain unclear. Here, we systematically evaluated rsfMRI foundation models using data from two independent randomized controlled trials of older adults with mild cognitive impairment, testing whether these models can robustly extract longitudinal brain representations that predict post-intervention changes in episodic memory across trials. Foundation models outperformed conventional machine learning and deep learning approaches across both trials. Clinically informed adaptation using an external Alzheimers disease cohort further improved performance and robustness to confounders (i.e., head motion, site, and intervention arm), with accuracy up to 82%. Multivariate decomposition of foundation model embeddings identified latent neural patterns associated with episodic memory change with cross-study consistency at baseline that became more spatially distributed at post-intervention. These findings show that rsfMRI foundation models can enable robust and generalizable identification of latent neural patterns linking longitudinal brain dynamics to individual intervention response, laying the foundation for precision-driven neural target discovery in cognitive aging research.

Significance StatementInterventions for cognitive aging show highly variable outcomes across individuals, limiting their clinical effectiveness. This study introduces a foundation model-based approach to identify latent neural patterns underlying individual differences in intervention response using resting-state fMRI. By leveraging pretrained models and domain-adaptive fine-tuning, we demonstrate robust and generalizable prediction of cognitive improvement across independent trials. Our findings suggest that latent brain representations, rather than predefined features, provide a scalable pathway toward precision-driven intervention strategies for aging populations.

---

## 论文详细总结（自动生成）

这是一份关于论文《Resting-state fMRI foundation models enable robust and generalizable latent neural target discovery in cognitive aging interventions》的结构化深入分析总结：

### 1. 核心问题与研究背景
*   **核心问题**：针对认知衰老（如轻度认知障碍 MCI）的干预措施（如运动、认知训练）在个体间表现出极大的效果差异。
*   **研究背景**：传统的静息态磁共振（rsfMRI）分析依赖于预定义的感兴趣区（ROI）或功能连接（FC）特征，难以捕捉复杂的、高阶的、个体化的神经可塑性模式。此外，传统的深度学习模型在样本量较小的临床干预研究中极易过拟合。
*   **整体含义**：本研究旨在探索 rsfMRI 基础模型（Foundation Models, FMs）是否能通过学习原始时间序列中的时空表征，更稳健地识别干预反应的神经靶点，并实现跨研究的泛化。

### 2. 方法论
*   **核心思想**：利用在大规模人群数据上预训练的基础模型提取大脑表征，通过“领域自适应微调”使其适应老龄化人群，最后通过“线性探测”预测干预后的认知变化。
*   **关键技术细节**：
    *   **基础模型选择**：评估了 **BrainLM**（基于掩码自编码器的自回归序列模型）和 **BrainJEPA**（基于联合嵌入预测架构的模型）。
    *   **领域自适应（Domain Adaptation）**：使用 ADNI 数据集（阿尔茨海默病 vs. 健康对照）对 BrainLM 进行微调，引入 LoRA（低秩自适应）技术，使模型学习与衰老和病理相关的神经模式。
    *   **纵向建模**：采用双流架构，同时处理基线（T1）和干预后（T2）的 rsfMRI 数据，将提取的嵌入（Embeddings）拼接，以捕捉纵向神经变化。
    *   **潜在模式发现**：利用偏最小二乘法（PLS）将高维的基础模型嵌入与全脑神经活动（ALFF 图）关联，识别出区分“反应者”与“非反应者”的潜在神经模式。

### 3. 实验设计
*   **数据集**：
    *   **微调集**：ADNI（用于临床领域适配）。
    *   **测试集 1**：ACT 研究（多中心随机对照试验，6 个月运动+认知训练）。
    *   **测试集 2**：CogTE 研究（单中心随机对照试验，6 周认知训练）。
*   **Benchmark（基准方法）**：
    *   **传统机器学习**：支持向量机（SVM）。
    *   **深度学习**：多层感知器（MLP）、图卷积网络（GCN）。
    *   *注：基准方法均使用传统的功能连接（FC）作为输入特征。*
*   **对比维度**：预测准确率（ACC）、F1 分数、时间点组合（仅 T1、仅 T2、T1+T2）、混杂因素鲁棒性（站点、头动、干预组别）。

### 4. 资源与算力
*   **模型规模**：使用了 BrainLM（1300 万参数版本）和 BrainJEPA（2200 万参数版本）。
*   **算力说明**：论文中**未明确说明**具体的 GPU 型号、数量或训练总时长。但提到了使用 LoRA 技术进行轻量化微调，这通常意味着对算力的需求相对较低，适合在局部临床数据集上部署。

### 5. 实验数量与充分性
*   **实验规模**：
    *   进行了跨两个独立临床试验（ACT 和 CogTE）的验证。
    *   实施了分层五折交叉验证，确保了结果的稳定性。
    *   进行了消融实验（对比不同时间点输入、不同基础模型架构）。
    *   进行了鲁棒性分析（针对头动、多中心效应、干预方案差异）。
*   **充分性评价**：实验设计非常充分且严谨。通过在两个设计迥异（时长、干预手段、中心数量均不同）的试验中获得一致性结果，有力证明了该方法的泛化能力。

### 6. 主要结论与发现
*   **性能优越**：基础模型（尤其是经过 ADNI 微调的 BrainLM）在预测认知改善方面显著优于 SVM、MLP 和 GCN，准确率最高达 **82%**。
*   **微调必要性**：临床信息的领域适配（ADNI 微调）对于提升模型在老年群体中的表现至关重要。
*   **纵向价值**：同时结合基线和干预后的脑表征比单一时间点提供更多预测信息。
*   **神经模式一致性**：识别出的潜在神经模式在基线时具有跨研究的高度一致性（集中在后部中线皮层等核心区域），而干预后的变化模式则表现出更高的空间分布性和上下文依赖性。

### 7. 优点与亮点
*   **突破特征限制**：摆脱了预定义 ROI 和静态 FC 的束缚，直接从原始 BOLD 信号中学习动态时空特征。
*   **高鲁棒性**：证明了模型对临床研究中常见的“噪声”（如头动、多中心差异）具有很强的抵抗力。
*   **临床转化潜力**：为“精准医疗”提供了工具，能够识别哪些个体更有可能从特定干预中受益（潜在神经靶点发现）。

### 8. 不足与局限
*   **样本量限制**：尽管使用了基础模型，但下游干预研究的样本量（N 约 100-200）相对较小，可能限制了对更复杂交互作用的探索。
*   **模型版本限制**：由于开源限制，仅使用了较小参数版本的基础模型（如 BrainLM 13M），更大规模的模型（如 650M）效果尚未可知。
*   **解释性挑战**：虽然使用了 PLS 进行解释，但基础模型的“黑箱”属性依然存在，潜在嵌入空间与具体生物学机制的对应关系仍需进一步挖掘。
*   **应用范围**：目前仅验证了情景记忆这一指标，对于其他认知领域（如执行功能、注意力）的适用性有待验证。

（完）
