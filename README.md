# Awesome Local LLM <img src="https://awesome.re/badge.svg"/>

A curated list of awesome platforms, tools, practices and resources that help run LLMs locally — in tabular format.

## Table of Contents

- [Inference Platforms](#inference-platforms)
- [Inference Engines](#inference-engines)
- [User Interfaces](#user-interfaces)
- [Large Language Models](#large-language-models)
  - [Explorers, Benchmarks, Leaderboards](#explorers-benchmarks-leaderboards)
  - [Model Providers](#model-providers)
  - [Specific Models](#specific-models)
    - [General Purpose](#general-purpose)
    - [Coding](#coding)
    - [Multimodal](#multimodal)
    - [Image](#image)
    - [Audio](#audio)
    - [Retrieval-Augmented Generation](#retrieval-augmented-generation)
    - [Safeguards](#safeguards)
    - [Miscellaneous](#miscellaneous)
- [Tools](#tools)
  - [Models](#models)
  - [Agent Frameworks](#agent-frameworks)
  - [Model Context Protocol](#model-context-protocol)
  - [Retrieval-Augmented Generation](#retrieval-augmented-generation-1)
  - [Coding Agents](#coding-agents)
  - [Computer Use](#computer-use)
  - [Browser Automation](#browser-automation)
  - [Memory Management](#memory-management)
  - [Testing, Evaluation and Observability](#testing-evaluation-and-observability)
  - [Research](#research)
  - [Training and Fine-tuning](#training-and-fine-tuning)
  - [Security and Sandboxing](#security-and-sandboxing)
  - [Miscellaneous](#miscellaneous-1)
- [Hardware](#hardware)
- [Tutorials](#tutorials)
  - [Models](#models-1)
  - [Prompt Engineering](#prompt-engineering)
  - [Context Engineering](#context-engineering)
  - [Inference](#inference)
  - [Agents](#agents)
  - [Retrieval-Augmented Generation](#retrieval-augmented-generation-2)
  - [Miscellaneous](#miscellaneous-2)
- [Communities](#communities)
- [Contributing](#contributing)

## Inference Platforms

| Project | Stars | Description |
|---|---|---|
| [LM Studio](https://lmstudio.ai/) | — | Discover, download and run local LLMs |
| [unsloth](https://github.com/unslothai/unsloth) | <img src="https://img.shields.io/github/stars/unslothai/unsloth?style=social" height="17"/> | Unified web UI for training and running open models like Qwen, DeepSeek, and Gemma locally |
| [LocalAI](https://github.com/mudler/LocalAI) | <img src="https://img.shields.io/github/stars/mudler/LocalAI?style=social" height="17"/> | The free, open-source alternative to OpenAI, Claude and others |
| [jan](https://github.com/menloresearch/jan) | <img src="https://img.shields.io/github/stars/menloresearch/jan?style=social" height="17"/> | An open source alternative to ChatGPT that runs 100% offline on your computer |
| [ChatBox](https://github.com/ChatBoxAI/ChatBox) | <img src="https://img.shields.io/github/stars/ChatBoxAI/ChatBox?style=social" height="17"/> | User-friendly desktop client app for AI models/LLMs |
| [lemonade](https://github.com/lemonade-sdk/lemonade) | <img src="https://img.shields.io/github/stars/lemonade-sdk/lemonade?style=social" height="17"/> | A local LLM server with GPU and NPU acceleration |

[Back to Table of Contents](#table-of-contents)

## Inference Engines

| Project | Stars | Description |
|---|---|---|
| [ollama](https://github.com/ollama/ollama) | <img src="https://img.shields.io/github/stars/ollama/ollama?style=social" height="17"/> | Get up and running with LLMs |
| [llama.cpp](https://github.com/ggml-org/llama.cpp) | <img src="https://img.shields.io/github/stars/ggml-org/llama.cpp?style=social" height="17"/> | LLM inference in C/C++ |
| [vllm](https://github.com/vllm-project/vllm) | <img src="https://img.shields.io/github/stars/vllm-project/vllm?style=social" height="17"/> | A high-throughput and memory-efficient inference and serving engine for LLMs |
| [exo](https://github.com/exo-explore/exo) | <img src="https://img.shields.io/github/stars/exo-explore/exo?style=social" height="17"/> | Run your own AI cluster at home with everyday devices |
| [BitNet](https://github.com/microsoft/BitNet) | <img src="https://img.shields.io/github/stars/microsoft/BitNet?style=social" height="17"/> | Official inference framework for 1-bit LLMs |
| [sglang](https://github.com/sgl-project/sglang) | <img src="https://img.shields.io/github/stars/sgl-project/sglang?style=social" height="17"/> | A fast serving framework for large language models and vision language models |
| [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | <img src="https://img.shields.io/github/stars/NVIDIA/TensorRT-LLM?style=social" height="17"/> | Easy-to-use Python API to define LLMs with state-of-the-art optimizations for efficient inference on NVIDIA GPUs |
| [Nano-vLLM](https://github.com/GeeeekExplorer/nano-vllm) | <img src="https://img.shields.io/github/stars/GeeeekExplorer/nano-vllm?style=social" height="17"/> | A lightweight vLLM implementation built from scratch |
| [omlx](https://github.com/jundot/omlx) | <img src="https://img.shields.io/github/stars/jundot/omlx?style=social" height="17"/> | LLM inference server with continuous batching & SSD caching for Apple Silicon — managed from the macOS menu bar |
| [koboldcpp](https://github.com/LostRuins/koboldcpp) | <img src="https://img.shields.io/github/stars/LostRuins/koboldcpp?style=social" height="17"/> | Run GGUF models easily with a KoboldAI UI |
| [mistral.rs](https://github.com/EricLBuehler/mistral.rs) | <img src="https://img.shields.io/github/stars/EricLBuehler/mistral.rs?style=social" height="17"/> | Fast, flexible LLM inference |
| [dynamo](https://github.com/ai-dynamo/dynamo) | <img src="https://img.shields.io/github/stars/ai-dynamo/dynamo?style=social" height="17"/> | A datacenter-scale distributed inference serving framework (NVIDIA) |
| [flashinfer](https://github.com/flashinfer-ai/flashinfer) | <img src="https://img.shields.io/github/stars/flashinfer-ai/flashinfer?style=social" height="17"/> | Kernel library for LLM serving |
| [mlx-lm](https://github.com/ml-explore/mlx-lm) | <img src="https://img.shields.io/github/stars/ml-explore/mlx-lm?style=social" height="17"/> | Generate text and fine-tune large language models on Apple silicon with MLX |
| [gpustack](https://github.com/gpustack/gpustack) | <img src="https://img.shields.io/github/stars/gpustack/gpustack?style=social" height="17"/> | Simple, scalable AI model deployment on GPU clusters |
| [LiteRT-LM](https://github.com/google-ai-edge/LiteRT-LM) | <img src="https://img.shields.io/github/stars/google-ai-edge/LiteRT-LM?style=social" height="17"/> | Google's production-ready, high-performance, open-source inference framework for deploying LLMs on edge devices |
| [mlx-vlm](https://github.com/Blaizzy/mlx-vlm) | <img src="https://img.shields.io/github/stars/Blaizzy/mlx-vlm?style=social" height="17"/> | A package for inference and fine-tuning of Vision Language Models (VLMs) on your Mac using MLX |
| [executorch](https://github.com/pytorch/executorch) | <img src="https://img.shields.io/github/stars/pytorch/executorch?style=social" height="17"/> | On-device AI across mobile, embedded and edge for PyTorch |
| [mini-sglang](https://github.com/sgl-project/mini-sglang) | <img src="https://img.shields.io/github/stars/sgl-project/mini-sglang?style=social" height="17"/> | A lightweight yet high-performance inference framework for Large Language Models |
| [distributed-llama](https://github.com/b4rtaz/distributed-llama) | <img src="https://img.shields.io/github/stars/b4rtaz/distributed-llama?style=social" height="17"/> | Connect home devices into a powerful cluster to accelerate LLM inference |
| [LiteRT](https://github.com/google-ai-edge/litert) | <img src="https://img.shields.io/github/stars/google-ai-edge/litert?style=social" height="17"/> | Google's on-device framework for high-performance ML & GenAI deployment on edge platforms |
| [ik_llama.cpp](https://github.com/ikawrakow/ik_llama.cpp) | <img src="https://img.shields.io/github/stars/ikawrakow/ik_llama.cpp?style=social" height="17"/> | llama.cpp fork with additional SOTA quants and improved performance |
| [aphrodite-engine](https://github.com/aphrodite-engine/aphrodite-engine) | <img src="https://img.shields.io/github/stars/aphrodite-engine/aphrodite-engine?style=social" height="17"/> | Large-scale LLM inference engine |
| [FastFlowLM](https://github.com/FastFlowLM/FastFlowLM) | <img src="https://img.shields.io/github/stars/FastFlowLM/FastFlowLM?style=social" height="17"/> | Run LLMs on AMD Ryzen™ AI NPUs |
| [tokenspeed](https://github.com/lightseekorg/tokenspeed) | <img src="https://img.shields.io/github/stars/lightseekorg/tokenspeed?style=social" height="17"/> | A speed-of-light LLM inference engine |
| [krasis](https://github.com/brontoguana/krasis) | <img src="https://img.shields.io/github/stars/brontoguana/krasis?style=social" height="17"/> | A hybrid LLM runtime focused on efficiently running larger models on consumer-grade, VRAM-limited hardware |
| [vllm-gfx906](https://github.com/nlzy/vllm-gfx906) | <img src="https://img.shields.io/github/stars/nlzy/vllm-gfx906?style=social" height="17"/> | vLLM for AMD gfx906 GPUs, e.g. Radeon VII / MI50 / MI60 |
| [llm-scaler](https://github.com/intel/llm-scaler) | <img src="https://img.shields.io/github/stars/intel/llm-scaler?style=social" height="17"/> | Run LLMs on Intel Arc™ Pro B60 GPUs |

[Back to Table of Contents](#table-of-contents)

## User Interfaces

| Project | Stars | Description |
|---|---|---|
| [Open WebUI](https://github.com/open-webui/open-webui) | <img src="https://img.shields.io/github/stars/open-webui/open-webui?style=social" height="17"/> | User-friendly AI interface (supports Ollama, OpenAI API, ...) |
| [Lobe Chat](https://github.com/lobehub/lobe-chat) | <img src="https://img.shields.io/github/stars/lobehub/lobe-chat?style=social" height="17"/> | An open-source, modern design AI chat framework |
| [Text generation web UI](https://github.com/oobabooga/text-generation-webui) | <img src="https://img.shields.io/github/stars/oobabooga/text-generation-webui?style=social" height="17"/> | LLM UI with advanced features, easy setup, and multiple backend support |
| [SillyTavern](https://github.com/SillyTavern/SillyTavern) | <img src="https://img.shields.io/github/stars/SillyTavern/SillyTavern?style=social" height="17"/> | LLM frontend for power users |
| [Page Assist](https://github.com/n4ze3m/page-assist) | <img src="https://img.shields.io/github/stars/n4ze3m/page-assist?style=social" height="17"/> | Use your locally running AI models to assist you in your web browsing |

[Back to Table of Contents](#table-of-contents)

## Large Language Models

### Explorers, Benchmarks, Leaderboards

| Name | Stars | Description |
|---|---|---|
| [Arena](https://arena.ai/) | — | Benchmark & compare the best AI models |
| [AI Models & API Providers Analysis](https://artificialanalysis.ai/) | — | Understand the AI landscape to choose the best model and provider for your use case |
| [SWE-rebench](https://swe-rebench.com/) | — | A continuously evolving and decontaminated benchmark for software engineering LLMs |
| [BullshitBench](https://github.com/petergpt/bullshit-benchmark) | <img src="https://img.shields.io/github/stars/petergpt/bullshit-benchmark?style=social" height="17"/> | Measure whether AI models challenge nonsensical prompts instead of confidently answering them |
| [LLM Explorer](https://llm-explorer.com/) | — | Explore list of the open-source LLM models |
| [Dubesor LLM Benchmark table](https://dubesor.de/benchtable) | — | Small-scale manual performance comparison benchmark |
| [oobabooga benchmark](https://oobabooga.github.io/benchmark.html) | — | A list sorted by size (on disk) for each score |
| [CyberGym](https://www.cybergym.io/) | — | Evaluating AI agents' real-world cybersecurity capabilities at scale |
| [vakra](https://github.com/IBM/vakra) | <img src="https://img.shields.io/github/stars/IBM/vakra?style=social" height="17"/> | A benchmark for evaluating multi-hop, multi-source tool-calling in AI agents |

[Back to Table of Contents](#table-of-contents)

### Model Providers

| Provider | Description |
|---|---|
| [Qwen](https://huggingface.co/Qwen) | Powered by Alibaba Cloud |
| [Mistral AI](https://huggingface.co/mistralai) | A pioneering French artificial intelligence startup |
| [Tencent](https://huggingface.co/tencent) | A profile of a Chinese multinational technology conglomerate and holding company |
| [Unsloth AI](https://huggingface.co/unsloth) | Focusing on making AI more accessible to everyone (GGUFs etc.) |
| [bartowski](https://huggingface.co/bartowski) | Providing GGUF versions of popular LLMs |
| [Beijing Academy of Artificial Intelligence](https://huggingface.co/BAAI) | A private non-profit organization engaged in AI research and development |
| [Open Thoughts](https://huggingface.co/open-thoughts) | A team of researchers and engineers curating the best open reasoning datasets |

[Back to Table of Contents](#table-of-contents)

### Specific Models

#### General Purpose

| Model | Provider | Description |
|---|---|---|
| [Qwen3.6](https://huggingface.co/collections/Qwen/qwen36) | Qwen (Alibaba) | A collection of the latest generation Qwen LLMs |
| [NVIDIA Nemotron v3](https://huggingface.co/collections/nvidia/nvidia-nemotron-v3) | NVIDIA | A family of open models with open weights, training data and recipes, delivering leading efficiency and accuracy for building specialized AI agents |
| [Gemma 4](https://huggingface.co/collections/google/gemma-4) | Google DeepMind | A family of open, multimodal models handling text and image input (with audio supported on small models) and generating text output |
| [Mistral Medium 3.5](https://huggingface.co/collections/mistralai/mistral-medium-35) | Mistral AI | The first flagship models from Mistral AI handling instruction-following, reasoning, and coding in a single set of open weights |
| [gpt-oss](https://huggingface.co/collections/openai/gpt-oss-68911959590a1634ba11c7a4) | OpenAI | A collection of open-weight models designed for powerful reasoning, agentic tasks, and versatile developer use cases |
| [gpt-oss-puzzle-88B](https://huggingface.co/nvidia/gpt-oss-puzzle-88B) | NVIDIA | A deployment-optimized large language model derived from OpenAI's gpt-oss-120b |
| [Hunyuan](https://huggingface.co/collections/tencent/hunyuan-dense-model-6890632cda26b19119c9c5e7) | Tencent | Open-source efficient LLMs designed for versatile deployment across diverse computational environments |
| [Phi-4](https://huggingface.co/collections/microsoft/phi-4) | Microsoft | A family of small language, multi-modal and reasoning models |
| [OpenReasoning-Nemotron](https://huggingface.co/collections/nvidia/openreasoning-nemotron-687730dae0170059860f1f01) | NVIDIA | Models trained on 5M reasoning traces for math, code and science |
| [Kimi K2.5](https://huggingface.co/collections/moonshotai/kimi-k25) | Moonshot AI | Open-source, native multimodal agentic models advancing long-horizon coding, coding-driven design, proactive autonomous execution, and swarm-based task orchestration |
| [GLM-5.2](https://huggingface.co/collections/zai-org/glm-52) | Z.ai | Z.ai's flagship model for long-horizon tasks |
| [Granite 4.1](https://huggingface.co/collections/ibm-granite/granite-41-language-models) | IBM | Efficient language models for multilingual generation, coding, RAG, and AI assistant workflows |
| [EXAONE-4.5](https://huggingface.co/collections/LGAI-EXAONE/exaone-45) | LG AI | LG's first open-weight vision-language model for industrial intelligence |
| [ERNIE 4.5](https://huggingface.co/collections/baidu/ernie-45-6861cd4c9be84540645f35c9) | Baidu | A collection of large-scale multimodal models |
| [Seed-OSS](https://huggingface.co/collections/ByteDance-Seed/seed-oss-68a609f4201e788db05b5dcd) | ByteDance Seed | LLMs designed for powerful long-context, reasoning, agent and general capabilities, with versatile developer-friendly features |
| [Step-3.5-Flash](https://huggingface.co/stepfun-ai/Step-3.5-Flash) | StepFun | Capable open-source foundation model, engineered to deliver frontier reasoning and agentic capabilities with exceptional efficiency |
| [Rio-3.5-Open-397B](https://huggingface.co/prefeitura-rio/Rio-3.5-Open-397B) | Prefeitura Rio | A frontier-class general-purpose AI model post-trained from Qwen 3.5 397B |
| [Nex-N2](https://huggingface.co/collections/nex-agi/nex-n2) | Nex AGI | A collection of agent models built for real-world productivity scenarios |

[Back to Table of Contents](#table-of-contents)

#### Coding

| Model | Provider | Description |
|---|---|---|
| [Qwen3-Coder-Next](https://huggingface.co/collections/Qwen/qwen3-coder-next) | Qwen (Alibaba) | Open-weight language models designed specifically for coding agents and local development |
| [Devstral 2](https://huggingface.co/collections/mistralai/devstral-2) | Mistral AI | Agentic LLMs for software engineering tasks, excelling at using tools to explore codebases, edit multiple files, and power SWE agents |
| [Mellum 2](https://huggingface.co/collections/JetBrains/mellum-2) | JetBrains | An assistant model trained by JetBrains |
| [MiniMax-M3](https://huggingface.co/MiniMaxAI/MiniMax-M3) | MiniMax | A native multimodal model with 1M context |
| [MiniMax-M2](https://huggingface.co/collections/MiniMaxAI/minimax-m2) | MiniMax | SOTA models for real-world dev & agents |
| [SWE-FastContext](https://huggingface.co/collections/microsoft/swe-fastcontext) | Microsoft | A family of code-search models powering the Explore subagent for coding agents |
| [OmniCoder-9B](https://huggingface.co/Tesslate/OmniCoder-9B) | Tesslate | A 9-billion parameter coding agent model fine-tuned on top of Qwen3.5-9B's hybrid architecture |
| [NousCoder-14B](https://huggingface.co/NousResearch/NousCoder-14B) | Nous Research | A competitive programming model post-trained on Qwen3-14B via reinforcement learning |
| [MusaCoder-27B](https://huggingface.co/MooreThreads/MusaCoder-27B) | Moore Threads | A code model for PyTorch-to-CUDA/MUSA native kernel generation |

[Back to Table of Contents](#table-of-contents)

#### Multimodal

| Model | Provider | Description |
|---|---|---|
| [Qwen3-Omni](https://huggingface.co/collections/Qwen/qwen3-omni-68d100a86cd0906843ceccbe) | Qwen (Alibaba) | Natively end-to-end multilingual omni-modal foundation models |
| [GLM-4.6V](https://huggingface.co/collections/zai-org/glm-46v) | Zhipu AI (Z.ai) | Open source multimodal models with native tool use |

[Back to Table of Contents](#table-of-contents)

#### Image

| Model | Provider | Description |
|---|---|---|
| [Qwen-Image](https://huggingface.co/collections/Qwen/qwen-image) | Qwen (Alibaba) | Models for image generation, editing and decomposition |
| [Qwen3-VL](https://huggingface.co/collections/Qwen/qwen3-vl-68d2a7c1b8a8afce4ebd2dbe) | Qwen (Alibaba) | The most powerful vision-language models in the Qwen series to date |
| [GLM-Image](https://huggingface.co/zai-org/GLM-Image) | Z.ai | An image generation model |
| [Granite Vision](https://huggingface.co/collections/ibm-granite/granite-vision) | IBM | Multimodal models built for visual document analysis and image understanding |
| [HunyuanImage](https://huggingface.co/collections/tencent/hunyuanimage) | Tencent | A collection of image generation models |
| [HunyuanVideo](https://huggingface.co/collections/tencent/hunyuanvideo) | Tencent | A collection of video generation models |
| [Vidi](https://huggingface.co/collections/bytedance-research/vidi) | ByteDance | Models for multimodal video understanding and creation |
| [FastVLM](https://huggingface.co/collections/apple/fastvlm-68ac97b9cd5cacefdd04872e) | Apple | VLMs with efficient vision encoding |
| [MiniCPM-o & MiniCPM-V](https://huggingface.co/collections/openbmb/minicpm-o-and-minicpm-v) | OpenBMB | Multimodal models with leading performance |
| [LFM2-VL](https://huggingface.co/collections/LiquidAI/lfm2-vl-68963bbc84a610f7638d5ffa) | Liquid AI | Vision-language models designed for on-device deployment |
| [ClipTagger-12b](https://huggingface.co/inference-net/ClipTagger-12b) | Inference.net | A vision-language model (VLM) designed for video understanding at massive scale |

[Back to Table of Contents](#table-of-contents)

#### Audio

| Model | Provider | Description |
|---|---|---|
| [whisper-large-v3](https://huggingface.co/openai/whisper-large-v3) | OpenAI | A state-of-the-art model for automatic speech recognition (ASR) and speech translation |
| [Nemotron Speech](https://huggingface.co/collections/nvidia/nemotron-speech) | NVIDIA | Open, state-of-the-art, production-ready enterprise speech models for ASR, TTS, speaker diarization and S2S |
| [Qwen3-ASR](https://huggingface.co/collections/Qwen/qwen3-asr) | Qwen (Alibaba) | Models supporting language identification and ASR for 52 languages and dialects |
| [Qwen3-TTS](https://huggingface.co/collections/Qwen/qwen3-tts) | Qwen (Alibaba) | TTS models covering 10 major languages plus multiple dialectal voice profiles |
| [Granite Speech](https://huggingface.co/collections/ibm-granite/granite-speech) | IBM | Compact and efficient speech-language models for multilingual ASR and bidirectional automatic speech translation (AST) |
| [Voxtral-Small-24B-2507](https://huggingface.co/mistralai/Voxtral-Small-24B-2507) | Mistral AI | An enhancement of Mistral Small 3 with state-of-the-art audio input capabilities and best-in-class text performance |
| [Voxtral-Mini-4B-Realtime-2602](https://huggingface.co/mistralai/Voxtral-Mini-4B-Realtime-2602) | Mistral AI | A multilingual, realtime speech-transcription model with accuracy comparable to offline systems at <500ms delay |
| [Voxtral-4B-TTS-2603](https://huggingface.co/mistralai/Voxtral-4B-TTS-2603) | Mistral AI | Frontier, open-weights text-to-speech model that's fast, instantly adaptable, and produces lifelike speech for voice agents |
| [chatterbox](https://huggingface.co/ResembleAI/chatterbox) | Resemble AI | First production-grade open-source TTS model |
| [VibeVoice](https://huggingface.co/collections/microsoft/vibevoice-68a2ef24a875c44be47b034f) | Microsoft | A collection of frontier text-to-speech models |
| [Kitten TTS](https://huggingface.co/KittenML/models) | KittenML | Open-source realistic text-to-speech models designed for lightweight deployment and high-quality voice synthesis |
| [Streaming Sortformer Diarizer 4spk v2.1](https://huggingface.co/nvidia/diar_streaming_sortformer_4spk-v2.1) | NVIDIA | A streaming version of a novel end-to-end neural model for speaker diarization |

[Back to Table of Contents](#table-of-contents)

#### Retrieval-Augmented Generation

| Model | Provider | Description |
|---|---|---|
| [Nemotron RAG](https://huggingface.co/collections/nvidia/nemotron-rag) | NVIDIA | Tools to build RAG systems, improve search and ranking accuracy, and extract structured data from complex docs |
| [Qwen3-Embedding](https://huggingface.co/collections/Qwen/qwen3-embedding) | Qwen (Alibaba) | Models specifically designed for text embedding and ranking tasks |
| [Qwen3-VL-Embedding](https://huggingface.co/collections/Qwen/qwen3-vl-embedding) | Qwen (Alibaba) | Embedding models designed for multimodal information retrieval and cross-modal understanding |
| [Qwen3-Reranker](https://huggingface.co/collections/Qwen/qwen3-vl-reranker) | Qwen (Alibaba) | Models engineered to refine embedding results |
| [Qwen3-VL-Reranker](https://huggingface.co/collections/Qwen/qwen3-vl-reranker) | Qwen (Alibaba) | Reranker models designed for multimodal information retrieval and cross-modal understanding |

[Back to Table of Contents](#table-of-contents)

#### Safeguards

| Model | Provider | Description |
|---|---|---|
| [Granite Guardian](https://huggingface.co/collections/ibm-granite/granite-guardian) | IBM | Safety models for detecting risks, toxicity, and hallucinations in LLM workflows |
| [Qwen3Guard](https://huggingface.co/collections/Qwen/qwen3guard-68d2729abbfae4716f3343a1) | Qwen (Alibaba) | Safety moderation models built upon Qwen3 |
| [NemoGuard](https://huggingface.co/collections/nvidia/nemoguard) | NVIDIA | Models for content safety, topic-following and security guardrails |
| [Nemotron-3.5-Content-Safety](https://huggingface.co/nvidia/Nemotron-3.5-Content-Safety) | NVIDIA | A small language model based on Google's Gemma-3-4B-it, fine-tuned on multimodal, multilingual, and reasoning-oriented content-safety datasets |
| [Privasis](https://huggingface.co/collections/nvidia/privasis) | NVIDIA | Lightweight text-sanitization models that remove or abstract sensitive information from text per a user-provided sanitization instruction |
| [HARC](https://huggingface.co/collections/microsoft/harc) | Microsoft | A family of safety-aligned instruction models trained with HARC |
| [gpt-oss-safeguard](https://huggingface.co/collections/openai/gpt-oss-safeguard) | OpenAI | Safety reasoning models built upon gpt-oss |
| [privacy-filter](https://huggingface.co/openai/privacy-filter) | OpenAI | A bidirectional token-classification model for personally identifiable information (PII) detection and masking in text |
| [AprielGuard](https://huggingface.co/ServiceNow-AI/AprielGuard) | ServiceNow | A safeguard model designed to detect and mitigate both safety risks and security threats in LLM interactions |

[Back to Table of Contents](#table-of-contents)

#### Miscellaneous

| Model | Provider | Description |
|---|---|---|
| [Marco-MoE](https://huggingface.co/collections/AIDC-AI/marco-moe) | AIDC-AI (Alibaba) | A suite of multilingual MoE models with highly-sparse architectures |
| [Jan-v3](https://huggingface.co/collections/janhq/jan-v3) | Jan | A 4B baseline model for fine-tuning: improved instruction following out of the box, strong starting point for fine-tuning and effective lightweight coding assistance |
| [Jan-v2-VL](https://huggingface.co/collections/janhq/jan-v2-vl) | Jan | A family of VLMs focused on reliable, many-step task execution |
| [Nemotron-Orchestrator-8B](https://huggingface.co/nvidia/Nemotron-Orchestrator-8B) | NVIDIA | A state-of-the-art 8B orchestration model designed to solve complex, multi-turn agentic tasks by coordinating a diverse set of expert models and tools |
| [Arch-Router-1.5B](https://huggingface.co/katanemo/Arch-Router-1.5B) | Katanemo | The fastest LLM router model that aligns to subjective usage preferences |
| [Waypoint](https://huggingface.co/collections/Overworld/waypoint) | Overworld | A collection of real-time interactive video world models |
| [Hunyuan3D](https://huggingface.co/collections/tencent/hunyuan3d) | Tencent | Everything related (models, datasets etc.) to 3D asset generation |
| [Hunyuan-GameCraft-1.0](https://huggingface.co/tencent/Hunyuan-GameCraft-1.0) | Tencent | A novel framework for high-dynamic interactive video generation in game environments |
| [void-model](https://huggingface.co/netflix/void-model) | Netflix | Removes objects from videos along with all interactions they induce on the scene — not just shadows and reflections, but physical interactions like objects falling when a person is removed |

[Back to Table of Contents](#table-of-contents)

## Tools

### Models

| Project | Stars | Description |
|---|---|---|
| [llmfit](https://github.com/AlexsJones/llmfit) | <img src="https://img.shields.io/github/stars/AlexsJones/llmfit?style=social" height="17"/> | Hundreds of models & providers, one command to find what runs on your hardware |
| [outlines](https://github.com/dottxt-ai/outlines) | <img src="https://img.shields.io/github/stars/dottxt-ai/outlines?style=social" height="17"/> | Structured outputs for LLMs |
| [llama-swap](https://github.com/mostlygeek/llama-swap) | <img src="https://img.shields.io/github/stars/mostlygeek/llama-swap?style=social" height="17"/> | Reliable model swapping for any local OpenAI compatible server — llama.cpp, vllm, etc. |
| [llguidance](https://github.com/guidance-ai/llguidance) | <img src="https://img.shields.io/github/stars/guidance-ai/llguidance?style=social" height="17"/> | Super-fast structured outputs |

[Back to Table of Contents](#table-of-contents)

### Agent Frameworks

| Project | Stars | Description |
|---|---|---|
| [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT) | <img src="https://img.shields.io/github/stars/Significant-Gravitas/AutoGPT?style=social" height="17"/> | A powerful platform to create, deploy, and manage continuous AI agents that automate complex workflows |
| [langflow](https://github.com/langflow-ai/langflow) | <img src="https://img.shields.io/github/stars/langflow-ai/langflow?style=social" height="17"/> | A powerful tool for building and deploying AI-powered agents and workflows |
| [langchain](https://github.com/langchain-ai/langchain) | <img src="https://img.shields.io/github/stars/langchain-ai/langchain?style=social" height="17"/> | Build context-aware reasoning applications |
| [anything-llm](https://github.com/Mintplex-Labs/anything-llm) | <img src="https://img.shields.io/github/stars/Mintplex-Labs/anything-llm?style=social" height="17"/> | The all-in-one Desktop & Docker AI application with built-in RAG, AI agents, no-code agent builder, MCP compatibility, and more |
| [autogen](https://github.com/microsoft/autogen) | <img src="https://img.shields.io/github/stars/microsoft/autogen?style=social" height="17"/> | A programming framework for agentic AI |
| [Flowise](https://github.com/FlowiseAI/Flowise) | <img src="https://img.shields.io/github/stars/FlowiseAI/Flowise?style=social" height="17"/> | Build AI agents, visually |
| [pi](https://github.com/earendil-works/pi) | <img src="https://img.shields.io/github/stars/earendil-works/pi?style=social" height="17"/> | AI agent toolkit: coding agent CLI, unified LLM API, TUI & web UI libraries, Slack bot, vLLM pods |
| [llama_index](https://github.com/run-llama/llama_index) | <img src="https://img.shields.io/github/stars/run-llama/llama_index?style=social" height="17"/> | The leading framework for building LLM-powered agents over your data |
| [crewAI](https://github.com/crewAIInc/crewAI) | <img src="https://img.shields.io/github/stars/crewAIInc/crewAI?style=social" height="17"/> | A framework for orchestrating role-playing, autonomous AI agents |
| [agno](https://github.com/agno-agi/agno) | <img src="https://img.shields.io/github/stars/agno-agi/agno?style=social" height="17"/> | A full-stack framework for building multi-agent systems with memory, knowledge and reasoning |
| [sim](https://github.com/simstudioai/sim) | <img src="https://img.shields.io/github/stars/simstudioai/sim?style=social" height="17"/> | Open-source platform to build and deploy AI agent workflows |
| [openai-agents-python](https://github.com/openai/openai-agents-python) | <img src="https://img.shields.io/github/stars/openai/openai-agents-python?style=social" height="17"/> | A lightweight, powerful framework for multi-agent workflows |
| [NemoClaw](https://github.com/NVIDIA/NemoClaw) | <img src="https://img.shields.io/github/stars/NVIDIA/NemoClaw?style=social" height="17"/> | Run OpenClaw more securely inside NVIDIA OpenShell with managed inference |
| [SuperAGI](https://github.com/TransformerOptimus/SuperAGI) | <img src="https://img.shields.io/github/stars/TransformerOptimus/SuperAGI?style=social" height="17"/> | An open-source framework to build, manage and run useful autonomous AI agents |
| [camel](https://github.com/camel-ai/camel) | <img src="https://img.shields.io/github/stars/camel-ai/camel?style=social" height="17"/> | The first and the best multi-agent framework |
| [pydantic-ai](https://github.com/pydantic/pydantic-ai) | <img src="https://img.shields.io/github/stars/pydantic/pydantic-ai?style=social" height="17"/> | A Python agent framework designed to help you quickly, confidently, and painlessly build production grade applications and workflows with Generative AI |
| [txtai](https://github.com/neuml/txtai) | <img src="https://img.shields.io/github/stars/neuml/txtai?style=social" height="17"/> | All-in-one open-source AI framework for semantic search, LLM orchestration and language model workflows |
| [agent-framework](https://github.com/microsoft/agent-framework) | <img src="https://img.shields.io/github/stars/microsoft/agent-framework?style=social" height="17"/> | A framework for building, orchestrating and deploying AI agents and multi-agent workflows with support for Python and .NET |
| [archgw](https://github.com/katanemo/archgw) | <img src="https://img.shields.io/github/stars/katanemo/archgw?style=social" height="17"/> | A high-performance proxy server that handles the low-level work in building agents: applying guardrails, routing prompts to the right agent, unifying access to LLMs, etc. |
| [genkit](https://github.com/genkit-ai/genkit) | <img src="https://img.shields.io/github/stars/genkit-ai/genkit?style=social" height="17"/> | Open-source framework for building AI-powered apps in JavaScript, Go, and Python, built and used in production by Google |
| [ClaraVerse](https://github.com/badboysm890/ClaraVerse) | <img src="https://img.shields.io/github/stars/badboysm890/ClaraVerse?style=social" height="17"/> | Privacy-first, fully local AI workspace with Ollama LLM chat, tool calling, agent builder, Stable Diffusion, and embedded n8n-style automation |
| [NeMo-Agent-Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) | <img src="https://img.shields.io/github/stars/NVIDIA/NeMo-Agent-Toolkit?style=social" height="17"/> | An open-source library for efficiently connecting and optimizing teams of AI agents |
| [ragbits](https://github.com/deepsense-ai/ragbits) | <img src="https://img.shields.io/github/stars/deepsense-ai/ragbits?style=social" height="17"/> | Building blocks for rapid development of GenAI applications |

[Back to Table of Contents](#table-of-contents)

### Model Context Protocol

| Project | Stars | Description |
|---|---|---|
| [mindsdb](https://github.com/mindsdb/mindsdb) | <img src="https://img.shields.io/github/stars/mindsdb/mindsdb?style=social" height="17"/> | Federated query engine for AI — the only MCP server you'll ever need |
| [github-mcp-server](https://github.com/github/github-mcp-server) | <img src="https://img.shields.io/github/stars/github/github-mcp-server?style=social" height="17"/> | GitHub's official MCP server |
| [playwright-mcp](https://github.com/microsoft/playwright-mcp) | <img src="https://img.shields.io/github/stars/microsoft/playwright-mcp?style=social" height="17"/> | Playwright MCP server |
| [chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | <img src="https://img.shields.io/github/stars/ChromeDevTools/chrome-devtools-mcp?style=social" height="17"/> | Chrome DevTools for coding agents |
| [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) | <img src="https://img.shields.io/github/stars/czlonkowski/n8n-mcp?style=social" height="17"/> | An MCP for Claude Desktop / Claude Code / Windsurf / Cursor to build n8n workflows for you |
| [awslabs/mcp](https://github.com/awslabs/mcp) | <img src="https://img.shields.io/github/stars/awslabs/mcp?style=social" height="17"/> | AWS MCP servers — helping you get the most out of AWS, wherever you use MCP |
| [mcp-atlassian](https://github.com/sooperset/mcp-atlassian) | <img src="https://img.shields.io/github/stars/sooperset/mcp-atlassian?style=social" height="17"/> | MCP server for Atlassian tools (Confluence, Jira) |
| [dbhub](https://github.com/bytebase/dbhub) | <img src="https://img.shields.io/github/stars/bytebase/dbhub?style=social" height="17"/> | Zero-dependency, token-efficient database MCP server for Postgres, MySQL, SQL Server, MariaDB, SQLite |

[Back to Table of Contents](#table-of-contents)

### Retrieval-Augmented Generation

| Project | Stars | Description |
|---|---|---|
| [pathway](https://github.com/pathwaycom/pathway) | <img src="https://img.shields.io/github/stars/pathwaycom/pathway?style=social" height="17"/> | Python ETL framework for stream processing, real-time analytics, LLM pipelines and RAG |
| [graphrag](https://github.com/microsoft/graphrag) | <img src="https://img.shields.io/github/stars/microsoft/graphrag?style=social" height="17"/> | A modular graph-based RAG system |
| [LightRAG](https://github.com/HKUDS/LightRAG) | <img src="https://img.shields.io/github/stars/HKUDS/LightRAG?style=social" height="17"/> | Simple and fast RAG |
| [haystack](https://github.com/deepset-ai/haystack) | <img src="https://img.shields.io/github/stars/deepset-ai/haystack?style=social" height="17"/> | AI orchestration framework to build customizable, production-ready LLM applications — best suited for RAG, question answering, semantic search or conversational agent chatbots |
| [vanna](https://github.com/vanna-ai/vanna) | <img src="https://img.shields.io/github/stars/vanna-ai/vanna?style=social" height="17"/> | An open-source Python RAG framework for SQL generation and related functionality |
| [graphiti](https://github.com/getzep/graphiti) | <img src="https://img.shields.io/github/stars/getzep/graphiti?style=social" height="17"/> | Build real-time knowledge graphs for AI agents |
| [onyx](https://github.com/onyx-dot-app/onyx) | <img src="https://img.shields.io/github/stars/onyx-dot-app/onyx?style=social" height="17"/> | The AI platform connected to your company's docs, apps, and people |
| [claude-context](https://github.com/zilliztech/claude-context) | <img src="https://img.shields.io/github/stars/zilliztech/claude-context?style=social" height="17"/> | Make entire codebase the context for any coding agent |
| [pipeshub-ai](https://github.com/pipeshub-ai/pipeshub-ai) | <img src="https://img.shields.io/github/stars/pipeshub-ai/pipeshub-ai?style=social" height="17"/> | A fully extensible and explainable workplace AI platform for enterprise search and workflow automation |

[Back to Table of Contents](#table-of-contents)

### Coding Agents

| Project | Stars | Description |
|---|---|---|
| [opencode](https://github.com/sst/opencode) | <img src="https://img.shields.io/github/stars/sst/opencode?style=social" height="17"/> | An AI coding agent built for the terminal |
| [zed](https://github.com/zed-industries/zed) | <img src="https://img.shields.io/github/stars/zed-industries/zed?style=social" height="17"/> | A next-generation code editor designed for high-performance collaboration with humans and AI |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | <img src="https://img.shields.io/github/stars/All-Hands-AI/OpenHands?style=social" height="17"/> | A platform for software development agents powered by AI |
| [cline](https://github.com/cline/cline) | <img src="https://img.shields.io/github/stars/cline/cline?style=social" height="17"/> | Autonomous coding agent right in your IDE, capable of creating/editing files, executing commands, using the browser, and more with your permission every step of the way |
| [aider](https://github.com/Aider-AI/aider) | <img src="https://img.shields.io/github/stars/Aider-AI/aider?style=social" height="17"/> | AI pair programming in your terminal |
| [tabby](https://github.com/TabbyML/tabby) | <img src="https://img.shields.io/github/stars/TabbyML/tabby?style=social" height="17"/> | An open-source GitHub Copilot alternative — set up your own LLM-powered code completion server |
| [continue](https://github.com/continuedev/continue) | <img src="https://img.shields.io/github/stars/continuedev/continue?style=social" height="17"/> | Create, share, and use custom AI code assistants with open-source IDE extensions and a hub of models, rules, prompts, docs, and other building blocks |
| [void](https://github.com/voideditor/void) | <img src="https://img.shields.io/github/stars/voideditor/void?style=social" height="17"/> | An open-source Cursor alternative — use AI agents on your codebase, checkpoint and visualize changes, and bring any model or host locally |
| [goose](https://github.com/block/goose) | <img src="https://img.shields.io/github/stars/block/goose?style=social" height="17"/> | An open-source, extensible AI agent that goes beyond code suggestions |
| [Roo-Code](https://github.com/RooCodeInc/Roo-Code) | <img src="https://img.shields.io/github/stars/RooCodeInc/Roo-Code?style=social" height="17"/> | A whole dev team of AI agents in your code editor |
| [crush](https://github.com/charmbracelet/crush) | <img src="https://img.shields.io/github/stars/charmbracelet/crush?style=social" height="17"/> | The glamourous AI coding agent for your favourite terminal |
| [kilocode](https://github.com/Kilo-Org/kilocode) | <img src="https://img.shields.io/github/stars/Kilo-Org/kilocode?style=social" height="17"/> | Open source AI coding assistant for planning, building, and fixing code |
| [humanlayer](https://github.com/humanlayer/humanlayer) | <img src="https://img.shields.io/github/stars/humanlayer/humanlayer?style=social" height="17"/> | The best way to get AI coding agents to solve hard problems in complex codebases |
| [99](https://github.com/ThePrimeagen/99) | <img src="https://img.shields.io/github/stars/ThePrimeagen/99?style=social" height="17"/> | Neovim AI agent done right |
| [ProxyAI](https://github.com/carlrobertoh/ProxyAI) | <img src="https://img.shields.io/github/stars/carlrobertoh/ProxyAI?style=social" height="17"/> | The leading open-source AI copilot for JetBrains |

[Back to Table of Contents](#table-of-contents)

### Computer Use

| Project | Stars | Description |
|---|---|---|
| [open-interpreter](https://github.com/OpenInterpreter/open-interpreter) | <img src="https://img.shields.io/github/stars/OpenInterpreter/open-interpreter?style=social" height="17"/> | A natural language interface for computers |
| [OmniParser](https://github.com/microsoft/OmniParser) | <img src="https://img.shields.io/github/stars/microsoft/OmniParser?style=social" height="17"/> | A simple screen parsing tool towards pure vision based GUI agent |
| [openwork](https://github.com/different-ai/openwork) | <img src="https://img.shields.io/github/stars/different-ai/openwork?style=social" height="17"/> | An open-source alternative to Claude Cowork, powered by OpenCode |
| [cua](https://github.com/trycua/cua) | <img src="https://img.shields.io/github/stars/trycua/cua?style=social" height="17"/> | The Docker container for computer-use AI agents |
| [Agent-S](https://github.com/simular-ai/Agent-S) | <img src="https://img.shields.io/github/stars/simular-ai/Agent-S?style=social" height="17"/> | An open agentic framework that uses computers like a human |
| [self-operating-computer](https://github.com/OthersideAI/self-operating-computer) | <img src="https://img.shields.io/github/stars/OthersideAI/self-operating-computer?style=social" height="17"/> | A framework to enable multimodal models to operate a computer |
| [OpenRoom](https://github.com/MiniMax-AI/OpenRoom) | <img src="https://img.shields.io/github/stars/MiniMax-AI/OpenRoom?style=social" height="17"/> | A browser-based desktop where an AI agent operates every app through natural language, from MiniMax |

[Back to Table of Contents](#table-of-contents)

### Browser Automation

| Project | Stars | Description |
|---|---|---|
| [puppeteer](https://github.com/puppeteer/puppeteer) | <img src="https://img.shields.io/github/stars/puppeteer/puppeteer?style=social" height="17"/> | A JavaScript API for Chrome and Firefox |
| [playwright](https://github.com/microsoft/playwright) | <img src="https://img.shields.io/github/stars/microsoft/playwright?style=social" height="17"/> | A framework for web testing and automation |
| [browser-use](https://github.com/browser-use/browser-use) | <img src="https://img.shields.io/github/stars/browser-use/browser-use?style=social" height="17"/> | Make websites accessible for AI agents |
| [firecrawl](https://github.com/mendableai/firecrawl) | <img src="https://img.shields.io/github/stars/mendableai/firecrawl?style=social" height="17"/> | Turn entire websites into LLM-ready markdown or structured data |
| [stagehand](https://github.com/browserbase/stagehand) | <img src="https://img.shields.io/github/stars/browserbase/stagehand?style=social" height="17"/> | The AI browser automation framework |
| [nanobrowser](https://github.com/nanobrowser/nanobrowser) | <img src="https://img.shields.io/github/stars/nanobrowser/nanobrowser?style=social" height="17"/> | Open-source Chrome extension for AI-powered web automation |

[Back to Table of Contents](#table-of-contents)

### Memory Management

| Project | Stars | Description |
|---|---|---|
| [mem0](https://github.com/mem0ai/mem0) | <img src="https://img.shields.io/github/stars/mem0ai/mem0?style=social" height="17"/> | Universal memory layer for AI agents |
| [mempalace](https://github.com/milla-jovovich/mempalace) | <img src="https://img.shields.io/github/stars/milla-jovovich/mempalace?style=social" height="17"/> | The highest-scoring AI memory system ever benchmarked |
| [letta](https://github.com/letta-ai/letta) | <img src="https://img.shields.io/github/stars/letta-ai/letta?style=social" height="17"/> | The stateful agents framework with memory, reasoning, and context management |
| [supermemory](https://github.com/supermemoryai/supermemory) | <img src="https://img.shields.io/github/stars/supermemoryai/supermemory?style=social" height="17"/> | Memory engine and app that is extremely fast, scalable |
| [cognee](https://github.com/topoteretes/cognee) | <img src="https://img.shields.io/github/stars/topoteretes/cognee?style=social" height="17"/> | Memory for AI agents in 5 lines of code |
| [LMCache](https://github.com/LMCache/LMCache) | <img src="https://img.shields.io/github/stars/LMCache/LMCache?style=social" height="17"/> | Supercharge your LLM with the fastest KV cache layer |
| [memU](https://github.com/NevaMind-AI/memU) | <img src="https://img.shields.io/github/stars/NevaMind-AI/memU?style=social" height="17"/> | An open-source memory framework for AI companions |
| [reasoning-bank](https://github.com/google-research/reasoning-bank) | <img src="https://img.shields.io/github/stars/google-research/reasoning-bank?style=social" height="17"/> | A memory mechanism for agents that learns from both successful and failed trajectories, with reasoning stored as memory content |

[Back to Table of Contents](#table-of-contents)

### Testing, Evaluation and Observability

| Project | Stars | Description |
|---|---|---|
| [langfuse](https://github.com/langfuse/langfuse) | <img src="https://img.shields.io/github/stars/langfuse/langfuse?style=social" height="17"/> | An open-source LLM engineering platform: LLM observability, metrics, evals, prompt management, playground, datasets. Integrates with OpenTelemetry, Langchain, OpenAI SDK, LiteLLM, and more |
| [opik](https://github.com/comet-ml/opik) | <img src="https://img.shields.io/github/stars/comet-ml/opik?style=social" height="17"/> | Debug, evaluate, and monitor your LLM applications, RAG systems, and agentic workflows with comprehensive tracing, automated evaluations, and production-ready dashboards |
| [openllmetry](https://github.com/traceloop/openllmetry) | <img src="https://img.shields.io/github/stars/traceloop/openllmetry?style=social" height="17"/> | An open-source observability for your LLM application, based on OpenTelemetry |
| [giskard](https://github.com/Giskard-AI/giskard) | <img src="https://img.shields.io/github/stars/Giskard-AI/giskard?style=social" height="17"/> | An open-source evaluation & testing for AI & LLM systems |
| [agenta](https://github.com/Agenta-AI/agenta) | <img src="https://img.shields.io/github/stars/Agenta-AI/agenta?style=social" height="17"/> | An open-source LLMOps platform: prompt playground, prompt management, LLM evaluation, and LLM observability all in one place |
| [Evaluator](https://github.com/NVIDIA-NeMo/evaluator) | <img src="https://img.shields.io/github/stars/NVIDIA-NeMo/evaluator?style=social" height="17"/> | Open-source library for scalable, reproducible evaluation of AI models and benchmarks (NVIDIA NeMo) |

[Back to Table of Contents](#table-of-contents)

### Research

| Project | Stars | Description |
|---|---|---|
| [Perplexica](https://github.com/ItzCrazyKns/Perplexica) | <img src="https://img.shields.io/github/stars/ItzCrazyKns/Perplexica?style=social" height="17"/> | An open-source alternative to Perplexity AI, the AI-powered search engine |
| [gpt-researcher](https://github.com/assafelovic/gpt-researcher) | <img src="https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social" height="17"/> | An LLM-based autonomous agent that conducts deep local and web research on any topic and generates a long report with citations |
| [SurfSense](https://github.com/MODSetter/SurfSense) | <img src="https://img.shields.io/github/stars/MODSetter/SurfSense?style=social" height="17"/> | An open-source alternative to NotebookLM / Perplexity / Glean |
| [open-notebook](https://github.com/lfnovo/open-notebook) | <img src="https://img.shields.io/github/stars/lfnovo/open-notebook?style=social" height="17"/> | An open-source implementation of Notebook LM with more flexibility and features |
| [RD-Agent](https://github.com/microsoft/RD-Agent) | <img src="https://img.shields.io/github/stars/microsoft/RD-Agent?style=social" height="17"/> | Automate the most critical and valuable aspects of the industrial R&D process |
| [local-deep-researcher](https://github.com/langchain-ai/local-deep-researcher) | <img src="https://img.shields.io/github/stars/langchain-ai/local-deep-researcher?style=social" height="17"/> | Fully local web research and report writing assistant |
| [local-deep-research](https://github.com/LearningCircuit/local-deep-research) | <img src="https://img.shields.io/github/stars/LearningCircuit/local-deep-research?style=social" height="17"/> | An AI-powered research assistant for deep, iterative research |
| [maestro](https://github.com/murtaza-nasir/maestro) | <img src="https://img.shields.io/github/stars/murtaza-nasir/maestro?style=social" height="17"/> | An AI-powered research application designed to streamline complex research tasks |

[Back to Table of Contents](#table-of-contents)

### Training and Fine-tuning

| Project | Stars | Description |
|---|---|---|
| [heretic](https://github.com/p-e-w/heretic) | <img src="https://img.shields.io/github/stars/p-e-w/heretic?style=social" height="17"/> | Fully automatic censorship removal for language models |
| [sentence-transformers](https://github.com/huggingface/sentence-transformers) | <img src="https://img.shields.io/github/stars/huggingface/sentence-transformers?style=social" height="17"/> | A Python library for using and training embedding and reranker models for applications like retrieval augmented generation, semantic search, and more |
| [trl](https://github.com/huggingface/trl) | <img src="https://img.shields.io/github/stars/huggingface/trl?style=social" height="17"/> | Train transformer language models with reinforcement learning |
| [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) | <img src="https://img.shields.io/github/stars/OpenRLHF/OpenRLHF?style=social" height="17"/> | An easy-to-use, high-performance open-source RLHF framework built on Ray, vLLM, ZeRO-3 and HuggingFace Transformers |
| [slime](https://github.com/THUDM/slime) | <img src="https://img.shields.io/github/stars/THUDM/slime?style=social" height="17"/> | An LLM post-training framework for RL scaling |
| [Kiln](https://github.com/kiln-ai/kiln) | <img src="https://img.shields.io/github/stars/kiln-ai/kiln?style=social" height="17"/> | The easiest tool for fine-tuning LLM models, synthetic data generation, and collaborating on datasets |
| [OpenEnv](https://github.com/meta-pytorch/OpenEnv) | <img src="https://img.shields.io/github/stars/meta-pytorch/OpenEnv?style=social" height="17"/> | An interface library for RL post training with environments |
| [augmentoolkit](https://github.com/e-p-armstrong/augmentoolkit) | <img src="https://img.shields.io/github/stars/e-p-armstrong/augmentoolkit?style=social" height="17"/> | Train an open-source LLM on new facts |
| [RL](https://github.com/nvidia-nemo/rl) | <img src="https://img.shields.io/github/stars/nvidia-nemo/rl?style=social" height="17"/> | Scalable toolkit for efficient model reinforcement (NVIDIA NeMo) |
| [miles](https://github.com/radixark/miles) | <img src="https://img.shields.io/github/stars/radixark/miles?style=social" height="17"/> | An enterprise-facing reinforcement learning framework for LLM and VLM post-training, forked from and co-evolving with slime |
| [Gym](https://github.com/NVIDIA-NeMo/gym) | <img src="https://img.shields.io/github/stars/NVIDIA-NeMo/gym?style=social" height="17"/> | Evaluate and improve models and agents using environments (NVIDIA NeMo) |

[Back to Table of Contents](#table-of-contents)

### Security and Sandboxing

| Project | Stars | Description |
|---|---|---|
| [garak](https://github.com/NVIDIA/garak) | <img src="https://img.shields.io/github/stars/NVIDIA/garak?style=social" height="17"/> | The LLM vulnerability scanner from NVIDIA |
| [Guardrails](https://github.com/NVIDIA-NeMo/Guardrails) | <img src="https://img.shields.io/github/stars/NVIDIA-NeMo/Guardrails?style=social" height="17"/> | An open-source toolkit from NVIDIA for easily adding programmable guardrails to LLM-based conversational systems |
| [OpenShell](https://github.com/NVIDIA/OpenShell) | <img src="https://img.shields.io/github/stars/NVIDIA/OpenShell?style=social" height="17"/> | The safe, private runtime for autonomous AI agents from NVIDIA |
| [CubeSandbox](https://github.com/TencentCloud/CubeSandbox) | <img src="https://img.shields.io/github/stars/TencentCloud/CubeSandbox?style=social" height="17"/> | Instant, concurrent, secure & lightweight sandbox for AI agents |

[Back to Table of Contents](#table-of-contents)

### Miscellaneous

| Project | Stars | Description |
|---|---|---|
| [context7](https://github.com/upstash/context7) | <img src="https://img.shields.io/github/stars/upstash/context7?style=social" height="17"/> | Up-to-date code documentation for LLMs and AI code editors |
| [deepwiki-open](https://github.com/AsyncFuncAI/deepwiki-open) | <img src="https://img.shields.io/github/stars/AsyncFuncAI/deepwiki-open?style=social" height="17"/> | Open source DeepWiki: AI-powered wiki generator for GitHub/Gitlab/Bitbucket repositories |
| [cai](https://github.com/aliasrobotics/cai) | <img src="https://img.shields.io/github/stars/aliasrobotics/cai?style=social" height="17"/> | Cybersecurity AI (CAI), the framework for AI security |
| [speakr](https://github.com/murtaza-nasir/speakr) | <img src="https://img.shields.io/github/stars/murtaza-nasir/speakr?style=social" height="17"/> | A personal, self-hosted web application designed for transcribing audio recordings |
| [presenton](https://github.com/presenton/presenton) | <img src="https://img.shields.io/github/stars/presenton/presenton?style=social" height="17"/> | An open-source AI presentation generator and API |
| [OmniGen2](https://github.com/VectorSpaceLab/OmniGen2) | <img src="https://img.shields.io/github/stars/VectorSpaceLab/OmniGen2?style=social" height="17"/> | Exploration to advanced multimodal generation |
| [4o-ghibli-at-home](https://github.com/TheAhmadOsman/4o-ghibli-at-home) | <img src="https://img.shields.io/github/stars/TheAhmadOsman/4o-ghibli-at-home?style=social" height="17"/> | A powerful, self-hosted AI photo stylizer built for performance and privacy |
| [Observer](https://github.com/Roy3838/Observer) | <img src="https://img.shields.io/github/stars/Roy3838/Observer?style=social" height="17"/> | Local open-source micro-agents that observe, log and react, all while keeping your data private and secure |
| [mobile-use](https://github.com/minitap-ai/mobile-use) | <img src="https://img.shields.io/github/stars/minitap-ai/mobile-use?style=social" height="17"/> | A powerful, open-source AI agent that controls your Android or iOS device using natural language |
| [gabber](https://github.com/gabber-dev/gabber) | <img src="https://img.shields.io/github/stars/gabber-dev/gabber?style=social" height="17"/> | Build AI applications that can see, hear, and speak using your screens, microphones, and cameras as inputs |
| [promptcat](https://github.com/sevenreasons/promptcat) | <img src="https://img.shields.io/github/stars/sevenreasons/promptcat?style=social" height="17"/> | A zero-dependency prompt manager/catalog/library in a single HTML file |

[Back to Table of Contents](#table-of-contents)

## Hardware

| Resource | Type | Description |
|---|---|---|
| [Alex Ziskind](https://www.youtube.com/@AZisk) | YouTube <img src="https://img.shields.io/youtube/channel/subscribers/UCajiMK_CY9icRhLepS8_3ug?style=social" height="17"/> | Tests of PCs, laptops, GPUs etc. capable of running LLMs |
| [Digital Spaceport](https://www.youtube.com/@DigitalSpaceport) | YouTube <img src="https://img.shields.io/youtube/channel/subscribers/UCiaQzXI5528Il6r2NNkrkJA?style=social" height="17"/> | Reviews of various builds designed for LLM inference |
| [Donato Capitella](https://www.youtube.com/@donatocapitella) | YouTube <img src="https://img.shields.io/youtube/channel/subscribers/UCP0QFok6EimQYTMj5qOLNow?style=social" height="17"/> | Practical and insightful tutorials on running LLMs locally |
| [JetsonHacks](https://www.youtube.com/@JetsonHacks) | YouTube <img src="https://img.shields.io/youtube/channel/subscribers/UCQs0lwV6E4p7LQaGJ6fgy5Q?style=social" height="17"/> | Information about developing on NVIDIA Jetson Development Kits |
| [Miyconst](https://www.youtube.com/@Miyconst) | YouTube <img src="https://img.shields.io/youtube/channel/subscribers/UC8h2Sf-yyo1WXeEUr-OHgyg?style=social" height="17"/> | Tests of various types of hardware capable of running LLMs |
| [LocalForge - Local LLM hardware and model fit](https://localai.hexmobius.com/en?utm_source=github&utm_medium=awesome_list&utm_campaign=rameshkrishna_awesome_local_llms) | Web tool | Estimate memory fit and practical context for a target model, then compare GPU, laptop and server options with measured and unknown speed kept separate |
| [LLM Inference VRAM & GPU Requirement Calculator](https://app.linpp2009.com/en/llm-gpu-memory-calculator) | Web tool | Calculate how many GPUs you need to deploy LLMs |
| [ZLUDA](https://github.com/vosen/ZLUDA) | GitHub <img src="https://img.shields.io/github/stars/vosen/ZLUDA?style=social" height="17"/> | CUDA on non-NVIDIA GPUs |
| [Strix Halo AI Toolboxes](https://strix-halo-toolboxes.com/) | Website | Toolboxes for GenAI on AMD Ryzen AI MAX+: containerized environments for LLMs, image generation, and fine-tuning |
| [Strix Halo Wiki](https://strixhalo.wiki/) | Website | Important information and practical guides for systems powered by AMD Ryzen AI MAX and MAX+ processors |
| [ai-notes](https://github.com/paudley/ai-notes) | GitHub <img src="https://img.shields.io/github/stars/paudley/ai-notes?style=social" height="17"/> | Random AI notes for working with local models or playing around with random machine learning bits |

[Back to Table of Contents](#table-of-contents)

## Tutorials

### Models

| Resource | Type | Description |
|---|---|---|
| [Let's reproduce GPT-2 (124M)](https://www.youtube.com/watch?v=l8pRSuU81PU) | YouTube | Andrej Karpathy's walkthrough of reproducing GPT-2 (124M) from scratch |
| [nanochat](https://github.com/karpathy/nanochat) | GitHub <img src="https://img.shields.io/github/stars/karpathy/nanochat?style=social" height="17"/> | A full-stack implementation of an LLM like ChatGPT in a single, clean, minimal, hackable, dependency-lite codebase, designed to run on a single 8XH100 node |
| [Knowledge Distillation: How LLMs train each other](https://www.youtube.com/watch?v=jrJKRYAdh7I) | YouTube | How knowledge distillation lets LLMs train each other |
| [gguf-docs](https://github.com/iuliaturc/gguf-docs) | GitHub <img src="https://img.shields.io/github/stars/iuliaturc/gguf-docs?style=social" height="17"/> | Docs for GGUF quantization (unofficial) |
| [Embarrassingly Simple Self-Distillation Improves Code Generation](https://arxiv.org/pdf/2604.01193) | arXiv | Paper on improving code generation via simple self-distillation |

[Back to Table of Contents](#table-of-contents)

### Prompt Engineering

| Resource | Source | Description |
|---|---|---|
| [Prompt Engineering Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) | DAIR.AI <img src="https://img.shields.io/github/stars/dair-ai/Prompt-Engineering-Guide?style=social" height="17"/> | Guides, papers, lectures, notebooks and resources for prompt engineering |
| [Prompt Engineering by NirDiamant](https://github.com/NirDiamant/Prompt_Engineering) | NirDiamant <img src="https://img.shields.io/github/stars/NirDiamant/Prompt_Engineering?style=social" height="17"/> | A comprehensive collection of tutorials and implementations for prompt engineering techniques, from fundamental concepts to advanced strategies |
| [Prompting guide 101](https://services.google.com/fh/files/misc/gemini-for-google-workspace-prompting-guide-101.pdf) | Google | A quick-start handbook for effective prompts |
| [Prompt Engineering by Google](https://drive.google.com/file/d/1AbaBYbEa_EbPelsT40-vj64L-2IwUJHy/view) | Google | Prompt engineering whitepaper |
| [Prompt Engineering by Anthropic](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) | Anthropic | Prompt engineering documentation |
| [Prompt Engineering Interactive Tutorial](https://github.com/anthropics/courses/blob/master/prompt_engineering_interactive_tutorial/README.md) | Anthropic | Interactive prompt engineering tutorial |
| [Real world prompting](https://github.com/anthropics/courses/blob/master/real_world_prompting/README.md) | Anthropic | Real world prompting tutorial |
| [Prompt evaluations](https://github.com/anthropics/courses/blob/master/prompt_evaluations/README.md) | Anthropic | Prompt evaluations course |
| [system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | Community <img src="https://img.shields.io/github/stars/x1xhlol/system-prompts-and-models-of-ai-tools?style=social" height="17"/> | A collection of system prompts extracted from AI tools |
| [system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | Community <img src="https://img.shields.io/github/stars/asgeirtj/system_prompts_leaks?style=social" height="17"/> | A collection of extracted system prompts from popular chatbots like ChatGPT, Claude & Gemini |
| [Prompt from Codex](https://github.com/openai/codex/blob/main/codex-rs/core/prompt.md) | OpenAI <img src="https://img.shields.io/github/stars/openai/codex?style=social" height="17"/> | Prompt used to steer behavior of OpenAI's Codex |

[Back to Table of Contents](#table-of-contents)

### Context Engineering

| Resource | Stars | Description |
|---|---|---|
| [Context-Engineering](https://github.com/davidkimai/Context-Engineering) | <img src="https://img.shields.io/github/stars/davidkimai/Context-Engineering?style=social" height="17"/> | A frontier, first-principles handbook inspired by Karpathy and 3Blue1Brown for moving beyond prompt engineering to the wider discipline of context design, orchestration, and optimization |
| [Awesome-Context-Engineering](https://github.com/Meirtz/Awesome-Context-Engineering) | <img src="https://img.shields.io/github/stars/Meirtz/Awesome-Context-Engineering?style=social" height="17"/> | A comprehensive survey on context engineering: from prompt engineering to production-grade AI systems |

[Back to Table of Contents](#table-of-contents)

### Inference

| Resource | Stars | Description |
|---|---|---|
| [vLLM Production Stack](https://github.com/vllm-project/production-stack) | <img src="https://img.shields.io/github/stars/vllm-project/production-stack?style=social" height="17"/> | vLLM's reference system for K8S-native cluster-wide deployment with community-driven performance optimization |

[Back to Table of Contents](#table-of-contents)

### Agents

| Resource | Source | Description |
|---|---|---|
| [superpowers](https://github.com/obra/superpowers) | GitHub <img src="https://img.shields.io/github/stars/obra/superpowers?style=social" height="17"/> | An agentic skills framework & software development methodology that works |
| [GenAI Agents](https://github.com/NirDiamant/GenAI_Agents) | GitHub <img src="https://img.shields.io/github/stars/NirDiamant/GenAI_Agents?style=social" height="17"/> | Tutorials and implementations for various Generative AI agent techniques |
| [500+ AI Agent Projects](https://github.com/ashishpatel26/500-AI-Agents-Projects) | GitHub <img src="https://img.shields.io/github/stars/ashishpatel26/500-AI-Agents-Projects?style=social" height="17"/> | A curated collection of AI agent use cases across various industries |
| [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) | GitHub <img src="https://img.shields.io/github/stars/humanlayer/12-factor-agents?style=social" height="17"/> | Principles for building reliable LLM applications |
| [Agents towards production](https://github.com/NirDiamant/agents-towards-production) | GitHub <img src="https://img.shields.io/github/stars/NirDiamant/agents-towards-production?style=social" height="17"/> | End-to-end, code-first tutorials covering every layer of production-grade GenAI agents, with proven patterns and reusable blueprints for real-world launches |
| [agents.md](https://github.com/agentsmd/agents.md) | GitHub <img src="https://img.shields.io/github/stars/agentsmd/agents.md?style=social" height="17"/> | A simple, open format for guiding coding agents |
| [Agent Skills](https://github.com/agentskills/agentskills) | GitHub <img src="https://img.shields.io/github/stars/agentskills/agentskills?style=social" height="17"/> | A simple, open format for giving agents new capabilities and expertise |
| [skills](https://github.com/huggingface/skills) | Hugging Face <img src="https://img.shields.io/github/stars/huggingface/skills?style=social" height="17"/> | Hugging Face Skills — definitions for AI/ML tasks like dataset creation, model training and evaluation |
| [LLM Agents & Ecosystem Handbook](https://github.com/oxbshw/LLM-Agents-Ecosystem-Handbook) | GitHub <img src="https://img.shields.io/github/stars/oxbshw/LLM-Agents-Ecosystem-Handbook?style=social" height="17"/> | One-stop handbook for building, deploying, and understanding LLM agents with 60+ skeletons, tutorials, ecosystem guides, and evaluation tools |
| [601 real-world gen AI use cases](https://cloud.google.com/transform/101-real-world-generative-ai-use-cases-from-industry-leaders) | Google | 601 real-world gen AI use cases from the world's leading organizations |
| [A practical guide to building agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) | OpenAI | A practical guide to building agents |

[Back to Table of Contents](#table-of-contents)

### Retrieval-Augmented Generation

| Resource | Stars | Description |
|---|---|---|
| [Pathway AI Pipelines](https://github.com/pathwaycom/llm-app) | <img src="https://img.shields.io/github/stars/pathwaycom/llm-app?style=social" height="17"/> | Ready-to-run cloud templates for RAG, AI pipelines, and enterprise search with live data |
| [RAG Techniques](https://github.com/NirDiamant/RAG_Techniques) | <img src="https://img.shields.io/github/stars/NirDiamant/RAG_Techniques?style=social" height="17"/> | Various advanced techniques for Retrieval-Augmented Generation (RAG) systems |
| [Controllable RAG Agent](https://github.com/NirDiamant/Controllable-RAG-Agent) | <img src="https://img.shields.io/github/stars/NirDiamant/Controllable-RAG-Agent?style=social" height="17"/> | An advanced RAG solution for complex question answering using a sophisticated graph-based algorithm |
| [LangChain RAG Cookbook](https://github.com/lokeswaran-aj/langchain-rag-cookbook) | <img src="https://img.shields.io/github/stars/lokeswaran-aj/langchain-rag-cookbook?style=social" height="17"/> | A collection of modular RAG techniques, implemented in LangChain + Python |

[Back to Table of Contents](#table-of-contents)

### Miscellaneous

| Resource | Type | Description |
|---|---|---|
| [local-llm](https://github.com/jamesob/local-llm) | GitHub <img src="https://img.shields.io/github/stars/jamesob/local-llm?style=social" height="17"/> | Everything jamesob knows about running LLMs locally |
| [Self-hosted AI coding that just works](https://www.reddit.com/r/LocalLLaMA/comments/1lt4y1z/selfhosted_ai_coding_that_just_works/) | Reddit | Community write-up on a self-hosted AI coding setup |

[Back to Table of Contents](#table-of-contents)

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request to add a new resource, fix a description, or suggest a new category.
