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
   In **KDD'2024**, [[Paper](https://arxiv.org/pdf/2402.09834)]  [[Code](https://github.com/cshhzhao/GCOPE)].

2. **UniGraph Learning a Cross-Domain Graph Foundation Model From Natural Language**.
   In **arXiv**, [[Paper](https://arxiv.org/pdf/2402.13630)].

3. **Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models**.
   In **arXiv**, [[Paper](https://arxiv.org/pdf/2406.01899)].

4. **Cross-domain few-shot graph classification**.
   In **AAAI 2022**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/20642/20401)].

5. **Cross-domain few-shot graph classification with a reinforced task coordinator**.
   In **AAAI 2023**, [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25615/25387)].
6. **Pending to extend...**


## Others
Pending to extend.

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
