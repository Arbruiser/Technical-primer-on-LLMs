# A Technical Primer on Large Language Models

This repository hosts an educational onboarding guide for running open-weight Large Language Models (LLMs) on the **LUMI supercomputer**. 

If you're already familiar with the basics of LLMs—like what a prompt is, how chatbots work, or why everyone is talking about AI—but you're ready to look under the hood, this guide is for you. 

It is designed to bridge the gap between high-level concepts and the hardware realities of running models on AMD MI250X GPUs. The material is fairly technical, diving into model architectures and hardware interactions, but it avoids getting bogged down in low-level code or complex machine learning math. It's the perfect middle ground for building a solid, working understanding of how these powerful models actually operate on supercomputing infrastructure.

## 📖 What You'll Learn

The guide breaks down the critical concepts needed to successfully run inference and fine-tuning workloads on LUMI:

* **Open-Weight Models:** The real meaning behind parameter counts, benchmarks, and the practical difference between Base and Instruct (Chat) models.
* **Architectures:** The performance and memory trade-offs between standard Dense models (e.g., Llama 3) and Mixture of Experts (MoE) models (e.g., Qwen3.6, Mixtral).
* **Under the Hood:** A look at how Attention mechanisms work (MHA, MQA, GQA) and why the KV Cache is so critical to your GPU's memory.
* **Inference at Scale:** Understanding hardware bottlenecks, text generation parameters, and why **vLLM** is the recommended engine for the job.
* **Parallelism:** When and how to split massive models across multiple GPUs using Tensor, Pipeline, and Data Parallelism.
* **Customizing Models:** A practical comparison of Full-Parameter Fine-Tuning, PEFT/LoRA, Quantization, and Retrieval-Augmented Generation (RAG).
* **Sizing Your Workload:** Straightforward rules of thumb for calculating VRAM requirements and requesting the right number of GCDs on LUMI.
