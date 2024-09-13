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

Setup the api key:

```bash
export OPENAI_API_KEY=sk-123456789
```

Then we can initilize the evaluator LLM with `xxx`:

```python
import os
from xx import xx

model = "xx"
api_base = "http://0.0.0.0:5000/v1"

```

### Run the Evaluation Pipeline

```python
from RefFreeEval import Results, Evaluator
from RefFreeEval.metrics import xxmetric

# set-up the evaluator
evaluator = Evaluator(model = 'xx', ...)

# evaluate results
evaluator.evaluate(Results)

```
