# hash:sha256:ce7f9f7c933e1ffb648c2ae5a9c42a84affe020fd383a29ed0f7f3697e43eb2a
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/jupyterlab:3.6.1-miniconda4.12.0-python3.9-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive
ARG GIT_ASKPASS
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    allensdk==2.16.2 \
    matplotlib==3.9.0 \
    numpy==1.6.1 \
    pandas==1.23.5 \
    scikit-learn==1.6.1
