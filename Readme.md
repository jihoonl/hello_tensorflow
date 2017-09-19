# Hello Tensorflow

## Installation

### Install Nvidia docker

* Ref: [https://github.com/NVIDIA/nvidia-docker](https://github.com/NVIDIA/nvidia-docker)
```
# Install nvidia-docker and nvidia-docker-plugin
wget -P /tmp https://github.com/NVIDIA/nvidia-docker/releases/download/v1.0.1/nvidia-docker_1.0.1-1_amd64.deb
sudo dpkg -i /tmp/nvidia-docker*.deb && rm /tmp/nvidia-docker*.deb

# Test nvidia-smi
nvidia-docker run --rm nvidia/cuda nvidia-smi
```

## Command

```
> nvidia-docker run -v <path to cloned repo>:/notebooks -it -p 8888:8888 gcr.io/tensorflow/tensorflow:latest-gpu
```
