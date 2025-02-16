# Triplane Gaussian

The implementation is based on [TriplaneGaussian](https://github.com/VAST-AI-Research/TriplaneGaussian) and leverages PyTorch and related deep learning frameworks.

## 📌 Installation  

### 1️⃣ Set up a Conda environment  

```bash
conda create --name triGau python=3.11
conda activate triGau
```

### 2️⃣ Clone the repository  

```bash
git clone https://github.com/VAST-AI-Research/TriplaneGaussian.git
cd TriplaneGaussian
```

### 3️⃣ Install PyTorch  

Choose the appropriate installation method based on your GPU setup:

#### ✅ Default Installation  
```bash
pip install torch torchvision torchaudio
```

#### ✅ Installation with CUDA Support (for NVIDIA GPUs)  
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
```

### 4️⃣ Verify CUDA Installation  

Ensure that CUDA is properly installed and accessible:  

```bash
nvcc --version
nvidia-smi
```

If CUDA is installed, you should see your GPU details listed.

### 5️⃣ Install Dependencies  

```bash
pip install cupy-cuda12x
pip install -r requirements.txt
pip install git+https://github.com/graphdeco-inria/diff-gaussian-rasterization.git
pip install torch-scatter
pip install fvcore iopath
pip install 'git+https://github.com/facebookresearch/pytorch3d.git'
```

### 6️⃣ Compile PointNet2 Operations  

```bash
cd tgs/models/snowflake/pointnet2_ops_lib
python setup.py install
cd ../../../..
```

### 7️⃣ Download Checkpoints  

```bash
mkdir checkpoints
cd checkpoints
wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth
cd ..
```

### 8️⃣ Install Additional Packages  

```bash
pip install onnxruntime-gpu
sudo apt-get install -y tensorrt
```

Note: There can be an issue with onnxruntime-gpu library after installation, however, the output can still be obtained. 

### 9️⃣ Hugging Face Model Download  

```python
from huggingface_hub import hf_hub_download
python from huggingface_hub import hf_hub_download
```


## 🚀 Running Inference  

To run inference with an example image:

```bash
python infer.py --config config.yaml data.image_list=[example_images/a_pikachu_with_smily_face.webp] --image_preprocess
```

## 🔗 References  

- [TriplaneGaussian Repository](https://github.com/VAST-AI-Research/TriplaneGaussian)  
- [Facebook Research - PyTorch3D](https://github.com/facebookresearch/pytorch3d)  
- [GraphDeco Inria - Diff Gaussian Rasterization](https://github.com/graphdeco-inria/diff-gaussian-rasterization)  

