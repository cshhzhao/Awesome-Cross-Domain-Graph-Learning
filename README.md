<h1 align="center"> Awesome-Cross-Domain-Graph-Learning</h2>
<h5 align="center">A collection of AWESOME things about performing cross-domain learning on Graphs. Our survey has been published on https://arxiv.org/abs/2503.11086. </h5>

<h5 align="center">
  
![Awesome](https://awesome.re/badge.svg)   ![GitHub stars](https://img.shields.io/github/stars/cshhzhao/Awesome-Cross-Domain-Graph-Learning.svg)

</h5>

## Why is cross-domain graph learning important?

Real-world graph data are abundant but inherently fragmented across heterogeneous application domains, such as social networks, molecular systems, financial transactions, transportation systems, and recommendation platforms. However, most existing graph models are still developed and optimized within individual graph domains, making their learned knowledge tightly coupled with domain-specific structural patterns, feature spaces, and feature semantics. Without cross-domain transferability, knowledge learned from one graph domain may therefore remain difficult to reuse in other application scenarios.

Cross-domain capability is also a fundamental capability toward **general-purpose graph foundation models (GFMs)**. Cross-domain graph learning aims to learn transferable graph knowledge from source domains and generalize it to different target domains. Advancing this capability can unlock the value of abundant yet fragmented graph data and move graph learning beyond domain-specific modeling toward broadly general models.

This repository organizes representative CDGL studies according to the graph-data-centric taxonomy proposed in our survey.

## Cross-domain Settings

We characterize CDGL settings along two complementary dimensions.

### Cross-domain Scale

Cross-domain scale describes the **domain scope** a method can accommodate and the **graph-data compatibility requirements** it imposes.

- **Limited CDGL**: source and target graph domains share directly compatible structural and feature spaces, so cross-domain transfer can be performed without explicit cross-space transformation.
- **Conditional CDGL**: source and target graph domains may have incompatible attributes or semantics, but can be transformed into a common representation space under predefined transformation conditions, shared schemas, or common semantic spaces.
- **Open CDGL**: source and target graph domains can be diverse and do not need to satisfy predefined structural- or feature-level compatibility conditions.

### Cross-domain Difficulty

Cross-domain difficulty describes the **knowledge gap between target domains and the knowledge available during training**.

- **Low-Difficulty CDGL**: the target domain is accessed during model training.
- **Moderate-Difficulty CDGL**: the target domain is unseen during training, but its domain category has been represented in the training domains.
- **High-Difficulty CDGL**: both the target domain and its domain category are unseen during training.

## Taxonomy

Our taxonomy is organized according to **what graph information is transferred across domains**, and is further refined according to **how that information is processed**.

```text
Cross-domain Graph Learning
├── Structure-oriented
│   ├── Generative
│   └── Contrastive
├── Feature-oriented
│   ├── In-space
│   └── Cross-space
│       ├── Remapping
│       └── Augmenting
└── Mixture-oriented
    ├── Sequential Mixture
    └── Unified Mixture
        ├── Graph-based Unified
        └── Flatten-based Unified
```

## Table of Contents

- [Why is cross-domain graph learning important?](#why-is-cross-domain-graph-learning-important)
- [Cross-domain Settings](#cross-domain-settings)
  - [Cross-domain Scale](#cross-domain-scale)
  - [Cross-domain Difficulty](#cross-domain-difficulty)
- [Taxonomy](#taxonomy)
- [Cross-domain Graph Learning Papers](#cross-domain-graph-learning-papers)
  - [1. Structure-oriented](#1-structure-oriented)
    - [1.1 Generative](#11-generative)
    - [1.2 Contrastive](#12-contrastive)
  - [2. Feature-oriented](#2-feature-oriented)
    - [2.1 In-space](#21-in-space)
    - [2.2 Cross-space](#22-cross-space)
      - [2.2.1 Remapping to a New Feature Space](#221-remapping-to-a-new-feature-space)
      - [2.2.2 Augmenting Representations](#222-augmenting-representations)
  - [3. Mixture-oriented](#3-mixture-oriented)
    - [3.1 Sequential Mixture](#31-sequential-mixture)
    - [3.2 Unified Mixture](#32-unified-mixture)
      - [3.2.1 Graph-based Unified](#321-graph-based-unified)
      - [3.2.2 Flatten-based Unified](#322-flatten-based-unified)
- [Contributing](#contributing)
- [Citation](#citation)

## Cross-domain Graph Learning Papers

### 1. Structure-oriented

Structure-oriented CDGL uses transferable **structural information** as the main basis for cross-domain learning. Existing methods mainly capture structural commonalities by generating or reformulating graph structures, or by comparing existing structural patterns.

#### 1.1 Generative

- **GraphControl: Adding Conditional Control to Universal Graph Pre-trained Models for Graph Domain Transfer Learning** — WWW 2024. [[Paper](https://doi.org/10.1145/3589334.3645439)] [[Code](https://github.com/wykk00/GraphControl)]
- **Exploring Task Unification in Graph Representation Learning via Generative Approach (GA2E)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2403.14340)]
- **OpenGraph: Towards Open Graph Foundation Models** — arXiv 2024. [[Paper](https://arxiv.org/abs/2403.01121)] [[Code](https://github.com/HKUDS/OpenGraph)]
- **Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models (UniAug)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2406.01899)] [[Code](https://github.com/WenzhuoTang/UniAug)]
- **GFT: Graph Foundation Model with Transferable Tree Vocabulary** — NeurIPS 2024. [[Paper](https://openreview.net/forum?id=0MXzbAv8xy)] [[Code](https://github.com/Zehong-Wang/GFT)]
- **Transferable Hypergraph Neural Networks via Spectral Similarity (HENN)** — LoG 2024. [[Paper](https://proceedings.mlr.press/v231/hayhoe24a.html)]
- **Towards a Universal Graph Structural Encoder (GFSE)** — arXiv 2025. [[Paper](https://arxiv.org/abs/2504.10917)] [[Code](https://github.com/Graph-and-Geometric-Learning/GFSE)]
- **GraphOracle: Efficient Fully-Inductive Knowledge Graph Reasoning via Relation-Dependency Graphs** — AAAI 2026. [[Paper](https://arxiv.org/abs/2505.11125)] [[Code](https://github.com/EnjunDu/GraphOracle)]

#### 1.2 Contrastive

- **GCC: Graph Contrastive Coding for Graph Neural Network Pre-Training** — KDD 2020. [[Paper](https://dl.acm.org/doi/abs/10.1145/3394486.3403168)] [[Code](https://github.com/THUDM/GCC)]
- **Pre-training Graph Neural Network for Cross Domain Recommendation (PCRec)** — CogMI 2021. [[Paper](https://arxiv.org/abs/2111.08268)] [[Code](https://github.com/THUDM/GCC)]
- **Non-IID Transfer Learning on Graphs (GRADE)** — AAAI 2023. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/26231/26003)]
- **Better with Less: A Data-Active Perspective on Pre-Training Graph Neural Networks (APT)** — NeurIPS 2023. [[Paper](https://arxiv.org/abs/2311.01038)] [[Code](https://github.com/galina0217/APT)]
- **Federated Learning on Non-IID Graphs via Structural Knowledge Sharing (FedStar)** — AAAI 2023. [[Paper](https://arxiv.org/abs/2211.13009)][[Code](https://github.com/yuetan031/FedStar)]
- **Boosting Graph Foundation Model from Structural Perspective (BooG)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2407.19941)]
- **ProCom: A Few-shot Targeted Community Detection Algorithm** — KDD 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671749)]
- **RiemannGFM: Learning a Graph Foundation Model from Riemannian Geometry** — WWW 2025. [[Paper](https://arxiv.org/abs/2502.03251)] [[Code](https://github.com/RiemannGraph/RiemannGFM)]

### 2. Feature-oriented

Feature-oriented CDGL focuses on learning transferable **feature-level representations** by identifying feature commonalities across graph domains. We divide these methods according to whether cross-domain feature dimensions are already compatible.

#### 2.1 In-space

In-space methods operate under compatible feature dimensions and mainly focus on aligning feature semantics across domains.

- **Zero-shot Transfer Learning within a Heterogeneous Graph via Knowledge Transfer Networks (KTN)** — NeurIPS 2022. [[Paper](https://arxiv.org/abs/2203.02018)] [[Code](https://github.com/minjiyoon/KTN)]
- **Universal Prompt Tuning for Graph Neural Networks (GPF-plus)** — NeurIPS 2023. [[Paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/a4a1ee071ce0fe63b83bce507c9dc4d7-Abstract-Conference.html)]
- **Negative as Positive: Enhancing Out-of-distribution Generalization for Graph Contrastive Learning (NaP)** — SIGIR 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3626772.3657927)]
- **MultiGPrompt for Multi-Task Pre-Training and Prompting on Graphs** — WWW 2024. [[Paper](https://dl.acm.org/doi/10.1145/3589334.3645423)] [[Code](https://github.com/Nashchou/MultiGPrompt)]
- **RELIEF: Reinforcement Learning Empowered Graph Feature Prompt Tuning** — KDD 2025. [[Paper](https://doi.org/10.1145/3690624.3709252)] [[Code](https://github.com/JasonZhujp/RELIEF)]
- **DAGPrompT: Pushing the Limits of Graph Prompting with a Distribution-aware Graph Prompt Tuning Approach** — WWW 2025. [[Paper](https://arxiv.org/abs/2501.15142)] [[Code](https://github.com/Cqkkkkkk/DAGPrompT)]
- **Cross-Domain Graph Anomaly Detection via Test-Time Training with Homophily-Guided Self-Supervision (GADT3)** — TMLR 2025. [[Paper](https://openreview.net/forum?id=sB3LqdOlNb)] [[Code](https://github.com/delaramphf/GADT3-Algorithm)]

#### 2.2 Cross-space

Cross-space methods further handle incompatible feature dimensions and semantics by mapping heterogeneous graph features into compatible representation spaces.

##### 2.2.1 Remapping to a New Feature Space

- **One for All: Towards Training One Graph Model for All Classification Tasks (OFA)** — ICLR 2024. [[Paper](https://openreview.net/pdf?id=4IT2pgc9v6)] [[Code](https://github.com/LechengKong/OneForAll)]
- **GraphAlign: Pretraining One Graph Neural Network on Multiple Graphs via Feature Alignment** — arXiv 2024. [[Paper](https://arxiv.org/abs/2406.02953)] [[Code](https://github.com/THUDM/GraphAlign)]
- **ZeroG: Investigating Cross-dataset Zero-shot Transferability in Graphs** — KDD 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671982)]

##### 2.2.2 Augmenting Representations

- **Towards Cross-domain Few-shot Graph Anomaly Detection (CDFS-GAD)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2410.08629)]
- **Cross-Context Backdoor Attacks against Graph Prompt Learning (CrossBA)** — KDD 2024. [[Paper](ttps://dl.acm.org/doi/10.1145/3637528.3671956)][[Code](https://github.com/xtLyu/CrossBA)]
- **Zero-shot Generalist Graph Anomaly Detection with Unified Neighborhood Prompts (UNPrompt)** — IJCAI 2025. [[Paper](https://arxiv.org/abs/2410.14886)] [[Code](https://github.com/mala-lab/UNPrompt)]
- **Uniform Graph Pre-training and Prompting for Transferable Recommendation (ProRec)** — ACM TOIS 2025.
- **Graph Prompt Clustering (GPC)** — IEEE TPAMI 2025. [[Paper](https://ieeexplore.ieee.org/document/10935718)]

### 3. Mixture-oriented

Mixture-oriented CDGL jointly transfers **structural and feature information**. According to how the two types of information are integrated, we divide these methods into Sequential Mixture and Unified Mixture.

#### 3.1 Sequential Mixture

Sequential Mixture methods process structural and feature information in separate stages. The order may be structure-to-feature or feature-to-structure.

- **PTGB: Pre-Train Graph Neural Networks for Brain Network Analysis** — CHIL 2023. [[Paper](https://arxiv.org/abs/2305.14376)] [[Code](https://github.com/Owen-Yang-18/BrainNN-PreTrain)]
- **Semi-supervised Domain Adaptation in Graph Transfer Learning (SDGA)** — IJCAI 2023. [[Paper](https://arxiv.org/abs/2309.10773)]
- **Source Free Unsupervised Graph Domain Adaptation (SOGA)** — WSDM 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3616855.3635802)] [[Code](https://github.com/HaitaoMao/SOGA)]
- **A Pure Transformer Pretraining Framework on Text-attributed Graphs (GSPT)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2406.13873)] [[Code](https://github.com/SongYYYY/GSPT)]
- **ARC: A Generalist Graph Anomaly Detector with In-Context Learning** — arXiv 2024. [[Paper](https://arxiv.org/abs/2405.16771)]
- **UniGraph: Learning a Cross-Domain Graph Foundation Model from Natural Language** — arXiv 2024. [[Paper](https://arxiv.org/abs/2402.13630)] [[Code](https://github.com/yf-he/UniGraph)]
- **AnyGraph: Graph Foundation Model in the Wild** — Findings of ACL 2026. [[Paper](https://aclanthology.org/2026.findings-acl.44/)] [[Code](https://github.com/hkuds/anygraph)]
- **GraphLoRA: Structure-aware Contrastive Low-rank Adaptation for Cross-Graph Transfer Learning** — arXiv 2024. [[Paper](https://arxiv.org/abs/2409.16670)]
- **SAMGPT: Text-free Graph Foundation Model for Multi-domain Pre-training and Cross-domain Adaptation** — WWW 2025. [[Paper](https://arxiv.org/abs/2502.05424)] [[Code](https://github.com/blue-soda/SAMGPT)]
- **Multi-Domain Graph Foundation Models: Robust Knowledge Transfer via Topology Alignment (MDGFM)** — ICML 2025. [[Paper](https://arxiv.org/abs/2502.02017)]
- **HyperTrans: Efficient Hypergraph-Driven Cross-Domain Pattern Transfer in Image Anomaly Detection** — IJCAI 2025. [[Paper](https://www.ijcai.org/proceedings/2025/267)][[Code](https://github.com/raRn0y/HyperTrans)]
- **MLDGG: Meta-Learning for Domain Generalization on Graphs** — KDD 2025. [[Paper](https://doi.org/10.1145/3690624.3709188)]

#### 3.2 Unified Mixture

Unified Mixture methods jointly process structural and feature information within a unified framework.

##### 3.2.1 Graph-based Unified

Graph-based Unified methods preserve the graph form and jointly encode structural and feature information through graph-oriented models and graph message passing.

- **Domain Adaptation Network Based on Hypergraph Regularized Denoising Autoencoder (DAHDA)** — Artificial Intelligence Review 2019. [[Paper](https://link.springer.com/article/10.1007/s10462-017-9576-0)]
- **Unsupervised Domain Adaptive Graph Convolutional Networks (UDA-GCN)** — WWW 2020. [[Paper](https://dl.acm.org/doi/abs/10.1145/3366423.3380219)]
- **Domain Adaptive Classification on Heterogeneous Information Networks (MuSDAC)** — IJCAI 2020. [[Paper](https://www.ijcai.org/proceedings/2020/196)]
- **DA-GCN: A Domain-aware Attentive Graph Convolution Network for Shared-account Cross-domain Sequential Recommendation** — IJCAI 2021. [[Paper](https://www.ijcai.org/proceedings/2021/0342.pdf)]
- **Cross-Domain Graph Anomaly Detection (COMMANDER)** — IEEE TNNLS 2021. [[Paper](https://ieeexplore.ieee.org/document/9556511)]
- **Federated Graph Classification over Non-IID Graphs (GCFL)** — NeurIPS 2021. [[Paper](https://proceedings.neurips.cc/paper_files/paper/2021/file/9c6947bd95ae487c81d4e19d3ed8cd6f-Paper.pdf)]
- **Cross-domain Few-shot Graph Classification (CDGEncoder)** — AAAI 2022. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/20642/20401)]
- **Few-shot Heterogeneous Graph Learning via Cross-domain Knowledge Transfer (CrossHG-Meta)** — KDD 2022. [[Paper](https://doi.org/10.1145/3534678.3539431)]
- **Data-Efficient Brain Connectome Analysis via Multi-Task Meta-Learning (METABrainC)** — KDD 2022. [[Paper](https://doi.org/10.1145/3534678.3542680)]
- **Contrastive Cross-domain Recommendation in Matching (CCDR)** — KDD 2022. [[Paper](https://doi.org/10.1145/3534678.3539125)]
- **Graph Adaptive Semantic Transfer for Cross-domain Sentiment Classification (GAST)** — SIGIR 2022. [[Paper](https://doi.org/10.1145/3477495.3531984)]
- **Decoupled Hyperbolic Graph Attention Network for Cross-domain Named Entity Recognition (DH-GAT)** — SIGIR 2023. [[Paper](https://doi.org/10.1145/3539618.3591662)]
- **Cross-Domain Graph Anomaly Detection via Anomaly-Aware Contrastive Alignment (ACT)** — AAAI 2023. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/25591/25363)]
- **ALEX: Towards Effective Graph Transfer Learning with Noisy Labels** — ACM MM 2023. [[Paper](https://doi.org/10.1145/3581783.3612026)]
- **Cross-domain Few-shot Graph Classification with a Reinforced Task Coordinator (CDTC)** — AAAI 2023. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25615/25387)]
- **Domain-Adaptive Graph Attention-Supervised Network for Cross-Network Edge Classification (DGASN)** — IEEE TNNLS 2023. [[Paper](https://ieeexplore.ieee.org/document/10246298/)]
- **Beyond the Overlapping Users: Cross-Domain Recommendation via Adaptive Anchor Link Learning (ALCDR)** — SIGIR 2023. [[Paper](https://doi.org/10.1145/3539618.3591642)]
- **Contrastive Graph Prompt-Tuning for Cross-Domain Recommendation (PGPRec)** — ACM TOIS 2023. [[Paper](https://dl.acm.org/doi/10.1145/3618298)]
- **Prompt-Based Spatio-Temporal Graph Transfer Learning (STGP)** — CIKM 2024. [[Paper](https://dl.acm.org/doi/10.1145/3627673.3679554)]
- **All in One and One for All: A Simple yet Effective Method towards Cross-domain Graph Pretraining (GCOPE)** — KDD 2024. [[Paper](https://arxiv.org/abs/2402.09834)] [[Code](https://github.com/cshhzhao/GCOPE)]
- **Text-Free Multi-domain Graph Pre-training: Toward Graph Foundation Models (MDGPT)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2405.13934)]
- **UniGLM: Training One Unified Language Model for Text-Attributed Graphs** — arXiv 2024. [[Paper](https://arxiv.org/abs/2406.12052)]
- **One Model for One Graph: A New Perspective for Pretraining with Cross-domain Graphs (OMOG)** — arXiv 2024. [[Paper](https://arxiv.org/abs/2412.00315)]
- **Enhancing Cross-domain Link Prediction via Evolution Process Modeling (CrossLink)** — WWW 2025. [[Paper](https://arxiv.org/abs/2402.02168)]
- **Unified Graph Neural Networks Pre-training for Multi-domain Graphs (MDP-GNN)** — AAAI 2025. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/33325)]
- **UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs** — WWW 2025. [[Paper](https://dl.acm.org/doi/abs/10.1145/3696410.3714818)] [[Code](https://github.com/yf-he/UniGraph2)]
- **Towards Graph Foundation Models: Learning Generalities Across Graphs via Task-Trees (GIT)** — 2025. [[Paper](https://arxiv.org/abs/2412.16441)] [[Code](https://github.com/Zehong-Wang/GIT)]
- **Bridging Source and Target Domains via Link Prediction for Unsupervised Domain Adaptation on Graphs (CMPGNN)** — WSDM 2025. [[Paper](https://doi.org/10.1145/3701551.3703519)]
- **A Cross-domain Knowledge Tracing Model Based on Graph Optimal Transport (AEGOT-CDKT)** — World Wide Web 2025. [[Paper](https://link.springer.com/article/10.1007/s11280-024-01311-1)]
- **Heterogeneous Graph Transfer Learning for Category-aware Cross-Domain Sequential Recommendation (HGTL)** — WWW 2025. [[Paper](https://dl.acm.org/doi/10.1145/3696410.3714885)] [[Code](https://github.com/zitaozz/HGTL)]

##### 3.2.2 Flatten-based Unified

Flatten-based Unified methods convert graph structures and features into token sequences or other language-compatible representations and use LLMs/VLMs as unified predictors.

- **GIMLET: A Unified Graph-Text Model for Instruction-Based Molecule Zero-Shot Learning** — NeurIPS 2023. [[Paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/129033c7c08be683059559e8d6bfd460-Abstract-Conference.html)]
- **GraphTranslator: Aligning Graph Model to Large Language Model for Open-Ended Tasks** — WWW 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3589334.3645682)]
- **GraphGPT: Graph Instruction Tuning for Large Language Models** — SIGIR 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3626772.3657775)] [[Code](https://github.com/HKUDS/GraphGPT)]
- **GITA: Graph to Visual and Textual Integration for Vision-Language Graph Reasoning** — NeurIPS 2024.
- **InstructGraph: Boosting Large Language Models via Graph-Centric Instruction Tuning and Preference Alignment** — arXiv 2024. [[Paper](https://arxiv.org/abs/2402.08785)]
- **LLMs as Zero-shot Graph Learners: Alignment of GNN Representations with LLM Token Embeddings (TEA-GLM)** — NeurIPS 2024.
- **HiGPT: Heterogeneous Graph Language Model** — KDD 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671987)]
- **GraphWiz: An Instruction-Following Language Model for Graph Computational Problems** — KDD 2024. [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3672010)]
- **GOFA: A Generative One-For-All Model for Joint Graph Language Modeling** — ICLR 2025. [[Paper](https://openreview.net/forum?id=mIjblC9hfm)] [[Code](https://github.com/JiaruiFeng/GOFA)]
- **GraphCLIP: Enhancing Transferability in Graph Foundation Models for Text-Attributed Graphs** — WWW 2025. [[Paper](https://arxiv.org/abs/2410.10329)]

## Contributing
👍 Contributions to this repository are welcome! 

If you have come across relevant resources, feel free to open an issue or submit a pull request.

## Citation

If you find this repo helpful to you, please feel free to cite these works:

<!--
[Survey Paper](https://arxiv.org/abs/2311.16534)
```latex
@article{sun2023graph,
  title = {Graph Prompt Learning: A Comprehensive Survey and Beyond},
  author = {Sun, Xiangguo and Zhang, Jiawen and Wu, Xixi and Cheng, Hong and Xiong, Yun and Li, Jia},
  year = {2023},
  journal = {arXiv:2311.16534},
  eprint = {2311.16534},
  archiveprefix = {arxiv}
}
```
-->

Other Representative Works:

🔥 **All in One** A Representative GNN Prompting Framework
  ```latex
  @inproceedings{sun2023all,
    title={All in One: Multi-Task Prompting for Graph Neural Networks},
    author={Sun, Xiangguo and Cheng, Hong and Li, Jia and Liu, Bo and Guan, Jihong},
    booktitle={Proceedings of the 26th ACM SIGKDD international conference on knowledge discovery \& data mining (KDD'23)},
    year={2023},
    pages = {2120–2131},
    location = {Long Beach, CA, USA},
    isbn = {9798400701030},
    url = {https://doi.org/10.1145/3580305.3599256},
    doi = {10.1145/3580305.3599256}
  }
 ```

🔥 **All in One and One for All** A Cross-domain Graph Pre-training Framework
  ```latex
  @article{zhao2024all,
    title={All in One and One for All: A Simple yet Effective Method towards Cross-domain Graph Pretraining}, 
    author={Haihong Zhao and Aochuan Chen and Xiangguo Sun and Hong Cheng and Jia Li},
    year={2024},
    eprint={2402.09834},
    archivePrefix={arXiv}
  }
  ```

🔥 **ProG** A Graph Prompt Learning Benchmark (I am the co-first author, contributing to the primary writing and experimental evaluation, including the extension of GPPT and GPF-plus on both node and graph classification tasks.)
  ```latex
  @inproceedings{Neurips2024prog,
    title={ProG: A Graph Prompt Learning Benchmark},
    author={Chenyi Zi and Haihong Zhao and Xiangguo Sun and Yiqing Lin and Hong Cheng and Jia Li},
    booktitle={The Thirty-eight Conference on Neural Information Processing Systems Datasets and Benchmarks Track},
    year={2024},
    url={https://openreview.net/forum?id=wqo6xEMyk9}
  }
  ```
