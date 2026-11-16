# Abyss Coder

**Abyss Coder 0.5B** is a compact, text-only coding assistant model packaged as a GGUF file for local inference.

## Download the model

Get the latest final model from the [GitHub Releases page](https://github.com/SonicZ-z/abyss-coder/releases/latest). Download **`Abyss-Coder-0.5B-Q2_K.gguf`** from the release assets. It is about 415 MB; the model file is distributed as a release download rather than stored in Git history.

Use it with a local inference app that supports GGUF, such as llama.cpp. For example, after installing llama.cpp and downloading the file:

```bash
llama-cli -m ./Abyss-Coder-0.5B-Q2_K.gguf -cnv -c 4096 -n 512
```

The exact command and hardware needs can vary between inference apps and devices.

## What to expect

- About 0.5 billion parameters, in the compact **Q2_K** quantization.
- Text-only: it does not understand images.
- It can help draft, explain, or discuss code, but its answers and generated code can be wrong. Review code before using it.
- It runs locally when used with a local inference app; this repository does not provide a hosted chat service.

## Model origin and license

The underlying weights come from **Qwen2.5-Coder-0.5B-Instruct**, created by the Qwen team. This is a renamed and quantized build; Abyss branding does not mean the weights were trained from scratch by Abyss or by the project creator. The upstream model is distributed under the **Apache License 2.0**.

- [Upstream Qwen model card](https://huggingface.co/Qwen/Qwen2.5-Coder-0.5B-Instruct)
- [Upstream GGUF repository](https://huggingface.co/Qwen/Qwen2.5-Coder-0.5B-Instruct-GGUF)
- [Attribution and model notice](model/NOTICE.txt)
- [Apache License 2.0 text](model/LICENSE-APACHE-2.0.txt)

## Releases

Final model files are published as assets on the [Releases page](https://github.com/SonicZ-z/abyss-coder/releases). Check the release notes for the version and file details.
