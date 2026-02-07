<img width="1920" height="1044" alt="Screenshot 2026-02-07 at 10 07 47 PM" src="https://github.com/user-attachments/assets/29e71b29-1363-4574-8f69-c39b6a1134f6" /># Smart Clinical Report Reader  
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

##  Demo Screenshot

<img width="1920" height="1044" alt="Screenshot 2026-02-07 at 10 07 47 PM" src="https://github.com/user-attachments/assets/8ab70d6b-8ab7-4e02-81ad-47a7baf8727c" />

<img width="1920" height="1042" alt="Screenshot 2026-02-07 at 10 08 12 PM" src="https://github.com/user-attachments/assets/b9e7739c-da85-4fae-b8c5-f36a24013f65" />



## ⚡ Quick Start

1. Clone the repo:
   ```bash
   git clone https://github.com/sufirumii/Smart-Clinical-Report-Reader-Powered-by-Qwen2.5-VL-32B.git
   cd Smart-Clinical-Report-Reader-Powered-by-Qwen2.5-VL-32B

Install dependencies:Bashpip install gradio openai PyPDF2 pdfplumber requests
Get a Hugging Face token (read access is enough):
Go to https://huggingface.co/settings/tokens
Create or copy your token

Set your token in the code (replace the placeholder):PythonHF_TOKEN = "hf_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"  # ← your token here
Run the app:Bashpython your_script_name.py   # usually the file with demo.launch()Open http://127.0.0.1:7860 (or public URL if you enable --share)

Advanced Setup (Recommended for Best PDF & Video Handling)
Bashpip install git+https://github.com/huggingface/transformers accelerate
pip install qwen-vl-utils[decord]==0.0.8   # faster video if needed in future
Important Disclaimer
This tool is built for educational and research purposes only.

It is not a medical device.
It is not intended for clinical decision-making, diagnosis, or treatment.
All outputs must be reviewed and verified by qualified healthcare professionals.
PubMed data is retrieved in real-time but may have delays or rate limits.
Always consult licensed medical experts for any health-related decisions.

License
Apache License 2.0
See the LICENSE file for details.
Connect

LinkedIn: Rumi Sufi
GitHub: @sufirumii
Hugging Face Model: Qwen2.5-VL-32B-Instruct

Acknowledgments

Alibaba Cloud Qwen Team for the excellent Qwen2.5-VL series
Hugging Face for inference API & transformers library
NCBI for PubMed E-utilities API
Gradio team for the beautiful UI framework

Contributions, feedback, and stars are very welcome! 🚀
#AIinHealthcare #HealthcareAI #MedicalAI #ClinicalAI #RAG #LLM #Qwen #Qwen2.5VL #HuggingFace #PubMed #HealthTech #DigitalHealth #MedicalInformatics #ClinicalDecisionSupport #VisionLanguageModel #GenerativeAI #RetrievalAugmentedGeneration #DeepLearning #MachineLearning #ArtificialIntelligence
