# 23.02 Requires CUDA 12.0, NVIDIA Driver 525 or later
FROM nvcr.io/nvidia/pytorch:23.02-py3

ARG DEBIAN_FRONTEND=noninteractive

WORKDIR /app
COPY requirements.txt /app/requirements.txt
SHELL ["/bin/bash", "-c"]

RUN pip install -r requirements.txt
