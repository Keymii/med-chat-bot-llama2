# Medical Chatbot

## Installation
### Installation of Dependencies
```
pip install -r requirements.txt
```
### Installing the model
Download GGML format model files for Meta Llama 2's 8-bit quantized Llama 2 7B Chat model from [here](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/resolve/main/llama-2-7b-chat.ggmlv3.q8_0.bin?download=true). Keep the filename as *lama-2-7b-chat.ggmlv3.q8_0.bin*  and save at the root of this directory.

### Customizing the database
Inside the 'data/' folder, put in the desired PDF(s). These will serve as your datasets.

### Generation of Vector Database
```
python ingest.py
```
Running this script will generate a vector database

## Execution
```
chainlit run model.py -w
```

