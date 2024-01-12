# Docker
Dockerfiles and compose for bunch of stuff
## Installation
1. Install Docker to desktop (on win11 machine)
2. Install WSL
3. From command prompt: `wsl.exe --upgrade`
4. `mkdir -p /datadrive/docker`
# Nvidia
Combine WSL with RAPIDS and pytorch
## Base
Just to test WSL & Docker play nice  
From base path (in WSL): `docker compose up`
## Jupyter
jupyter lab server with nvidia container
1. `mkdir -p /datadrive/docker/cuda_pytorch_jupyter`
2. From cuda_pytorch_jupyter path (in WSL):
    -   `./build.sh`
    -   `docker compose up`
3. Run `test_cuda.ipynb` on remote server to test CUDA and all goodies are working
All files accessed by the container are at `/datadrive/docker/cuda_pytorch_jupyter`