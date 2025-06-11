# 📘Few-shot & Zero-shot Translation

This repository explores **few-shot** and **zero-shot** machine translation (NMT) using state-of-the-art multilingual models like **mBART** and **M2M-100**. It covers techniques such as:

- 🔁 Back-translation
- 🔀 Pivot translation
- 🌐 Zero-shot inference
- 🧠 Cross-lingual transfer from high- to low-resource languages

The focus is especially on low-resource Indian languages like **Telugu** and **Kannada**.

---

## 📁 Folder Structure

```

fewshot-zeroshot-translation/
│
├── Notebooks/
│   ├── 01\_mbart\_fewshot\_backtranslation.ipynb
│   ├── 02\_m2m100\_pivot\_translation\_kn\_en\_hi.ipynb
│   ├── 03\_mbart\_m2m100\_zeroshot\_translation\_examples.ipynb
│   ├── 04\_fewshot\_crosslingual\_transfer\_template.ipynb
│
├── README.md
├── requirements.txt
└── LICENSE

````

---

## 📓 Notebooks Overview

### 1. Few-shot Back-Translation (MBart)
- **Model:** `facebook/mbart-large-50-many-to-many-mmt`
- **Dataset:** `HackHedron/English_Telugu_Parallel_Corpus`
- **Method:** Uses few-shot fine-tuning and back-translation to improve English ↔ Telugu translation quality.
- **Status:** Complete and tested

 `Notebooks/01_mbart_fewshot_backtranslation.ipynb`

---

### 2. Pivot Translation: Kannada → English → Hindi (M2M-100)
- **Model:** `facebook/m2m100_418M`
- **Method:** Uses **English** as a pivot to translate **Kannada → Hindi**.
- **Status:** Complete and tested

 `Notebooks/02_m2m100_pivot_translation_kn_en_hi.ipynb`

---

## 🧪 Experimental / Conceptual

### 3. Zero-shot Multilingual Translation Examples
- **Models:** mBART and M2M-100
- **Examples:** Tamil → Kannada, English → Hindi
- **Purpose:** Showcase multilingual model's zero-shot capabilities.
- **Status:** Contains runnable examples; partly explored

 `Notebooks/03_mbart_m2m100_zeroshot_translation_examples.ipynb`

---

### 4. Few-shot + Cross-lingual Transfer (Code Template)
- **Idea:** First fine-tune on Hindi ↔ English (high-resource), then transfer knowledge to Kannada ↔ English (low-resource).
- **Approach:** Uses mBART with custom preprocessing and training logic.
- **Status:** Code complete but not executed yet

 `Notebooks/04_fewshot_crosslingual_transfer_template.ipynb`

---

## 🧠 Techniques Covered

- ✅ Few-shot Machine Translation
- 🔁 Back-Translation
- 🌐 Zero-shot Translation
- 🔄 Pivot-based Translation
- 🔀 Cross-lingual Transfer

---

## 💻 Run Locally

```bash
git clone https://github.com/Koushim/fewshot-zeroshot-translation.git
cd fewshot-zeroshot-translation
pip install -r requirements.txt
````

---

## 📦 Requirements

```text
transformers
datasets
torch
accelerate
```

---

## 📌 Notes

* ✅ The notebooks under `Experimental / Conceptual` are included **for research completeness and future development**.
* 📈 These could be converted into fully working pipelines in future iterations.

---

## ✍️ Author

**Koushik Reddy**
🔗 [Hugging Face](https://huggingface.co/Koushim) | [LinkedIn](https://www.linkedin.com/in/koushik-reddy-k-790938257)

---

## 📌 License

This project is open source and available under the [Apache License](LICENSE).
