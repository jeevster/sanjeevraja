---
layout: page
title: research
permalink: /research/
nav: true
---
<font size="+1"> <b> AquaGen: Scaling generative models to molecular dynamics precision on thousands of atoms
 </b></font>
AquaGen is the first all-atom, explicit solvent, periodic-boundary-condition-aware generative model that produces molecular configurations from the Boltzmann distribution at a fraction of the cost of molecular dynamics (MD). This is in contrast with existing generative models that remove degrees of freedom by operating on coarse-grained, vacuum, or implicit solvent systems. Operating at this resolution allows for post-processing through force field energy evaluations and MD simulations, and enables the prediction of relevant properties in a gray-box manner (as ensemble averages of potential energy evaluations over generated samples). We demonstrate the utility of this paradigm on absolute hydration free energy (AHFE), producing estimates 4-10x faster and with comparable accuracy to standard GPU-based MD. By generating uncorrelated samples from alchemical Boltzmann distributions, we create more accurate, interpretable, and refinable ensemble predictions with calibrated uncertainty estimates, unlike regression methods which are entirely black-box predictors. Our approach also yields predictable benefits from increasing train- and test-time compute, realized by scaling model size and generating more samples, respectively. We believe that this approach demonstrates the utility of high-resolution ensemble generation for free energy estimation, with future potential to replace MD in tasks such as the prediction of lipophilicity, membrane permeability, or absolute binding free energy (ABFE) -- whose grounding and interpretability may be critical for the development of new drugs and materials.
<br>
With: Emmanuel Bengio, Sanjeev Raja, Yui Tik Pang, Kerstin Klaeser, Cristian Gabellini, Nikhil Shenoy, Francesco Di Giovanni, Prudencio Tossou
<br>
[Paper](https://arxiv.org/abs/2607.03513v1){:target="\_blank"} | [Blog Post](https://substack.com/home/post/p-204039624){:target="\_blank"}


<font size="+1"> <b> Action-Minimization Meets Generative Modeling: Efficient Transition Path Sampling with the Onsager-Machlup Functional
 </b></font>
Transition path sampling (TPS), which involves finding probable paths connecting two points on an energy landscape, remains a challenge due to the complexity of real-world atomistic systems. Current machine learning approaches use expensive, task-specific, and data-free training procedures, limiting their ability to benefit from recent advances in atomistic machine learning, such as high-quality datasets and large-scale pre-trained models. In this work, we address TPS by interpreting candidate paths as trajectories sampled from stochastic dynamics induced by the learned score function of pre-trained generative models, specifically denoising diffusion and flow matching. Under these dynamics, finding high-likelihood transition paths becomes equivalent to minimizing the Onsager-Machlup (OM) action functional. This enables us to repurpose pre-trained generative models for TPS in a zero-shot manner, in contrast with bespoke, task-specific TPS models trained in previous work. We demonstrate our approach on varied molecular systems, obtaining diverse, physically realistic transition pathways and generalizing beyond the pre-trained model's original training dataset. Our method can be easily incorporated into new generative models, making it practically relevant as models continue to scale and improve with increased data availability.
<br>
With: Martin Sipka, Michael Psenka, Toby Kreiman, Michal Pavelka, and Aditi Krishnapriyan.
<br>
[Paper - ICML 2025](https://arxiv.org/abs/2504.18506){:target="\_blank"} | [Github](https://github.com/ASK-Berkeley/OM-TPS){:target="\_blank"}

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





