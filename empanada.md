## Empanada and MitoNet

### Overview

<img src="images/empanada_logo.png" alt="empanada logo" width="400px"/>
<img src="images/mitonet_logo.png" alt="mitonet logo" width="400px"/>

**EMPANADA** stands for **EM** **Pan**optic **A**ny **D**imension **A**nnotation. It's a library
developed to efficiently train and deploy deep learning models for the panoptic
segmentation of large 2D and 3D EM images. We trained a general model called _MitoNet_
to automatically segment mitochondrial instances, using empanada and a highly heterogeneous dataset of labeled mitochondria.
_MitoNet_ is currently available for use in [napari](https://napari.org) with the **empanada-napari**
plugin -- though we're open to supporting it's use in other software platforms.

### Resources

- [empanada](https://github.com/volume-em/empanada.git): Source code for the empanada library.
[Documentation is here](https://empanada.readthedocs.io/en/latest/index.html).

- [empanada-napari](https://github.com/volume-em/empanada-napari): Source code for the empanada-napari plugin.
[Documentation is here](https://empanada.readthedocs.io/en/latest/empanada-napari.html).

- [CEM1.5M](https://www.ebi.ac.uk/empiar/EMPIAR-10592/): An unlabeled dataset of 1.5 million
EM images of cells. Used for self-supervised pre-training and selecting heterogenous image data
to annotate for segmentation model training.

- [CEM1.5M Pre-trained Weights](https://zenodo.org/record/6453160#.YmlzHS-cbTQ): PyTorch weights for a ResNet50 model pre-trained on CEM1.5M
using the SwAV algorithm.

- [CEM-MitoLab](https://www.ebi.ac.uk/empiar/EMPIAR-10592/): A dataset of ~22,000 images
containing over 135,000 individually labeled mitochondria. This is the dataset we used
to train _MitoNet_.

- [MitoNet models](https://zenodo.org/record/6327742#.YmltqS-cbTQ): Model definition
and weights as PyTorch scripted modules (includes optimized GPU and CPU versions).

- [Benchmark datasets](https://www.ebi.ac.uk/empiar/EMPIAR-10982/): Six benchmark volumes of
instance segmented mitochondria from diverse volume EM datasets.

### Citing this work

If you find any of these resources useful in your work, please cite:

```bibtex
@article {Conrad2022.03.17.484806,
	author = {Conrad, Ryan and Narayan, Kedar},
	title = {Instance segmentation of mitochondria in electron microscopy images with a generalist deep learning model},
	elocation-id = {2022.03.17.484806},
	year = {2022},
	doi = {10.1101/2022.03.17.484806},
	publisher = {Cold Spring Harbor Laboratory},
	URL = {https://www.biorxiv.org/content/early/2022/03/18/2022.03.17.484806},
	eprint = {https://www.biorxiv.org/content/early/2022/03/18/2022.03.17.484806.full.pdf},
	journal = {bioRxiv}
}
```
