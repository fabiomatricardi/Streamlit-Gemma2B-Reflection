<img src='https://github.com/fabiomatricardi/Streamlit-Gemma2B-Reflection/raw/main/images/logo_reflection2B.png' width=900>

# Streamlit-Gemma2B-Reflection
Stramlit interface for Reflection2B - a Gemma2-2B-it prompt hack


## Instructions

- Clone the repo
- browse inside the main directory

### 1. Create a venv
Python 3.11+

### 2. Install dependencies in `venv`
```
pip install streamlit==1.36.0 llama-cpp-python==0.2.85 tiktoken
```

### 3. Download the model inside `model` subdirectory
- GGUF file from [https://huggingface.co/bartowski/gemma-2-2b-it-GGUF
](https://huggingface.co/bartowski/gemma-2-2b-it-GGUF
)

- original Google Gemma REPO [https://huggingface.co/google/gemma-2-2b-it
](https://huggingface.co/google/gemma-2-2b-it
)
- FileName: **gemma-2-2b-it-Q5_K_M.gguf**

### 4. Run the streamlit app
from the terminal run
```
streamlit run .\HF_streamlitAPP.py
```



<img src='https://github.com/fabiomatricardi/Streamlit-Gemma2B-Reflection/raw/main/images/Gemma2B-reflectionLLM-streamlit.gif' width=900>



### MODEL CARD
```
NCTX = 8192
CHAT TEMPLATE YES
SYSTEM MESSAGE NOT SUPPORTED
```

### Prompt Format
```
<bos><start_of_turn>user
{prompt}<end_of_turn>
<start_of_turn>model
<end_of_turn>
```

### GGUF model details
```
llm_load_print_meta: format           = GGUF V3 (latest)
llm_load_print_meta: arch             = gemma2
llm_load_print_meta: vocab type       = SPM
llm_load_print_meta: n_vocab          = 256000
llm_load_print_meta: n_merges         = 0
llm_load_print_meta: vocab_only       = 0
llm_load_print_meta: n_ctx_train      = 8192
llm_load_print_meta: model type       = 2B
llm_load_print_meta: model ftype      = Q5_K - Medium
llm_load_print_meta: model params     = 2.61 B
llm_load_print_meta: model size       = 1.79 GiB (5.87 BPW)
llm_load_print_meta: general.name     = Gemma 2 2b It
llm_load_print_meta: BOS token        = 2 '<bos>'
llm_load_print_meta: EOS token        = 1 '<eos>'
llm_load_print_meta: UNK token        = 3 '<unk>'
llm_load_print_meta: PAD token        = 0 '<pad>'
llm_load_print_meta: LF token         = 227 '<0x0A>'
llm_load_print_meta: EOT token        = 107 '<end_of_turn>'
```

