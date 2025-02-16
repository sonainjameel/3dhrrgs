# 3D Reconstruction and Relighting using 3D Gaussian Splatting from Single View Input

This repository provides a pipeline for 3D reconstruction and relighting using **3D Gaussian Splatting** from a single-view image. The implementation is based on [TriplaneGaussian](https://github.com/VAST-AI-Research/TriplaneGaussian) and [Relightable 3D Gaussian](https://github.com/NJU-3DV/Relightable3DGaussian). It leverages PyTorch and related deep-learning frameworks to achieve high-quality relighting and reconstruction.

## 📌 Installation

Follow the installation guides for each module:

- **[Triplane Gaussian Installation](../TriplaneGaussian/Readme.md)**: For single-view 3D reconstruction using Triplane Gaussian.
- **[Relightable 3D Gaussian Installation](./relightable_README.md)**: For real-time relighting using BRDF decomposition and ray tracing.

## 🚀 Running Inference

### Triplane Gaussian Reconstruction
```bash
python infer.py --config config.yaml data.image_list=[example_images/a_pikachu_with_smily_face.webp] --image_preprocess
```

### Relightable 3D Gaussian Rendering
```bash
python render.py --input_mesh input.obj --lighting_conditions config.yaml
```

## 🔗 References

- [TriplaneGaussian Repository](https://github.com/VAST-AI-Research/TriplaneGaussian)
- [Relightable 3D Gaussian Repository](https://github.com/NJU-3DV/Relightable3DGaussian)
- [Facebook Research - PyTorch3D](https://github.com/facebookresearch/pytorch3d)
- [GraphDeco Inria - Diff Gaussian Rasterization](https://github.com/graphdeco-inria/diff-gaussian-rasterization)

