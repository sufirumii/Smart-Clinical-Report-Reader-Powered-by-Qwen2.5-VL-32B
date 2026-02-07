# Smart Clinical Report Reader  
**Powered by Qwen2.5-VL-32B-Instruct with PubMed RAG**

AI-powered tool that analyzes uploaded PDF clinical reports, answers natural-language questions conversationally, grounds answers in the document + real-time PubMed literature, and generates structured outputs like summaries and SOAP notes — all with proper citations.

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Qwen2.5--VL--32B-orange)](https://huggingface.co/Qwen/Qwen2.5-VL-32B-Instruct)

##  Features

- Upload PDF clinical reports → instant intelligent extraction & analysis
- Ask follow-up questions naturally (multi-turn conversation with memory)
- Evidence-based answers combining report content + real-time PubMed search (up to 5 articles)
- Automatic citations & references to sources
- Generate structured clinical documentation:
  - SOAP notes
  - Concise summaries
- Professional hospital-grade Gradio UI (clean, responsive, no cartoonish elements)
- Fully cloud-based inference — no local GPU required (uses Hugging Face Inference API)
- Single-file architecture (~700 lines of clean Python)

##  Powered By

- **Core Model**: [Qwen/Qwen2.5-VL-32B-Instruct](https://huggingface.co/Qwen/Qwen2.5-VL-32B-Instruct) (33B parameters, vision-language model optimized for document understanding, complex reasoning, structured outputs)
- **RAG Pipeline**: Hybrid retrieval — local document context + PubMed E-utilities API
- **UI Framework**: Gradio
- **PDF Processing**: pdfplumber (primary) + PyPDF2 (fallback)
- **API Client**: OpenAI-compatible client via Hugging Face router
- **PubMed Integration**: NCBI E-utilities (rate-limited & respectful)

##  Demo Screenshots

<img width="1920" height="1044" alt="1" src="https://github.com/user-attachments/assets/b363d5fd-9900-42cf-a3e9-5d052b26918e" />

<img width="1920" height="1042" alt="2" src="https://github.com/user-attachments/assets/17e76bbd-f868-4071-ba5d-a7654eee1162" />


## ⚡ Quick Start

1. Clone the repo:
   ```bash
   git clone https://github.com/sufirumii/Smart-Clinical-Report-Reader-Powered-by-Qwen2.5-VL-32B.git
   cd Smart-Clinical-Report-Reader-Powered-by-Qwen2.5-VL-32B
