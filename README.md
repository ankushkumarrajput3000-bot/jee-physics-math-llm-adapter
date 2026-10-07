# 🎓 JEE Physics & Math LLM Fine-Tuner (QLoRA)

An end-to-end parameter-efficient fine-tuning (PEFT) pipeline adapting **Qwen-2.5-Math-7B** for multi-step, structured Chain-of-Thought reasoning on JEE Advanced Physics and Mathematics problems.

---

## 📌 Features

- **Fine-Tuned Architecture:** Leveraged 4-bit QLoRA via **Unsloth** for low-VRAM training.
- **Chain-of-Thought (CoT) Prompting:** Formatted data to force step-by-step reasoning (Free Body Diagrams, Component Resolution, Symbolic Integration).
- **LaTeX Generation:** Trained model to output clean, structured LaTeX for math/physics notation.

---

## 🛠️ Tech Stack

- **Model:** `Qwen2.5-Math-7B-Instruct`
- **Frameworks:** PyTorch, Hugging Face `transformers`, `datasets`, `trl`
- **Optimization:** Unsloth, QLoRA (bitsandbytes 4-bit quantization)
- **Hardware Target:** Google Colab / Single T4 GPU (16GB VRAM)

---

## 🚀 Getting Started

### 1. Install Dependencies
```bash
pip install -r requirements.txt
