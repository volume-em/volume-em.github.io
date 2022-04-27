## The CEM Dataset

### Overview

The CEM dataset is an unlabeled collection of 2D cellular EM images designed for
self-supervised learning algorithms. Gathered from over 2 PB of data, it is heterogeneous
enough to capture a significant variety of organisms, tissues, and imaging methods.

### Resources

- [CEM1.5M](https://www.ebi.ac.uk/empiar/EMPIAR-10592/): The newest release of the
dataset with 1.5 million images.

- [CEM500K](https://www.ebi.ac.uk/empiar/EMPIAR-10592/): The first release of the
dataset with 500 thousand images.

- [CEM1.5M Pre-trained Weights](https://zenodo.org/record/6453160#.YmlzHS-cbTQ): PyTorch weights for a ResNet50 model pre-trained on CEM1.5M
using the SwAV algorithm.

- [CEM500K Pre-trained Weights](https://zenodo.org/record/6453140#.Ymlxoy-cbTQ): PyTorch weights for a ResNet50 model pre-trained on CEM500K
using the MoCoV2 algorithm.

- [CEM Patch Filtering Weights](https://zenodo.org/record/6458015#.Yml1ci-cbTQ): PyTorch weights for a ResNet34 model trained on 12,000
EM images that were labeled as "informative" or "uninformative". Used to curate patches in the CEM dataset.

- [cem-dataset](https://github.com/volume-em/cem-dataset): Source code to reproduce
the results of our paper; scripts to preprocess, standardize, and curate 2D and 3D
EM datasets; scripts to download and prepare the [EMOrganelles](https://paperswithcode.com/sota/electron-microscopy-image-segmentation-on-1?p=cem500k-a-large-scale-heterogeneous-unlabeled)
benchmark datasets (including the All Mitochondria benchmark established in the CEM500K paper)
and SnakeMake files to evaluate pre-trained models on the benchmarks. Plus, explanatory
Jupyter Notebooks.

### Citing this work

If you find any of these resources useful in your work, please cite:

```bibtex
@article {Conrad2021,
	author = {Conrad, Ryan and Narayan, Kedar},
	doi = {10.7554/eLife.65894},
	issn = {2050-084X},
	journal = {eLife},
	month = {apr},
	title = {{CEM500K, a large-scale heterogeneous unlabeled cellular electron microscopy image dataset for deep learning}},
	url = {https://elifesciences.org/articles/65894},
	volume = {10},
	year = {2021}
}
```
