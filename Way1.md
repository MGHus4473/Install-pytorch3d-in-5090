I solved this issue on Windows 11 with an RTX 5070 Ti and WSL2.

First, install CUDA 12.8.
Then, install PyTorch using:
```
pip3 install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/cu128
```
Finally, clone the PyTorch3D source code and install it:
```
git clone https://github.com/facebookresearch/pytorch3d.git
cd pytorch3d
pip install -e .
```
