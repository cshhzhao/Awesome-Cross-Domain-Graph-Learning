<h1 align="center"> Awesome-Cross-Domain-Graph-Learning</h2>
<h5 align="center">A collection of AWESOME things about performing cross-domain learning on Graphs.</h5>

<h5 align="center">
  
![Awesome](https://awesome.re/badge.svg)   ![GitHub stars](https://img.shields.io/github/stars/cshhzhao/Awesome-Cross-Domain-Graph-Learning.svg)

</h5>

## Why are the cross-domain learning on graphs important?
Recently, Large Language Models (LLMs) have demonstrated powerful cross-domain capabilities, attracting a large number of researchers. Although cross-domain graph learning has always been an important research direction, existing works on tackling cross-domain tasks are not as effective as LLMs. Inspired by the powerful cross-domain abilities of LLMs, cross-domain graph learning has once again become a focal point of attention. This is also a critical issue that must be resolved before truly proposing graph foundation models.

This repo aims to provide a curated list of research papers that explore the cross-domain learning on graphs. 
<!--
 **It is based on our Survey Paper: [Graph Prompt Learning: A Comprehensive Survey and Beyond](https://arxiv.org/abs/2311.16534)**. -->
We will try to make this list updated frequently. If you found any error or any missed paper, please don't hesitate to open issues or pull requests.🌹

## Table of Contents

- [Why are the cross-domain learning on graphs important?](#why-are-the-cross-domain-learning-on-graphs-important)
- [Table of Contents](#table-of-contents)
- [Cross-domain Graph Learning Papers](#cross-domain-graph-learning-papers)
- [Others](#others)
- [Contributing](#contributing)
- [Citation](#citation)
  


## Cross-domain Graph Learning Papers

Summary of existing representative works on cross-domain graph learning. 

<!-- 先罗列收集文章，然后对这些文章进行分类，参考孙博和宇涵他们的文章 -->
1. **All in One and One for All: A Simple yet Effective Method towards Cross-domain Graph Pretraining**.
   In **KDD'2024**, [[Paper](https://arxiv.org/abs/2402.09834)]  [[Code](https://github.com/cshhzhao/GCOPE)].

2. **UniGraph: Learning a Unified Cross-Domain Foundation Model for Text-Attributed Graphs**.
   In **arXiv**, [[Paper](https://arxiv.org/abs/2402.13630)].

3. **Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models**.
   In **arXiv**, [[Paper](https://arxiv.org/abs/2406.01899)].

4. **Cross-domain few-shot graph classification**.
   In **AAAI 2022**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/20642/20401)].

5. **Cross-domain few-shot graph classification with a reinforced task coordinator**.
   In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25615/25387)].
6. **Cross-Context Backdoor Attacks against Graph Prompt Learning**. In **KDD 2024**, [[Paper](https://doi.org/10.1145/3637528.3671956)].
7. **Federated Learning on Non-IID Graphs via Structural Knowledge Sharing**. In **AAAI 2023**, [[Paper](https://doi.org/10.1609/aaai.v37i8.26187)].
8. **Adversarial Graph Representation Adaptation for Cross-Domain Facial Expression Recognition**. In **MM 2020**, [[Paper](https://doi.org/10.1145/3394171.3413822)].
9. **OpenGraph: Towards Open Graph Foundation Models**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2403.01121)].
10. **GraphControl: Adding Conditional Control to Universal Graph Pre-trained Models for Graph Domain Transfer Learning**. In **WWW 2024**, [[Paper](https://doi.org/10.1145/3589334.3645439)].
11. **Gcc: Graph contrastive coding for graph neural network pre-training**. In **KDD 2020**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3394486.3403168)].
12. **GraphGPT: Graph Instruction Tuning for Large Language Models**. In **SIGIR 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3626772.3657775)].
13. **One for all: Towards training one graph model for all classification tasks**. In **ICLR 2024**, [[Paper](https://openreview.net/pdf?id=4IT2pgc9v6)].
14. **LLMs as Zero-shot Graph Learners: Alignment of GNN Representations with LLM Token Embeddings**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2408.14512)].
15. **PTGB: Pre-Train Graph Neural Networks for Brain Network Analysis**. In **CHIL 2023**, [[Paper](https://arxiv.org/abs/2305.14376)] [[Code](https://github.com/Owen-Yang-18/BrainNN-PreTrain)].
16. **MultiGPrompt for Multi-Task Pre-Training and Prompting on Graphs**. In **WWW 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3589334.3645423)].
17. **A Pure Transformer Pretraining Framework on Text-attributed Graphs**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.13873)] [[Code](https://github.com/SongYYYY/GSPT)].
18. **ProCom: A Few-shot Targeted Community Detection Algorithm**. In **KDD 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671749)].
19. **Semi-supervised Domain Adaptation in Graph Transfer Learning**. In **IJCAI 2023**, [[Paper](https://doi.org/10.24963/ijcai.2023/253)].
20. **Negative as Positive: Enhancing Out-of-distribution Generalization for Graph Contrastive Learning**. In **SIGIR 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3626772.3657927)].
21. **Source Free Graph Unsupervised Domain Adaptation**. In **WSDM 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3616855.3635802)].
22. **Graph few-shot learning via knowledge transfer**. In **AAAI 2020**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/6142/5998)].
23. **Graph Machine Learning in the Era of Large Language Models (LLMs)**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2404.14928)].
24. **GraphAlign: Pretraining One Graph Neural Network on Multiple Graphs via Feature Alignment**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.02953)] [[Code](https://github.com/THUDM/GraphAlign)].
25. **Better with Less: A Data-Active Perspective on Pre-Training Graph Neural Networks**. In **NeurIPS 2023**, [[Paper](https://arxiv.org/abs/2311.01038)].
26. **Exploring Task Unification in Graph Representation Learning via Generative Approach**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2403.14340)].
27. **Zero-shot Transfer Learning within a Heterogeneous Graph via Knowledge Transfer Networks**. In **NeurIPS 2022**, [[Paper](https://arxiv.org/abs/2203.02018)] [[Code](https://github.com/minjiyoon/KTN)].
28. **Privacy-preserving Cross-domain Recommendation with Federated Graph Learning**. In **ACM TIS 2024**, [[Paper](https://dl.acm.org/doi/abs/10.1145/3653448)].
29. **Few-shot Heterogeneous Graph Learning via Cross-domain Knowledge Transfer**. In **KDD 2022**, [[Paper](https://doi.org/10.1145/3534678.3539431)].
30. **Learning Representations of Inactive Users: A Cross Domain Approach with Graph Neural Networks**. In **CIKM 2021**, [[Paper](https://doi.org/10.1145/3459637.3482131)].
31. **Contrastive Cross-domain Recommendation in Matching**. In **KDD 2022**, [[Paper](https://doi.org/10.1145/3534678.3539125)].
32. **Cross Domain Recommendation via Bi-directional Transfer
Graph Collaborative Filtering Networks**. In **CIKM 2020**, [[Paper](https://doi.org/10.1145/3340531.3412012)].
33. **Cross-Domain Graph Anomaly Detection via Anomaly-Aware Contrastive Alignment**. In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/25591/25363)].
34. **DA-GCN: A Domain-aware Attentive Graph Convolution Network for Shared-account Cross-domain Sequential Recommendation**. In **IJCAI 2021**, [[Paper](https://www.ijcai.org/proceedings/2021/0342.pdf)].
35. **Cross-Domain Aspect Extraction using Transformers Augmented with Knowledge Graphs**. In **CIKM 2022**, [[Paper](https://doi.org/10.1145/3511808.3557275)].
36. **Decoupled Hyperbolic Graph Attention Network for Cross-domain Named Entity Recognition**. In **SIGIR 2023**, [[Paper](https://doi.org/10.1145/3539618.3591662)].
37. **One Graph Model for Cross-domain Dynamic Link Prediction**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2402.02168)].
38. **Graph Signal Processing for Cross-Domain Recommendation**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2407.12374)].
39. **One for All, All for One: Learning and Transferring User Embeddings for Cross-Domain Recommendation**. In **WSDM 2023**, [[Paper](https://doi.org/10.1145/3539597.3570379)].
40. **Non-IID Transfer Learning on Graphs**. In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/26231/26003)].
41. **Unsupervised Domain Adaptive Graph Convolutional Network**. In **WWW 2020**, [[Paper](https://doi.org/10.1145/3366423.3380219)].
42. **Contrastive Graph Prompt-tuning for Cross-domain Recommendation**. In **ACM TIS 2023**, [[Paper](https://doi.org/10.1145/3618298)].
43. **Graph Adaptive Semantic Transfer for Cross-domain Sentiment Classification**. In **SIGIR 2022**, [[Paper](https://doi.org/10.1145/3477495.3531984)].
44. **Beyond the overlapping users: Cross-domain recommendation via adaptive anchor link learning**. In **SIGIR 2023**, [[Paper](https://doi.org/10.1145/3539618.3591642)].
45. **HiGPT: Heterogeneous Graph Language Model**. In **KDD 2024**, [[Paper](https://doi.org/10.1145/3637528.3671987)].
46. **Boosting Graph Foundation Model from Structural Perspective**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2407.19941)].
47. **UniGLM: Training One Unified Language Model for Text-Attributed Graphs**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2406.12052)].
48. **ARC: A Generalist Graph Anomaly Detector with In-Context Learning**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2405.16771)].
49. **Prompt-Enhanced Spatio-Temporal Graph Transfer Learning**. In **arXiv 2024**, [[Paper](https://arxiv.org/abs/2405.12452)].
50. **Domain-adaptive Graph Attention-supervised Network for Cross-network Edge Classification**. In **TNNLS 2023**, [[Paper](https://doi.org/10.1109/TNNLS.2023.3309632)].
51. **Data-Efficient Brain Connectome Analysis via Multi-Task Meta-Learning**. In **KDD 2022**, [[Paper](https://doi.org/10.1145/3534678.3542680)].
52. **Federated Graph Classification over Non-IID Graphs**. In **NeurIPS 2021**, [[Paper](https://proceedings.neurips.cc/paper_files/paper/2021/file/9c6947bd95ae487c81d4e19d3ed8cd6f-Paper.pdf)].
53. **Graph Learning Regularization and Transfer Learning
for Few-Shot Event Detection**. In **SIGIR 2021**, [[Paper](https://doi.org/10.1145/3404835.3463054)].
54. **ALEX: Towards Effective Graph Transfer Learning with Noisy Labels**. In **MM 2023**, [[Paper](https://doi.org/10.1145/3581783.3612026)].
55. **Adaptive Transfer Learning on Graph Neural Networks**. In **KDD 2021**, [[Paper](https://doi.org/10.1145/3447548.3467450)].
56. **Pending to extend...**


## Others
Pending to extend...

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
