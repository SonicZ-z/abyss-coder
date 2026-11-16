# Abyss Coder

**Abyss Coder** is a compact, text-only coding assistant model packaged as a GGUF file for local use.

## Download the model

Download **[`abyss.gguf`](https://github.com/SonicZ-z/abyss-coder/releases/download/v0.5.0/abyss.gguf)** from the [latest GitHub Release](https://github.com/SonicZ-z/abyss-coder/releases/latest). The file is about 415 MB and is distributed as a release asset, not stored in Git history.

For a desktop inference app that supports GGUF, such as llama.cpp, a sample command is:

```bash
llama-cli -m ./abyss.gguf -cnv -c 4096 -n 512
```

Commands and hardware needs vary between apps and devices.

## Android setup with AndroidHarness

[AndroidHarness](https://github.com/Sanuu7/AndroidHarness) is an Android app that supports local GGUF models as well as cloud model providers. Install it from [Google Play](https://play.google.com/store/apps/details?id=com.androidharness.app) or its [GitHub Releases page](https://github.com/Sanuu7/AndroidHarness/releases/latest), then finish the app's first-run setup.

1. Download `abyss.gguf` from the [Abyss Coder release](https://github.com/SonicZ-z/abyss-coder/releases/latest) to your phone.
2. In AndroidHarness, open **Settings** and scroll down to **Local models**.
3. Tap **Import file** and choose `abyss.gguf` from your phone's file picker, such as the Downloads folder.
4. After import, select Abyss Coder in the app's model picker to use it locally.

AndroidHarness documents that **Import file** accepts GGUF files. Local inference works offline after setup on a compatible 64-bit device. The app also supports cloud models, which are configured separately from imported local models.

## What to expect

- About 0.5 billion parameters, in the compact **Q2_K** quantization.
- Text only. It does not understand images.
- It can help draft, explain, or discuss code, but its answers and generated code can be wrong. Review code before using it.
- This repository does not provide a hosted chat service.
## Model origin and license

The weights were trained from scratch by @fakesonicz_ on discord. This is an original model built end-to-end on its own training run, The model is distributed under the **Apache License 2.0**.

## Releases

Final model files are published on the [GitHub Releases page](https://github.com/SonicZ-z/abyss-coder/releases). Check the release notes for each version's file details.
