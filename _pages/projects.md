---
layout: page
title: projects
permalink: /projects/
nav: true
---

<font size="+1"> <b> Towards Fast, Specialized Machine Learning Force Fields: Distilling Foundation Models via Energy Hessians
 </b></font>
The foundation model (FM) paradigm is transforming Machine Learning Force Fields (MLFFs), leveraging general-purpose representations and scalable training to perform a variety of computational chemistry tasks. Although MLFF FMs have begun to close the accuracy gap relative to first-principles methods, there is still a strong need for faster inference speed. Additionally, while research is increasingly focused on general-purpose models which transfer across chemical space, practitioners typically only study a small subset of systems at a given time. This underscores the need for fast, specialized MLFFs relevant to specific downstream applications, which preserve test-time physical soundness while maintaining train-time scalability. In this work, we introduce a method for transferring general-purpose representations from MLFF foundation models to smaller, faster MLFFs specialized to specific regions of chemical space. We formulate our approach as a knowledge distillation procedure, where the smaller "student" MLFF is trained to match the Hessians of the energy predictions of the "teacher" foundation model. Our specialized MLFFs can be up to 20 × faster than the original foundation model, while retaining, and in some cases exceeding, its performance and that of undistilled models. More broadly, our work suggests a new paradigm for MLFF development, in which foundation models are released along with smaller, specialized simulation "engines" for common chemical subsets.
<br>
With: Ishan Amin and Aditi Krishnapriyan at UC Berkeley.
<br>
[Paper - ICLR 2025](https://arxiv.org/abs/2501.09009){:target="\_blank"} | [Github](https://github.com/ASK-Berkeley/MLFF-distill){:target="\_blank"}


<font size="+1"> <b> Stability-Aware Training of Machine Learning Force Fields with Differentiable Boltzmann Estimators
 </b></font>
Machine learning force fields (MLFFs) are an attractive alternative to ab-initio methods for molecular dynamics (MD) simulations. However, they can produce unstable simulations, limiting their ability to model phenomena occurring over longer timescales and compromising the quality of estimated observables. To address these challenges, we present Stability-Aware Boltzmann Estimator (StABlE) Training, a multi-modal training procedure which leverages joint supervision from reference quantum-mechanical calculations and system observables. StABlE Training iteratively runs many MD simulations in parallel to seek out unstable regions, and corrects the instabilities via supervision with a reference observable. We achieve efficient end-to-end automatic differentiation through MD simulations using our Boltzmann Estimator, a generalization of implicit differentiation techniques to a broader class of stochastic algorithms. Unlike existing techniques based on active learning, our approach requires no additional ab-initio energy and forces calculations to correct instabilities. We demonstrate our methodology across organic molecules, tetrapeptides, and condensed phase systems, using three modern MLFF architectures. StABlE-trained models achieve significant improvements in simulation stability, data efficiency, and agreement with reference observables.
<br>
With: Ishan Amin, Fabian Pedregosa, and Aditi Krishnapriyan at UC Berkeley.
<br>
[Paper - TMLR 2025](https://arxiv.org/abs/2402.13984){:target="\_blank"} | [Github](https://github.com/ASK-Berkeley/StABlE-Training/){:target="\_blank"}

<font size="+1"> <b> Multigrid Neural Operators for Efficient Deep Learning on Large Fields in the Physical Sciences </b></font>
Data arising in many physical science applications contain hundreds of variables at high spatial resolution. Often, a single such image cannot be loaded onto a GPU, making machine learning workflows unfeasible. I developed a multigrid neural network which performs memory-efficient training and inference by training on multiscale crops while preserving long-range spatial interactions. This paved the way for FourCastNet, which was a state-of-the-art weather prediction model at the time of development. <br>
With: Jaideep Pathak, Ashesh Chattopadhyay, Zongyi Li, Mustafa Mustafa, Kamyar Azizzadenesheli and Karthik Kasinath at [Lawrence Berkeley National Laboratory](https://www.lbl.gov/){:target="\_blank"}. Advisor: [Anima Anandkumar](http://tensorlab.cms.caltech.edu/users/anima/){:target="\_blank"} 
<br>
[Paper](https://arxiv.org/abs/2202.11214){:target="\_blank"} | [Github](https://github.com/NVlabs/FourCastNet){:target="\_blank"}



<font size="+1"> <b> Spatial and Temporal Super-Resolution of Global Climate Models using Deep Learning </b></font>
Physics-based global climate simulations are computationally expensive and limited to low spatial and temporal resolutions, making it difficult to predict and track highly localized extreme weather phenomena. We used deep learning (SRGAN, CycleGAN, Super Slo Mo, and other methods) to increase the resolution of global climate models in both space and time. For this work we won the Best Paper Award and $20,000 prize at the [ProjectX](https://www.projectx2020.com/){:target="\_blank"} research competition
<br>
With: Eric Chen, Ziwei Tian, Anh Huan Tran, Yue Yao, Zhizhuo Zhou. Advisor: [Sindhu Kutty](https://www.cs.swarthmore.edu/~sindhu/){:target="\_blank"}
<br>
[Paper - UofT AI Conference 2021](https://drive.google.com/file/d/1cbwTb7DNe0vRZiN9hg53W5MZdRbXJqsg/view?usp=sharing){:target="\_blank"} | [GitHub](https://github.com/ericch99/bayes-and-blue){:target="\_blank"}
<br>


<font size="+1"> <b>Machine Learning for Immune Cell Profiling</b> </font>
Time-of-flight mass cytometry - [CyTOF](https://www.fluidigm.com/products/helios){:target="\_blank"}- enables high-throughput, deep phenotyping of immune cells at the single-cell level. I worked on ML techniques like clustering (GMM, hierarchical), dimensionality reduction (tSNE, PCA), and supervised deep learning (CNN, graph networks) to analyze immunological datasets. 
<br>
With: Brett Hill, Andrew Zak, Christine Yee, Luke Bugada. Advisor: [Fei Wen](http://cheresearch.engin.umich.edu/wen/){:target="\_blank"}
<br>
[Paper - JCI Insight 2024](https://pmc.ncbi.nlm.nih.gov/articles/PMC11383363/){:target="\_blank"}
<br>


<font size="+1"> <b>Multi-stage Fault Warning for Large Electric Grids using Anomaly Detection and Machine Learning</b> </font>
In this work, we proposed a multi-stage early warning system for electric grid fault detection, classification, subgroup discovery, and visualization. We leveraged both supervised and unsupervised ML methods as well as dimensionality reduction.
<br>
With: [Ernest Fokoue](https://www.rit.edu/directory/epfeqa-ernest-fokoue){:target="\_blank"}
<br>
[Paper - Mathematics for Applications 2020](http://ma.fme.vutbr.cz/archiv/8_2/ma_8_2_2_raja_fokoue_final.pdf){:target="\_blank"}





