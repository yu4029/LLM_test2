FROM amd64/ubuntu:20.04

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y git python3 python3-pip

FROM python:3.12
RUN pip3 install tokenizers>=0.13.2 prompt_toolkit numpy torch
RUN pip install rwkv transformers accelerate sentencepiece colorama
RUN pip install llama-cpp-python
RUN pip install einops bitsandbytes scipy

WORKDIR /root
