# MGNN

## This is the code for our paper "Leveraging Brain Modularity Prior for Interpretable Representation Learning of fMRI"[arXiv](http://arxiv.org/abs/2306.14080)


##Cite as: arXiv:2306.14080 [q-bio.QM]  (or arXiv:2306.14080v1 [q-bio.QM] for this version)

https://arxiv.org/abs/2306.14080

## Abstract  

-  Resting-state functional magnetic resonance imaging (rs-fMRI) can reflect spontaneous neural activities in brain and is widely used for brain disorder analysis.Previous studies propose to extract fMRI representations through diverse machine/deep learning methods for subsequent analysis. But the learned features typically lack biological interpretability, which limits their clinical utility. From the view of graph theory, the brain exhibits a remarkable modular structure in spontaneous brain functional networks, with each module comprised of functionally interconnected brain regions-of-interest (ROIs). However, most existing learning-based methods for fMRI analysis fail to adequately utilize such brain modularity prior. In this paper, we propose a Brain Modularity-constrained dynamic Representation learning (BMR) framework for interpretable fMRI analysis, consisting of three major components: (1) dynamic graph construction, (2) dynamic graph learning via a novel modularity-constrained graph neural network (MGNN), (3) prediction and biomarker detection for interpretable fMRI analysis. Especially, three core neurocognitive modules (i.e., salience network, central executive network, and default mode network) are explicitly incorporated into the MGNN, encouraging the nodes/ROIs within the same module to share similar representations. To further enhance discriminative ability of learned features, we also encourage the MGNN to preserve the network topology of input graphs via a graph topology reconstruction constraint. Experimental results on 534 subjects with rs-fMRI scans from two datasets validate the effectiveness of the proposed method. The identified discriminative brain ROIs and functional connectivities can be regarded as potential fMRI biomarkers to aid in clinical diagnosis.


## Dependencies  

The framework needs the following dependencies:

```
torch~=1.13.0
numpy~=1.21.5
torch_scatter~=2.1.0+pt113cu117
scipy~=1.9.3
einops~=0.5.0
```


Many thanks to Dr Byung-Hoon Kim for sharing their project [STAGIN](https://github.com/egyptdj/stagin).
