# 🤖 terTATa-LLM: Dari Tabel dan Teks Menjadi Langkah Bisnis Strategis

terTATa-LLM adalah sistem AI berbasis LLM (Large Language Model) yang dirancang untuk membantu pelaku usaha, terutama UMKM, dalam mengekstrak wawasan strategis dari data tabel dan teks. Sistem ini merupakan hasil fine-tuning dari model **Nous-Hermes-2-Mistral-7B-DPO** menggunakan dataset **TAT-QA** dengan pendekatan _step-wise reasoning pipeline_ (Extractor–Reasoner–Executor).

## Use Case

- Menganalisis laporan keuangan internal (Excel)
- Menjawab pertanyaan kuantitatif & deskriptif berbasis tabel
- Memberikan rekomendasi bisnis dari data historis
- Dirancang untuk Bahasa Indonesia

## Arsitektur Sistem

- Base Model: [`Nous-Hermes-2-Mistral-7B-DPO`](https://huggingface.co/NousResearch/Nous-Hermes-2-Mistral-7B-DPO)
- Fine-tuning: PEFT LoRA + 4-bit quantization
- Dataset: [`TAT-QA`](https://huggingface.co/datasets/next-tat/TAT-QA)
- Prompting: 6-step pipeline (Instruction → Table → Text → Question)

## Update 
- Submisi terTATa-LLM: Top 10 Datathon RISTEK Fasilkom UI 2025
