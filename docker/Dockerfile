FROM nvcr.io/nvidia/cuda:11.8.0-cudnn8-devel-ubuntu22.04

RUN apt-get update \ 
    && apt-get install -y git git-lfs curl python3 python3-pip ffmpeg \
    && curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | bash \
    && git lfs install \
    && rm cuda-keyring_1.0-1_all.deb \
    && ln -s /usr/bin/python3 /usr/bin/python \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install --no-cache-dir torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118

RUN git clone --depth 1 https://huggingface.co/spaces/chiliktam/OpenVoiceV2 \
    && cd OpenVoiceV2 && pip3 install --no-cache-dir -r requirements.txt \
    && pip3 install --no-cache-dir gradio==3.48.0

WORKDIR /OpenVoiceV2