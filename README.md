<h1 align="center"> Awesome-Cross-Domain-Graph-Learning</h2>
<h5 align="center">A collection of AWESOME things about performing cross-domain learning on Graphs. Our survey has been published on https://arxiv.org/abs/2503.11086. </h5>

<h5 align="center">
  
![Awesome](https://awesome.re/badge.svg)   ![GitHub stars](https://img.shields.io/github/stars/cshhzhao/Awesome-Cross-Domain-Graph-Learning.svg)

</h5>

## Why are the cross-domain learning on graphs important?
Recently, Large Language Models (LLMs) have demonstrated powerful cross-domain capabilities, attracting a large number of researchers. Although cross-domain graph learning has always been an important research direction, existing works on tackling cross-domain tasks are not as effective as LLMs. Inspired by the powerful cross-domain abilities of LLMs, cross-domain graph learning has once again become a focal point of attention. This is also a critical issue that must be resolved before truly proposing graph foundation models.

This repo aims to provide a curated list of research papers that explore cross-domain learning on graphs. 
<!--
 **It is based on our Survey Paper: [Graph Prompt Learning: A Comprehensive Survey and Beyond](https://arxiv.org/abs/2311.16534)**. -->
We will try to make this list updated frequently. If you find any error or any missed paper, please don't hesitate to open issues or pull requests.🌹

## Table of Contents

- [Why are the cross-domain learning on graphs important?](#why-are-the-cross-domain-learning-on-graphs-important)
- [Table of Contents](#table-of-contents)
- [Cross-domain Graph Learning](#cross-domain-graph-learning)
  - [Structure-oriented](#structure-oriented)
    - [Structure Generation](#structure-generation)
    - [Structure Contrast](#structure-contrast)
  - [Feature-oriented](#feature-oriented)
    - [Dimension Align](#dimension-align)
    - [Dimension Misalign](#dimension-misalign)
  - [Mixture-oriented](#mixture-oriented)
    - [Sequential Mixture](#sequential-mixture)
    - [Unified Mixture](#unified-mixture)
      - [Graph-based](#graph-based)
      - [Flatten-based](#flatten-based)
- [Contributing](#contributing)
- [Citation](#citation)
  


## Cross-domain Graph Learning Papers

## Structure-oriented

### Structure Generation
1. **GraphControl: Adding Conditional Control to Universal Graph Pre-trained Models for Graph Domain Transfer Learning**. In **WWW 2024**, [[Paper](https://doi.org/10.1145/3589334.3645439)][[Code](https://github.com/wykk00/GraphControl)]
2. **Exploring Task Unification in Graph Representation Learning via Generative Approach**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2403.14340)].
3. **OpenGraph: Towards Open Graph Foundation Models**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2403.01121)][[Code](https://github.com/HKUDS/OpenGraph)].
4. **Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.01899)] [[Code](https://github.com/WenzhuoTang/UniAug)].
5. **GFT: Graph Foundation Model with Transferable Tree Vocabulary**. In **NeurIPS 2024**, [[Paper](https://openreview.net/forum?id=0MXzbAv8xy)].[[Code](https://github.com/Zehong-Wang/GFT)].
6. **Towards A Universal Graph Structural Encoder**. In **arXiv 2025**, [[Paper](https://arxiv.org/pdf/2504.10917)].[[Code](https://github.com/Graph-and-Geometric-Learning/GFSE)].


### Structure Contrast
1. **Graph few-shot learning via knowledge transfer**. In **AAAI 2020**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/6142/5998)].
2. **Gcc: Graph contrastive coding for graph neural network pre-training**. In **KDD 2020**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3394486.3403168)][[Code](https://github.com/THUDM/GCC)].
3. **Pre-training Graph Neural Network for Cross Domain Recommendation**. In **CogMI 2021**, [[Paper](https://arxiv.org/abs/2405.13934)].
4. **Better with Less: A Data-Active Perspective on Pre-Training Graph Neural Networks**. In **NeurIPS 2023**, [[Paper](https://arxiv.org/abs/2311.01038)][[Code](https://github.com/galina0217/APT)].
5. **ProCom: A Few-shot Targeted Community Detection Algorithm**. In **KDD 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671749)].
6. **Non-IID Transfer Learning on Graphs**. In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/26231/26003)].
7. **Boosting Graph Foundation Model from Structural Perspective**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2407.19941)].
8. **RiemannGFM: Learning a Graph Foundation Model from Riemannian Geometry**. In **WWW 2025**, , [[Paper](https://arxiv.org/abs/2502.03251)].[[Code](https://github.com/RiemannGraph/RiemannGFM)].

## Feature-oriented
   
### Dimension Align
1. **Zero-shot Transfer Learning within a Heterogeneous Graph via Knowledge Transfer Networks**. In **NeurIPS 2022**, [[Paper](https://arxiv.org/abs/2203.02018)] [[Code](https://github.com/minjiyoon/KTN)].
2. **Negative as Positive: Enhancing Out-of-distribution Generalization for Graph Contrastive Learning**. In **SIGIR 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3626772.3657927)].
3. **Universal prompt tuning for graph neural networks**. In **NeurIPS 2023**, [[Paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/a4a1ee071ce0fe63b83bce507c9dc4d7-Abstract-Conference.html)].
4. **Relief: Reinforcement learning empowered graph feature prompt tuning**. In **SIGKDD 2025**, [[Paper](https://doi.org/10.1145/3690624.3709252)][[Code](https://github.com/JasonZhujp/RELIEF)].
5. **Cross-Domain Graph Anomaly Detection via Test-Time Training with Homophily-Guided Self-Supervision**. In **TMLR 2025**, [[Paper](https://openreview.net/forum?id=sB3LqdOlNb)][[Code](https://github.com/delaramphf/GADT3-Algorithm)].
### Dimension Misalign
1. **One for all: Towards training one graph model for all classification tasks**. In **ICLR 2024**, [[Paper](https://openreview.net/pdf?id=4IT2pgc9v6)][[Code](https://github.com/LechengKong/OneForAll)].
2. **GraphAlign: Pretraining One Graph Neural Network on Multiple Graphs via Feature Alignment**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.02953)] [[Code](https://github.com/THUDM/GraphAlign)].
3. **Towards Cross-domain Few-shot Graph Anomaly Detection**. In **ICDM 2024**, [[Paper](https://arxiv.org/abs/2410.08629)].
4. **Zerog: Investigating cross-dataset zero-shot transferability in graphs**. In **SIGKDD 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671982)].
5. **DAGPrompT: Pushing the Limits of Graph Prompting with a Distribution-aware Graph Prompt Tuning Approach**. In **WWW 2025**, [[Paper](https://arxiv.org/abs/2501.15142)] [[Code](https://github.com/Cqkkkkkk/DAGPrompT)].
6. **Zero-shot Generalist Graph Anomaly Detection with Unified Neighborhood Prompts**. In **IJCAI 2025**, [[Paper](https://arxiv.org/abs/2410.14886)] [[Code](https://github.com/mala-lab/UNPrompt)].
## Mixture-oriented

### Sequential Mixture
1. **PTGB: Pre-Train Graph Neural Networks for Brain Network Analysis**. In **CHIL 2023**, [[Paper](https://arxiv.org/abs/2305.14376)] [[Code](https://github.com/Owen-Yang-18/BrainNN-PreTrain)].
2. **Semi-supervised domain adaptation in graph transfer learning**. In **IJCAI 2023**, [[Paper](https://arxiv.org/abs/2309.10773)].
3. **Harnessing explanations: Llm-to-lm interpreter for enhanced text-attributed graph representation learning**. In **ICLR 2024**, [[Paper](https://arxiv.org/abs/2305.19523)].
4. **Source Free Unsupervised Graph Domain Adaptation**. In **WSDM 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3616855.3635802)][[Code](https://github.com/HaitaoMao/SOGA)].
5. **A Pure Transformer Pretraining Framework on Text-attributed Graphs**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.13873)] [[Code](https://github.com/SongYYYY/GSPT)].
6. **ARC: A Generalist Graph Anomaly Detector with In-Context Learning**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2405.16771)].
7. **UniGraph: Learning a Unified Cross-Domain Foundation Model for Text-Attributed Graphs**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2402.13630)] [[Code](https://github.com/yf-he/UniGraph)].
8. **AnyGraph: Graph Foundation Model in the Wild**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2408.10700)].
9. **Graphlora: Structure-aware contrastive low-rank adaptation for cross-graph transfer learning**. In **SIGKDD 2025**, [[Paper](https://arxiv.org/abs/2409.16670)].
10. **SAMGPT: Text-free Graph Foundation Model for Multi-domain Pre-training and Cross-domain Adaptation**, In **WWW 2025**, [[Paper](https://arxiv.org/abs/2502.05424)] [[Code](https://github.com/blue-soda/SAMGPT)].
11. **Multi-Domain Graph Foundation Models: Robust Knowledge Transfer via Topology Alignment**, In **ICML 2025**, [[Paper](https://arxiv.org/abs/2502.02017)]
12. **MLDGG: Meta-Learning for Domain Generalization on Graphs**. In **KDD 2025**,[[Paper](https://doi.org/10.1145/3690624.3709188)]

### Unified Mixture
#### GNN-based
1. **Unsupervised domain adaptive graph convolutional networks**. In **WWW 2020**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3366423.3380219)].
2. **DA-GCN: A Domain-aware Attentive Graph Convolution Network for Shared-account Cross-domain Sequential Recommendation**. In **IJCAI 2021**, [[Paper](https://www.ijcai.org/proceedings/2021/0342.pdf)].
3. **Cross-Domain Graph Anomaly Detection**.In **TNNLS 2021**, [[Paper](https://ieeexplore.ieee.org/document/9556511)].
4. **Federated Graph Classification over Non-IID Graphs**. In **NeurIPS 2021**, [[Paper](https://proceedings.neurips.cc/paper_files/paper/2021/file/9c6947bd95ae487c81d4e19d3ed8cd6f-Paper.pdf)].
5. **Cross-domain few-shot graph classification**. In **AAAI 2022**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/20642/20401)].
6. **Few-shot Heterogeneous Graph Learning via Cross-domain Knowledge Transfer**. In **KDD 2022**, [[Paper](https://doi.org/10.1145/3534678.3539431)].
7. **Data-Efficient Brain Connectome Analysis via Multi-Task Meta-Learning**. In **KDD 2022**, [[Paper](https://doi.org/10.1145/3534678.3542680)].
8. **Contrastive Cross-domain Recommendation in Matching**. In **KDD 2022**, [[Paper](https://doi.org/10.1145/3534678.3539125)].
9. **Graph Adaptive Semantic Transfer for Cross-domain Sentiment Classification**. In **SIGIR 2022**, [[Paper](https://doi.org/10.1145/3477495.3531984)].
10. **Decoupled Hyperbolic Graph Attention Network for Cross-domain Named Entity Recognition**. In **SIGIR 2023**, [[Paper](https://doi.org/10.1145/3539618.3591662)].
11. **ALEX: Towards Effective Graph Transfer Learning with Noisy Labels**. In **MM 2023**, [[Paper](https://doi.org/10.1145/3581783.3612026)].
12. **Cross-Domain Graph Anomaly Detection via Anomaly-Aware Contrastive Alignment**. In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/25591/25363)].
13. **Cross-domain few-shot graph classification with a reinforced task coordinator**. In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25615/25387)].
14. **Domain-adaptive graph attention-supervised network for cross-network edge classification**. In **TNNLS 2023**, [[Paper]([https://ojs.aaai.org/index.php/AAAI/article/view/25615/25387](https://ieeexplore.ieee.org/abstract/document/10246298?casa_token=C38uj2h0crwAAAAA:xEBiar5-4MqVuv861aJs4xy95JyUG8IHvbtbg0qzs-Xg312-Ob2LSpuD_4Ulgc4HaH0jJ79GmaXGNYc))].
15. **Prompt-Based Spatio-Temporal Graph Transfer Learning**. In **CIKM 2024**, [[Paper](https://dl.acm.org/doi/10.1145/3627673.3679554)].
16. **Beyond the overlapping users: Cross-domain recommendation via adaptive anchor link learning**. In **SIGIR 2023**, [[Paper](https://doi.org/10.1145/3539618.3591642)].
17. **Contrastive graph prompt-tuning for cross-domain recommendation**. In **ACM Transactions on Information Systems 2023**, [[Paper](https://dl.acm.org/doi/10.1145/3627673.3679554))].
18. **All in One and One for All: A Simple yet Effective Method towards Cross-domain Graph Pretraining**. In **KDD'2024**, [[Paper](https://arxiv.org/abs/2402.09834)]  [[Code](https://github.com/cshhzhao/GCOPE)].
19. **Text-Free Multi-domain Graph Pre-training: Toward Graph Foundation Models**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2405.13934)].
20. **UniGLM: Training One Unified Language Model for Text-Attributed Graphs**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.12052)].
21. **Enhancing Cross-domain Link Prediction via Evolution Process Modeling**. In **WWW 2025**, [[Paper](https://arxiv.org/abs/2402.02168)].
22.  **Unified Graph Neural Networks Pre-training for Multi-domain Graphs**, In **AAAI 2025**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/33325)]
23. **Unigraph2: Learning a unified embedding space to bind multimodal graphs**. In **WWW 2025**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3696410.3714818)] [[Code](https://github.com/yf-he/UniGraph2)].
24. **Towards Graph Foundation Models: Learning Generalities Across Graphs via Task-Trees**. In **arXiv 2025**, [[Paper](https://arxiv.org/abs/2412.16441)] [[Code](https://github.com/Zehong-Wang/GIT)].
25. **A cross-domain knowledge tracing model based on graph optimal transport**. In **World Wide Web 2025**,[[Paper](https://link.springer.com/article/10.1007/s11280-024-01311-1)]
26. **Bridging Source and Target Domains via Link Prediction for Unsupervised Domain Adaptation on Graphs**. In **WSDM 2025**,[[Paper](https://doi.org/10.1145/3701551.3703519)]

#### Flatten-based
1. **Gimlet: A unified graph-text model for instruction-based molecule zero-shot learning**. In **NeurIPS 2023**, [[Paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/129033c7c08be683059559e8d6bfd460-Abstract-Conference.html)].
2. **Graphtranslator: Aligning graph model to large language model for open-ended tasks**. In **WWW 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3589334.3645682)]
3. **GraphGPT: Graph Instruction Tuning for Large Language Models**. In **SIGIR 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3626772.3657775)]  [[Code](https://github.com/HKUDS/GraphGPT)].
4. **Gita: Graph to visual and textual integration for vision-language graph reasoning**. In **NeurIPS 2024**, [[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/00295cede6e1600d344b5cd6d9fd4640-Abstract-Conference.html)].
5. **Instructgraph: Boosting large language models via graph-centric instruction tuning and preference alignment**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2402.08785)].
6. **LLMs as Zero-shot Graph Learners: Alignment of GNN Representations with LLM Token Embeddings**. In **NeurIPS 2024**, [[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0b77d3a82b59e9d9899370b378087faf-Abstract-Conference.html)].
7. **GOFA: A Generative One-For-All Model for Joint Graph Language Modeling**. In **Neurips 2024**, [[Paper](https://arxiv.org/abs/2407.09709)].
8. **Higpt: Heterogeneous graph language model**. In **KDD 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671987)].
9. **Graphwiz: An instruction-following language model for graph computational problems**. In **KDD 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3672010)].
10. **Graphclip: Enhancing transferability in graph foundation models for text-attributed graphs**. In **WWW 2025**, [[Paper](https://arxiv.org/abs/2410.10329)].
11. **One Model for One Graph: A New Perspective for Pretraining with Cross-domain Graphs**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2412.00315)].

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
