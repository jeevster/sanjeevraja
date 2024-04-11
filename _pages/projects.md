---
layout: page
title: projects
permalink: /projects/
nav: true
---
<font size="+1"> <b> Stability-Aware Training of Neural Network Interatomic Potentials with Differentiable Boltzmann Estimators
 </b></font>
Neural network interatomic potentials (NNIPs) are an attractive alternative to ab-initio methods for molecular dynamics (MD) simulations. However, they can produce unstable simulations which sample unphysical states, limiting their usefulness for modeling phenomena occurring over longer timescales. To address these challenges, we present Stability-Aware Boltzmann Estimator (StABlE) Training, a multi-modal training procedure which combines conventional supervised training from quantum-mechanical energies and forces with reference system observables, to produce stable and accurate NNIPs. StABlE Training iteratively runs MD simulations to seek out unstable regions, and corrects the instabilities via supervision with a reference observable. The training procedure is enabled by the Boltzmann Estimator, which allows efficient computation of gradients required to train neural networks to system observables, and can detect both global and local instabilities. We demonstrate our methodology across organic molecules, tetrapeptides, and condensed phase systems, along with using three modern NNIP architectures. In all three cases, StABlE-trained models achieve significant improvements in simulation stability and recovery of structural and dynamic observables. In some cases, StABlE-trained models outperform conventional models trained on datasets 50 times larger. As a general framework applicable across NNIP architectures and systems, StABlE Training is a powerful tool for training stable and accurate NNIPs, particularly in the absence of large reference datasets. <br>
With: Ishan Amin, Fabian Pedregosa, and Aditi Krishnapriyan at UC Berkeley.
<br>
[Paper](https://arxiv.org/abs/2402.13984){:target="\_blank"} | [Github](https://github.com/ASK-Berkeley/StABlE-Training/){:target="\_blank"}

<font size="+1"> <b> Multigrid Neural Operators for Efficient Deep Learning on Large Fields in the Physical Sciences </b></font>
Data arising in many physical science applications contain hundreds of variables at high spatial resolution. Often, a single such image cannot be loaded onto a GPU, making machine learning workflows unfeasible. I developed a multigrid neural network which performs memory-efficient training and inference by training on multiscale crops while preserving long-range spatial interactions. I demonstrated applications in global weather forecasting and high-resolution fluid flow prediction. <br>
With: Jaideep Pathak, Ashesh Chattopadhyay, Zongyi Li, Mustafa Mustafa, Kamyar Azizzadenesheli and Karthik Kasinath at [Lawrence Berkeley National Laboratory](https://www.lbl.gov/){:target="\_blank"}. Advisor: [Anima Anandkumar](http://tensorlab.cms.caltech.edu/users/anima/){:target="\_blank"} 
<br>
[Paper](https://arxiv.org/abs/2202.11214){:target="\_blank"} | [Github](https://github.com/NVlabs/FourCastNet){:target="\_blank"}



<font size="+1"> <b> Spatial and Temporal Super-Resolution of Global Climate Models using Deep Learning </b></font>
Physics-based global climate simulations are computationally expensive and limited to low spatial and temporal resolutions, making it difficult to predict and track highly localized extreme weather phenomena. We used deep learning (SRGAN, CycleGAN, Super Slo Mo, and other methods) to increase the resolution of global climate models in both space and time. For this work we won the Best Paper Award and $20,000 prize at the [ProjectX](https://www.projectx2020.com/){:target="\_blank"} research competition
<br>
With: Eric Chen, Ziwei Tian, Anh Huan Tran, Yue Yao, Zhizhuo Zhou. Advisor: [Sindhu Kutty](https://www.cs.swarthmore.edu/~sindhu/){:target="\_blank"}
<br>
[Paper](https://drive.google.com/file/d/1cbwTb7DNe0vRZiN9hg53W5MZdRbXJqsg/view?usp=sharing){:target="\_blank"} | [GitHub](https://github.com/ericch99/bayes-and-blue){:target="\_blank"}
<br>

<font size="+1"> <b> Deep Semantic Segmentation of Silicon Carbide Wafer Scratches </b> </font>
I designed a deep segmentation pipeline in TensorFlow for scratch detection on silicon carbide wafers. At the heart of the pipeline is a fully convolutional network inspired by UNet, ResNet, and Inception architectures. Along the way, I curated a benchmark dataset of ground truth wafer segmentation maps pooled from multiple chemical engineers and domain experts.
<br>
With: [Matthew Conrad](https://www.linkedin.com/in/matthewdavidconrad/){:target="\_blank"} at [Wolfspeed](https://www.wolfspeed.com/){:target="\_blank"}
<br>
I can't share materials due to the proprietary nature of this work
<br>

<font size="+1"> <b>Machine Learning for Immune Cell Profiling</b> </font>
Time-of-flight mass cytometry - [CyTOF](https://www.fluidigm.com/products/helios){:target="\_blank"}- enables high-throughput, deep phenotyping of immune cells at the single-cell level. I work on ML techniques like clustering (GMM, hierarchical), dimensionality reduction (tSNE, PCA), and supervised deep learning (CNN, graph networks) to analyze immunological datasets. Manuscripts currently under review.
<br>
With: Brett Hill, Andrew Zak, Christine Yee, Luke Bugada. Advisor: [Fei Wen](http://cheresearch.engin.umich.edu/wen/){:target="\_blank"}
<br>


<font size="+1"> <b>Multi-stage Fault Warning for Large Electric Grids using Anomaly Detection and Machine Learning</b> </font>
In this work, we proposed a multi-stage early warning system for electric grid fault detection, classification, subgroup discovery, and visualization. We leveraged both supervised and unsupervised ML methods as well as dimensionality reduction.
<br>
With: [Ernest Fokoue](https://www.rit.edu/directory/epfeqa-ernest-fokoue){:target="\_blank"}
<br>
[Paper](http://ma.fme.vutbr.cz/archiv/8_2/ma_8_2_2_raja_fokoue_final.pdf){:target="\_blank"}

<font size="+1"> <b>Computational Modeling of Waste Heat Recovery Systems for Internal Combustion Engines</b> </font>
Waste heat recovery (WHR) systems recover heat energy from vehicle exhaust in order to improve engine efficiency. In this work, we used the GT-Power modeling software to design a Rankine Cycle waste heat recovery system for application in internal combustion engines. We incorporated PID process control elements to ensure system stability at a wide range of operating conditions.
<br>
With: [Greg Hulbert](https://me.engin.umich.edu/people/faculty/greg-hulbert){:target="\_blank"} at UofM and [Chris Reid](https://www.linkedin.com/in/christopher-reid-57643610/){:target="\_blank"} at General Motors
<br>
I can't share materials due to the proprietary nature of this work.
<br>

<font size="+1"> <b>Statistical and Machine Learning Analysis of Homicides and Shootings in Rochester, NY </b></font>
We used gaussian mixture models, regression, and hypothesis testing to analyze historical crime data from Rochester, NY. For this work, we won 1st place in the 2018 Monroe County High School Data Analysis Competition.
<br>
With: Joyce Luo, Jeremy Nguyen, Zachary Yung
<br>
[Report](https://drive.google.com/file/d/1jvKaF2qBM_dsybzr1LE5V6hioJg5Cm_T/view){:target="\_blank"}







