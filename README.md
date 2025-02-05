# 3D Human Reconstruction and Relighting using 3D Gaussian Splatting from Single View Input
``
conda create --name triGau python=3.11
``

``
conda activate triGau
``

``
git clone https://github.com/VAST-AI-Research/TriplaneGaussian.git
``

``
pip install torch
``

``
pip install torchvision
``

``
pip install torchaudio
``

or 

``
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
``

``
cd TriplaneGaussian
``

Make sure CUDA is working

``
nvcc --version
``

``
nvidia-smi
``

``
pip install cupy-cuda12x
``

``
pip install -r requirements.txt
``

``
pip install git+https://github.com/graphdeco-inria/diff-gaussian-rasterization.git
``

``
pip install torch-scatter
``

``
python setup.py install
``

``
pip install fvcore iopath
``

``
pip install 'git+https://github.com/facebookresearch/pytorch3d.git'
``

``
mkdir checkpoints
cd checkpoints
wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth
``

``
cd ..
from huggingface_hub import hf_hub_download
python from huggingface_hub import hf_hub_download
``

``
pip install onnxruntime-gpu
``

``
sudo apt-get install -y tensorrt
``

``
python infer.py --config config.yaml data.image_list=[example_images/a_pikachu_with_smily_face.webp] --image_preprocess
``



