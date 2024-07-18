# llamafile Examples

## Using llamafile with external weights

Download the llamafile executable:

```bash
mkdir models
cd models

curl -L -o llamafile https://github.com/Mozilla-Ocho/llamafile/releases/download/0.8.9/llamafile-0.8.9
chmod +x llamafile
```

Download the model and run with llamafile:

```bash
curl -L -o h2o-danube3-500m-chat-Q5_K_M.gguf https://huggingface.co/h2oai/h2o-danube3-500m-chat-GGUF/resolve/main/h2o-danube3-500m-chat-Q5_K_M.gguf?download=true
./llamafile -m h2o-danube3-500m-chat-Q5_K_M.gguf
```

The `zipalign` executable can be found in the following download:
https://github.com/Mozilla-Ocho/llamafile/releases/download/0.8.9/llamafile-0.8.9.zip

## Create a llamafile

```bash
./make_llamafile h2o-danube3-500m-chat-Q5_K_M
```