# YOLO-ResTinyECG

install pytorch
conda create --name ALEX_3 python=3.9 -y
conda activate ALEX_3
conda install -c conda-forge cudatoolkit=11.3
conda install -c anaconda cudnn
conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch

#
https://pytorch.org/get-started/previous-versions/
# R5 3600 + RTX 2070s # CUDA 10.1
pip install torch==1.7.0+cu101 torchvision==0.8.1+cu101 torchaudio==0.7.0 -f https://download.pytorch.org/whl/torch_stable.html
or --> torchvision==0.8.1+cu101 fit torch==1.8.1
# CUDA 10.2
pip install torch==1.10.1+cu102 torchvision==0.11.2+cu102 torchaudio==0.10.1 -f https://download.pytorch.org/whl/cu102/torch_stable.html

# in PS42 GTX1050Q # CUDA 10.2
conda install pytorch==1.7.1 torchvision==0.8.2 torchaudio==0.7.2 cudatoolkit=10.2 -c pytorch

# Check torch GPU:
nvidia-smi
nvcc --version
$ python
>>> import torch
>>> torch.cuda.is_available()
True
>>> torch.cuda.get_device_name(0)
