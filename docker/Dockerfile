FROM nvidia/cuda:12.0.1-cudnn8-devel-ubuntu22.04 AS runtime-origin

RUN apt-get update && \
    apt-get install -y \
    software-properties-common;

RUN apt-get update && \
    apt-get install -y \
    python3-pip \
    git \
    wget;

RUN pip3 install notebook pycuda matplotlib torch torchvision torchaudio;
