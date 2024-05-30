FROM nvidia/cuda:11.1.1-cudnn8-devel-ubuntu20.04
#コメントアウト


RUN apt-get update -y && \
    DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    sudo \
    python3-dev \
    python3-pip \
    python3-wheel \
    python3-setuptools \
    nano \
    cifs-utils \
    libgl1-mesa-dev \
    libglib2.0-0 \
    && \
    rm -rf /var/lib/apt/lists/* /var/cache/apt/archives/*

RUN pip3 install torch==1.9.1+cu111 torchvision==0.10.1+cu111 -f https://download.pytorch.org/whl/torch_stable.html
RUN pip3 install --no-cache-dir \
                cython==0.29.24 \
                numpy==1.21.2 \
                tqdm==4.62.3 \
                pillow==8.3.2 \
                scipy==1.7.1 \
                joblib==1.0.1 \
		matplotlib==3.4.3 \
                scikit-learn==1.0 \
                scikit-image==0.18.3 \
                statsmodels==0.13.1 \
		opencv-python==4.5.1.48
		

