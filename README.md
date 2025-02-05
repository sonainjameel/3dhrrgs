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




