# A Technical Primer on Large Language Models

This repository contains a comprehensive technical onboarding guide for users deploying open-weight Large Language Models (LLMs) on the **LUMI supercomputer**.

The guide serves as an educational resource to bridge the gap between high-level AI concepts and the hardware realities of running models at scale on AMD MI250X GPUs. The content is fairly technical—diving into how architectures and hardware interact—but it avoids getting bogged down in overly complex, low-level code implementations. It's the perfect middle ground for understanding *how* things work under the hood without needing to be an expert in machine learning engineering.

## 📖 What's Inside

The primer covers the critical architectural and infrastructure concepts needed to successfully run inference and fine-tuning workloads:

* **Open-Weight Models:** Understanding parameter counts, benchmarks, and the difference between Base and Instruct (Chat) models.
* **Architectures:** The performance and memory trade-offs between Dense models (e.g., Llama 3) and Mixture of Experts (MoE) models (e.g., Qwen3.6, Mixtral).
* **Under the Hood:** How Attention mechanisms work (MHA, MQA, GQA) and the critical role of the KV Cache in VRAM.
* **Inference at Scale:** Hardware bottlenecks (Compute vs. Memory Bandwidth), text generation parameters, and why **vLLM** is the recommended engine on LUMI.
* **Multi-GPU Strategies:** When and how to use Tensor Parallelism (TP), Pipeline Parallelism (PP), and Data Parallelism (DP).
* **Customizing Models:** A technical comparison of Full-Parameter Fine-Tuning, PEFT/LoRA, Quantization, and RAG (Retrieval-Augmented Generation).
* **LUMI Hardware Sizing:** Practical rules of thumb for calculating VRAM requirements and requesting the correct number of GCDs.

## 🎯 Target Audience

This guide is written for those who are already comfortable with the high-level, non-technical basics of Large Language Models (like what a prompt is or how chatbots work) and are ready to look beneath the surface. If you want a solid technical understanding of how these models actually operate on supercomputer hardware—without getting lost in the weeds of complex machine learning code—this guide is for you.
