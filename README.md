# RefFreeEval-RAG

## Highligth Features

xx

## Quick Start

### Setup Evaluator LLMs

- OpenAI

xx

- Open source LLMs

Please use [vllm](https://github.com/vllm-project/vllm) to setup the API server for open source LLMs. For example, use the following command to deploy a xx hosted on HuggingFace:

```bash
python -m vllm.entrypoints.openai.api_server \
  --model meta-llama/Meta-Llama-3-8B-Instruct \
  --tensor-parallel-size 8 \
  --dtype auto \
  --api-key sk-123456789 \
  --gpu-memory-utilization 0.9 \
  --port 5000
```

### Run the Evaluation Pipeline

```python
import os
from RefFreeEval import Results, Evaluator
from RefFreeEval.metrics import xxmetric

os.environments[]

# set-up the evaluator
evaluator = Evaluator(model = 'xx', ...)

# evaluate results
evaluator.evaluate(Results)

```
