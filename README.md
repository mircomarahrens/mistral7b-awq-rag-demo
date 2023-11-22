# Demo about retrieval-augmented generation with quantized open-source large language models

... or me learning LLMs.

- original model: <https://huggingface.co/mistralai/Mistral-7B-v0.1>
- quantized model: <https://huggingface.co/TheBloke/Mistral-7B-v0.1-AWQ>
- vllm: <https://docs.vllm.ai/>
- autoawq:
    - <https://docs.vllm.ai/en/latest/quantization/auto_awq.html>
    - <https://github.com/casper-hansen/AutoAWQ>

## To evaluate

- <https://huggingface.co/TheBloke/SciPhi-Self-RAG-Mistral-7B-32k-AWQ>
- <https://github.com/oobabooga/text-generation-webui>
- <https://medium.com/@thakermadhav/build-your-own-rag-with-mistral-7b-and-langchain-97d0c92fa146>

- <https://github.com/TimDettmers/bitsandbytes>
- <https://www.youtube.com/watch?v=IxrlHAJtqKE>

## References

- Quantization: <https://huggingface.co/docs/transformers/main_classes/quantization>
- Tokenizer: <https://huggingface.co/docs/transformers/main_classes/tokenizer>

## Paper

- MistralAI paper: <https://arxiv.org/pdf/2310.06825.pdf>
- OpenAI Text embeddings paper: <https://arxiv.org/abs/2201.10005>

## TODOs

- add bash script for model download
- add vector database
- add custom data (pdfs)
- add api server serving model
