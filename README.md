# bailingMM-Chat

## Approach

bailingMM-Chat is a multimodal method trained on a variety of multimodal datasets, which benefits many different tasks.

bailingMM-Chat has a total of 11B parameters. The visual encoder, dubbed as bailingMM-Encoder, is a transformer-based model with ~1B parameters. The LLM, namely bailing-10B shares the same structure with GLM. Before multi-modal training, we first pre-train the visual encoder as well as the LLM respectively using in-house visual and multilingual data, where the visual encoder and bailing-10B LLM are both trained from scratch. After that, we tune the parameters of the whole model in multimodal training process.

## Model architecture

<div align="center">
<img src=assets/framework.jpg style="zoom:40%">
