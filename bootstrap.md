## Ortho-plane Inference with Bootstrapping

### Overview

Ortho-plane inference is used for isotropic voxel EM data. Independent stacks of
2D predictions on XY, XZ, and YZ planes are averaged into a final 3D segmentation.
This can introduce artifacts like "cross-hatching" that typically would require manual
cleanup. Training a separate DL model with weak supervision (bootstrapping) on the ortho-plane inference
output can significantly improve 3D segmentation quality.

### Resources

- [boostrap2.5d](https://github.com/volume-em/bootstrap2.5d): Source code to run
orthoplane inference and weakly supervised training.

- [APEER module](https://www.apeer.com/app/modules/Bootstrap-2.5D-Trainer/e897d3e7-e05b-4eaa-a2c4-a9c9498d0dff): An
APEER module to easily apply this technique on any 3D binary segmentation task.

- [Colab notebook](https://colab.research.google.com/github/volume-em/bootstrap2.5d/blob/master/colab_notebook.ipynb): Google
Colab notebook that demonstrates an application for mitochondria and lysosomes.

### Citing this work

If you find any of these resources useful in your work, please cite:

```bibtex
@article{conrad_lee_narayan_2020,
  title={Enforcing Prediction Consistency Across Orthogonal Planes Significantly Improves Segmentation of FIB-SEM Image Volumes by 2D Neural Networks.},
  volume={26},
  DOI={10.1017/S143192762002053X},
  number={S2},
  journal={Microscopy and Microanalysis},
  publisher={Cambridge University Press},
  author={Conrad, Ryan and Lee, Hanbin and Narayan, Kedar},
  year={2020},
  pages={2128–2130}
}
```
