# 🧠 AI Doctor – Fine-Tuned DeepSeek-R1

An AI-powered medical assistant built by fine-tuning **DeepSeek-R1** using modern techniques like **LoRA / QLoRA**.
This project demonstrates how large language models can be adapted for **health-related question answering and guidance**.

---

## 🚀 Project Overview

The **AI Doctor** is a fine-tuned LLM designed to:

* Answer general medical queries
* Provide basic health guidance
* Simulate a conversational medical assistant

> ⚠️ Disclaimer: This project is for **educational and research purposes only**. It is NOT a substitute for professional medical advice.

---

## 🧩 Features

* 🧠 Fine-tuned **DeepSeek-R1 model**
* ⚡ Efficient training using **LoRA / QLoRA**
* 💬 Conversational AI interface
* 📚 Domain-specific responses (healthcare)
* 🖥️ Runs on limited hardware (with quantization)

---

## 🛠️ Tech Stack

* **Python**
* **Transformers (Hugging Face)**
* **Unsloth (for fast fine-tuning)**
* **PyTorch**
* **Datasets**
* **PEFT (LoRA/QLoRA)**

---

## 📂 Project Structure

```
AI_DOCTOR_Finetuned_Deepseek-R1/
│── AI_DOCTOR_Finetuned_Deepseek_R1.ipynb   # Main notebook
│── README.md                               # Project documentation
```

---

## ⚙️ How It Works

1. Load the base **DeepSeek-R1** model
2. Apply **quantization (4-bit)** for efficiency
3. Fine-tune using **LoRA adapters**
4. Train on domain-specific dataset (medical Q&A)
5. Generate responses using the fine-tuned model

---

## ▶️ How to Run

### 🔹 Option 1: Google Colab (Recommended)

1. Open the notebook:
   👉 [Run on Colab](https://colab.research.google.com/github/ArnavAdhikary05/AI_DOCTOR_Finetuned_Deepseek-R1/blob/main/AI_DOCTOR_Finetuned_Deepseek_R1.ipynb)

2. Run all cells step-by-step

---

### 🔹 Option 2: Local Setup

#### 1. Clone the repo

```bash
git clone https://github.com/ArnavAdhikary05/AI_DOCTOR_Finetuned_Deepseek-R1.git
cd AI_DOCTOR_Finetuned_Deepseek-R1
```

#### 2. Install dependencies

```bash
pip install -r requirements.txt
```

#### 3. Run the notebook

```bash
jupyter notebook
```

---

## 💾 Model Usage

If you have saved LoRA adapters:

```python
from transformers import AutoModelForCausalLM
from peft import PeftModel

base_model = AutoModelForCausalLM.from_pretrained("deepseek-model")
model = PeftModel.from_pretrained(base_model, "your-adapter-path")
```

---

## 📊 Hardware Requirements

| Setup   | Requirement             |
| ------- | ----------------------- |
| Minimum | 8GB RAM                 |
| GPU     | 4GB+ VRAM (recommended) |
| Best    | Google Colab (Free/Pro) |

---

## 🔒 Limitations

* Not medically certified
* May produce incorrect or unsafe advice
* Depends heavily on training data quality

---

## 📌 Future Improvements

* Add real-time medical APIs
* Improve dataset quality
* Deploy as a web app
* Add voice assistant support
* Integrate with wearable health data

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork the repo and submit pull requests.

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 👨‍💻 Author

**Arnav Adhikary**

* GitHub: https://github.com/ArnavAdhikary05

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!

---
