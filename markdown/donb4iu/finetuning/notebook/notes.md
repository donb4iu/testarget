# Fine Tuning


## References

- [LLM Fine Tuning Mistral-7B for Text to SQL](https://www.kaggle.com/code/donbuddenbaum/llm-fine-tuning-mistral-7b-for-text-to-sql/edit)

- [![alt text](image.png) Hugging Face Models](https://huggingface.co/dbuddenbaum)

- [Fine-tune Gemma open models using multiple GPUs on GKE](https://cloud.google.com/kubernetes-engine/docs/tutorials/finetune-gemma-gpu)

- [Serve Gemma open models using GPUs on GKE with vLLM](https://cloud.google.com/kubernetes-engine/docs/tutorials/serve-gemma-gpu-vllm)

## Datasets

- [b-mc2/sql-create-context](https://huggingface.co/datasets/b-mc2/sql-create-context)

- [NousResearch/Hermes-2-Pro-Mistral-7B](https://huggingface.co/NousResearch/Hermes-2-Pro-Mistral-7B)

## Execution

### #(base) (11/08/24@19:26:21)dbuddenbaum@amd64-01:~$ source ~/Documents/cuda/bin/activate

### #(cuda) (base) (11/08/24@19:26:53)dbuddenbaum@amd64-01:~$ cd Documents/fine_tuning/

### #(cuda) (base) (11/08/24@19:49:22)dbuddenbaum@amd64-01:~/Documents/fine_tuning$ python -m ipykernel install --user --name=cuda --display-name "cuda-gpt"
Installed kernelspec cuda in /home/dbuddenbaum/.local/share/jupyter/kernels/cuda

### #(cuda) (base) (11/08/24@19:51:12)dbuddenbaum@amd64-01:~/Documents/fine_tuning$ jupyter notebook

```
[I 2024-11-09 15:25:01.549 ServerApp] Serving notebooks from local directory: /home/dbuddenbaum/Documents/fine_tuning
    1 active kernel
    Jupyter Server 2.14.2 is running at:
```
