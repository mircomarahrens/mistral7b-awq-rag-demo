# Retrieval-augmented generation with open-source large language models

## Prerequisites

The tested environment is

```bash
$ uname -a
Linux richardfeynman 5.15.133.1-microsoft-standard-WSL2 #1 SMP Thu Oct 5 21:02:42 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
```

```bash
$ cat /etc/lsb-release
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=22.04
DISTRIB_CODENAME=jammy
DISTRIB_DESCRIPTION="Ubuntu 22.04.3 LTS"
```

```bash
$ poetry --version
Poetry (version 1.5.1)
```

```bash
$ /usr/local/cuda/bin/nvcc --version
nvcc: NVIDIA (R) Cuda compiler driver
Copyright (c) 2005-2022 NVIDIA Corporation
Built on Wed_Sep_21_10:33:58_PDT_2022
Cuda compilation tools, release 11.8, V11.8.89
Build cuda_11.8.r11.8/compiler.31833905_0
```

```bash
$ nvidia-smi --query-gpu=gpu_name,memory.total --format=csv
name, memory.total [MiB]
NVIDIA GeForce RTX 3060, 12288 MiB
```

## Setup

Using [poetry](https://python-poetry.org/)

```bash
poetry install
```

or using the provided `requirements.txt` with [pip](https://pip.pypa.io/en/stable/)

```bash
pip install -r requirements.txt
```

## Presentation

Each of the notebooks are representable as slides in a browser using, i.e. for `notebook/00_introduction.ipynb`, run

```bash
jupyter nbconvert notebook/00_introduction.ipynb --to slides --post serve
```

This will open a browser window with the notebook rendered as slides.

## References

- <https://learn.microsoft.com/en-us/azure/search/retrieval-augmented-generation-overview>
- <https://python.langchain.com/docs/expression_language/cookbook/retrieval>
- original model: <https://huggingface.co/mistralai/Mistral-7B-v0.1>
- quantized model: <https://huggingface.co/TheBloke/Mistral-7B-v0.1-AWQ>
- vllm: <https://docs.vllm.ai/>
- autoawq:
  - <https://docs.vllm.ai/en/latest/quantization/auto_awq.html>
  - <https://github.com/casper-hansen/AutoAWQ>
- <https://huggingface.co/TheBloke/SciPhi-Self-RAG-Mistral-7B-32k-AWQ>
- <https://github.com/oobabooga/text-generation-webui>
- <https://medium.com/@thakermadhav/build-your-own-rag-with-mistral-7b-and-langchain-97d0c92fa146>
- <https://redis.io/docs/get-started/vector-database/>
- <https://github.com/facebookresearch/faiss/wiki>
- <https://github.com/TimDettmers/bitsandbytes>
- <https://www.youtube.com/watch?v=IxrlHAJtqKE>
- <https://research.ibm.com/blog/retrieval-augmented-generation-RAG>
- NLP Course: <https://huggingface.co/learn/nlp-course/chapter1/1>
- Quantization: <https://huggingface.co/docs/transformers/main_classes/quantization>
- Tokenizer: <https://huggingface.co/docs/transformers/main_classes/tokenizer>
- <https://python.langchain.com/docs/integrations/vectorstores/faiss>
- <https://python.langchain.com/docs/modules/data_connection/document_loaders/pdf>
- <https://openai.com/blog/introducing-text-and-code-embeddings>

## Papers

- RAG: <https://arxiv.org/abs/2005.11401v4>
- MistralAI paper: <https://arxiv.org/pdf/2310.06825.pdf>
- OpenAI Text embeddings paper: <https://arxiv.org/abs/2201.10005>
- Similarity search: <https://arxiv.org/abs/1702.08734>
