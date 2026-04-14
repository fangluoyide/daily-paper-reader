---
title: Structural Connectome Analysis using a Graph-based Deep Model for Age and Dementia Prediction
title_zh: 基于图深度模型的结构连接组分析，用于年龄与痴呆症预测
authors: "Kazi, A., Mora, J., Fischl, B., Dalca, A., Aganj, I."
date: 2026-04-10
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.09.642165v3.full.pdf"
tags: ["query:cog-eld"]
score: 8.0
evidence: 预测年龄和痴呆症MMSE评分
tldr: 本研究提出一种基于图卷积网络（GCN）的深度学习模型，旨在通过弥散磁共振成像衍生的结构脑连接组预测年龄和MMSE评分。该模型采用并行多分支GCN架构，并引入创新的连接注意力模块（Connectivity Attention Block）来学习脑图的嵌入表示。在PREVENT-AD和OASIS3数据集上的实验表明，该方法在处理人口统计学和临床变量预测任务时表现优异，为理解健康与疾病状态下的脑网络变化提供了新工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-001.webp\", \"caption\": \"Table 4: Performance evaluation for all the methods on 10% unseen test data. Bold and Blue indicate the best and second-best, respectively, in each column. For the fullforms and corresponding citation please refer to Table 2.\", \"page\": 15, \"index\": 1, \"width\": 1108, \"height\": 517}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-002.webp\", \"caption\": \"Table 3: Cross-validation results by all methods for the MMSE prediction task on the validation set using the OASIS3 dataset. Bold and Blue indicate the best and second-best, respectively, in each column. For the fullforms and corresponding citation please refer to Table 2.\", \"page\": 15, \"index\": 2, \"width\": 792, \"height\": 459}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-003.webp\", \"caption\": \"Table 7: This table summarizes the selected hyperparameters and training efficiency across three setups. The learning rate was set to 0.0001 for all experiments, except for the age task on the OASIS3 dataset, where it was empirically set to 0.001. The proposed model is competitive in runtime, but its parameter count and speed vary by dataset, showing that performance depends strongly on the task.\", \"page\": 21, \"index\": 3, \"width\": 875, \"height\": 773}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-004.webp\", \"caption\": \"Figure 3: Scatter plots comparing predicted age to ground-truth age on the OASIS3 dataset. Each dot represents a subject in the test set. The darker line is the identity line, whereas the lighter line is the least-squares line. The color indicates the MMSE score.\", \"page\": 30, \"index\": 4, \"width\": 950, \"height\": 1206}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-005.webp\", \"caption\": \"Figure 1: Overview of an end-to-end DL architecture for brain connectivity analysis using dMRI and tractography. The pre-processing module (left) includes the dMRI-based tracts forming the structural connectome matrices. dMRI-derived features (FA, ADC, degree) are concatenated with each row of the connectivity matrix and then used as node features. The model (middle) processes input features and graphs through residual GCNs, fully connected (FC) layers, and a novel Connectivity Attention Block (CAB, right), which refines the graph structure and highlights key connections. Outputs from all modules are combined to predict phenotypes. See the Method section for more details.\", \"page\": 7, \"index\": 5, \"width\": 1056, \"height\": 387}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-006.webp\", \"caption\": \"Table 2: Age prediction results on the validation set from the 10-fold cross-validation, for the PREVENTAD and OASIS3 datasets. Asterisk ‘*’ indicates that the proposed method significantly outperformed the respective methods when compared using paired t-test (with α = 0.05). Bold and blue indicate the best and second-best, respectively, in each column. LR = Linear Regression (Su et al., 2012); Support Vector Regression (SVR) (Awad & Khanna, 2015); DT = Decision Tree (De Ville, 2013); RT = Regression Tree (Loh, 2011); ET = Ensemble Tree (Che et al., 2011); NN = Neural Network (S.-C. Wang, 2003); MLP (Goodfellow et al., 2016); GCN (Kipf & Welling, 2016); GIN (K. Xu et al., 2018); GraphConv (Fey & Lenssen, 2019); ResGCN (Pei et al., 2022).\", \"page\": 14, \"index\": 6, \"width\": 1050, \"height\": 355}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-007.webp\", \"caption\": \"Figure 2: Histograms of the ground-truth values in the cross-validation (purple bars) and test (orange bars) sets for all datasets and tasks. The mean of each cross-validation distribution is marked by thick red dotted lines, while the standard deviation is indicated by thin green dotted lines. These visualizations help assess how well the training and test distributions align and provide insights into potential challenges in model training. For the PREVENT-AD dataset, the age distribution is notably skewed, indicating an imbalance in subject age representation. The OASIS3 dataset’s MMSE distribution exhibits a power-law trend, where most samples cluster in the higher score range (i.e., cognitively normal individuals), with relatively few samples showing lower scores. The age distribution in the OASIS3 dataset is approximately symmetric and Gaussian, which is more favorable for training.\", \"page\": 17, \"index\": 7, \"width\": 950, \"height\": 250}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-008.webp\", \"caption\": \"Figure 5: Scatter plots for test set on OASIS3 dataset for the task of MMSE prediction. The darker line is the identity line, whereas the lighter line is the least-squares line. The color indicates the ground-truth MMSE.\", \"page\": 32, \"index\": 8, \"width\": 950, \"height\": 1223}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-009.webp\", \"caption\": \"Figure 4: Scatter plots of prediction performance for the test set of the PREVENT-AD dataset for the task of age prediction. The darker line is the identity line, whereas the lighter line is the least-squares line. The color indicates the ground-truth age.\", \"page\": 31, \"index\": 9, \"width\": 950, \"height\": 1202}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-010.webp\", \"caption\": \"Table 6: Top regions identified across different tasks.\", \"page\": 20, \"index\": 10, \"width\": 990, \"height\": 216}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-09-642165-v3/fig-011.webp\", \"caption\": \"Table 5: Ablations on the prediction tasks. Each column represents the respective block removed from the pipeline. Bold and Blue indicate the best and second-best, respectively, in each row. Mod denotes a module ablation. We define: Mod 1 — no ResGCN layers; Mod 2 — no FC1 layer; Mod 3 — no CAB; Mod 4 — no skip connection; Mod i — no E in CAB; Mod ii (left) — no GmmT and Mod ii (right) no G in GmmT ; Mod iii— no Sigmoid in CAB; Mod iv — no MLPs in CAB.\", \"page\": 16, \"index\": 11, \"width\": 977, \"height\": 565}]"
motivation: 旨在利用结构脑连接组数据更准确地预测年龄和认知功能指标，以深化对大脑健康与疾病演变规律的理解。
method: 提出一种结合并行多分支GCN与连接注意力模块的深度学习架构，通过图级注意力机制实现对脑网络特征的高效提取。
result: 在公开数据集上的实验验证表明，该模型在年龄和MMSE评分预测任务中均显著优于传统机器学习及现有的图深度学习方法。
conclusion: 研究证明了基于图注意力的深度学习模型在分析复杂脑连接数据方面的有效性，为神经影像学的临床预测提供了强有力的技术支持。
---

## 摘要
本研究利用基于图的机器学习，探讨了基于弥散磁共振成像衍生的结构脑连接对非影像变量的预测。我们选取年龄和简易精神状态检查（MMSE）评分分别作为人口统计学变量和临床变量的示例进行预测。我们提出了一种受图卷积网络（GCN）启发的机器学习模型，该模型以脑连接图作为输入，并通过具有多个分支的并行GCN机制对数据进行独立处理。本研究的创新之处在于其模型架构，特别是连接注意力模块（Connectivity Attention Block），该模块在提供图级注意力的同时学习脑图的嵌入表示。我们在公开数据集 PREVENT-AD 和 OASIS3 上进行了实验，并通过与现有方法的对比及消融实验验证了模型的有效性。这量化了连接组随任务变化的程度，对于深化我们对人群健康与疾病的理解至关重要。与我们测试的现有机器学习算法（包括传统方法以及图和非图深度学习）相比，所提模型通常表现出更优越的性能，尤其是在年龄预测任务中。

## Abstract
We address the prediction of non-imaging variables based on structural brain connectivity derived from diffusion magnetic resonance images, using graph-based machine learning. We predict age and the mini-mental state examination (MMSE) score as examples of a demographic and a clinical variable. We propose a machine-learning model inspired by graph convolutional networks (GCNs), which takes a brain connectivity graph as input and processes the data separately through a parallel GCN mechanism with multiple branches. The novelty of our work lies in the model architecture, especially the Connectivity Attention Block, which learns an embedding representation of brain graphs while providing graph-level attention. We show experiments on publicly available datasets of PREVENT-AD and OASIS3. We validate our model by comparing it to existing methods and via ablations. This quantifies the degree to which the connectome varies depending on the task, which is important for improving our understanding of health and disease across the population. The proposed model generally demonstrates higher performance especially for age prediction compared to the existing machine-learning algorithms we tested, including classical methods and (graph and non-graph) deep learning.

---

## 论文详细总结（自动生成）

### 论文结构化深入总结：基于图深度模型的结构连接组分析

#### 1. 核心问题与整体含义（研究动机和背景）
论文关注的核心问题是如何利用**弥散磁共振成像（dMRI）**衍生的**结构脑连接组（Structural Connectome）**数据，准确预测非影像变量，如生理年龄和临床认知评分（MMSE）。
*   **背景**：脑连接组描述了大脑区域间的白质通路，是理解发育、衰老及神经退行性疾病（如阿尔茨海默症）的关键。
*   **动机**：脑连接数据具有高维度、非欧几里得结构的特点，传统的卷积神经网络（CNN）难以直接处理。现有的图神经网络（GNN）在处理密集脑网络时容易出现“过度平滑”或泛化能力差的问题。因此，研究者旨在开发一种既能捕捉局部解剖特征，又能提取全局连接模式的鲁棒深度学习模型。

#### 2. 论文提出的方法论
论文提出了一种多分支并行架构的图深度学习模型，核心思想是融合图卷积、全连接网络和创新的注意力机制。
*   **核心架构（四个模块）**：
    1.  **图卷积模块（Module 1）**：采用带残差连接的图卷积网络（ResGCN），通过两个不同嵌入维度的分支捕捉图的低级和高级结构特征。
    2.  **全连接模块（Module 2）**：直接处理原始节点特征，提取与图结构无关的独立信息。
    3.  **连接注意力模块（CAB, Module 3 - 核心创新）**：
        *   学习一个图级注意力权重，通过 Frobenius 内积生成受试者级别的嵌入表示。
        *   利用秩一投影（Rank-one projection）技术，将复杂的连接矩阵 $G$ 简化为任务相关的表示，动态识别对预测最重要的脑区连接。
    4.  **跳跃连接（Module 4）**：将原始特征直接传递至输出层，缓解深层网络中的梯度消失问题。
*   **损失函数**：结合了 **Huber Loss**（对异常值具有鲁棒性）和针对注意力掩码的正则化项。

#### 3. 实验设计
*   **数据集**：
    *   **PREVENT-AD**：347名受试者，789次扫描（针对有AD风险的人群）。
    *   **OASIS3**：771名受试者，1294次扫描（涵盖正常老化到AD患者）。
*   **Benchmark（基准方法）**：
    *   **传统机器学习**：线性回归（LR）、支持向量回归（SVR）、决策树（DT）、集成树（ET）等。
    *   **深度学习**：多层感知机（MLP）、标准图卷积（GCN）、图同构网络（GIN）、GraphConv、ResGCN。
*   **评估指标**：RMSE、MAE、Pearson 相关系数（PC）、Spearman 相关系数（SC）。

#### 4. 资源与算力
*   **硬件环境**：Linux 服务器，配置 512 GB RAM，Intel Xeon Gold 6256 CPU。
*   **GPU**：使用了一块 **NVIDIA RTX A6000 (48 GB)** 显卡。
*   **模型规模**：提出的模型参数量约为 **5073** 个，与对比的 GNN 模型（如 DGCNN、GraphConv）处于同一量级，属于轻量级架构。
*   **训练时长**：文中提供了每轮（epoch）的训练时间，在 OASIS3 数据集上约为 0.41 - 1.14 秒/轮，显示出较高的计算效率。

#### 5. 实验数量与充分性
*   **实验规模**：
    *   进行了 **10 折交叉验证**，确保结果的统计稳定性。
    *   保留了 **10% 的独立测试集**（Unseen Test Set），用于验证模型的泛化能力。
    *   针对 PREVENT-AD 和 OASIS3 两个独立的大型公开数据集进行了验证。
*   **消融实验**：进行了极其详尽的消融研究（Mod 1-4 以及 CAB 内部组件的 4 种变体），验证了每个模块（如 ResGCN、CAB、跳跃连接）的必要性。
*   **客观性**：实验采用了相同的划分策略和预处理流程，并进行了配对 t 检验以验证显著性，实验设计客观且公平。

#### 6. 主要结论与发现
*   **性能优越性**：提出的模型在**年龄预测**任务中显著优于所有传统 ML 和现有 DL 方法，在两个数据集上均取得了最低的误差和最高的相关性。
*   **MMSE 预测挑战**：在 MMSE 预测中，模型表现虽优于其他 DL 方法，但与 SVR 等传统方法相比优势不明显。这归因于 MMSE 分数分布极度倾斜（大部分受试者分数较高），导致模型难以学习细微的认知衰退模式。
*   **生物学一致性**：CAB 模块自动识别出的重要脑区（如右侧海马体、后扣带回）与现有神经科学文献中关于衰老和痴呆的关键区域高度一致。

#### 7. 优点
*   **架构创新**：CAB 模块通过矩阵属性（秩一投影）而非简单的节点注意力来处理脑图，更符合脑连接组的全局特性。
*   **多分支融合**：成功结合了图结构特征与非结构化特征，增强了模型对异质数据的处理能力。
*   **解释性**：注意力机制能够定位关键脑区，为临床研究提供潜在的生物标志物线索。
*   **效率高**：参数量少，训练速度快，适合大规模神经影像数据分析。

#### 8. 不足与局限
*   **数据分布敏感性**：对于像 MMSE 这样具有严重偏态分布（Skewed distribution）的临床指标，模型的提升效果有限。
*   **任务局限**：目前仅验证了回归任务（年龄、评分），尚未在分类任务（如诊断分类）中进行大规模验证。
*   **外部验证**：虽然使用了两个数据集，但均来自公开库，未来需在更多样化的临床真实场景（Domain Shift）中测试其鲁棒性。

（完）
