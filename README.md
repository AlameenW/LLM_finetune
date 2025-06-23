# 🧠 LLM Finetune Project

## 📌 Description

An intelligent assistant designed to classify news articles into the following categories:  
**business, entertainment, politics, sport, tech** — using real-world, categorized data sources.

---

## 🔧 Fine-Tuning Procedure

### 1. Dataset Identification
- Collected real categorized news data from [@Huggingface](https://huggingface.co/).

### 2. Exploratory Data Analysis (EDA) & Pre-processing
- Removed duplicates and null values to ensure consistency.  
- Analyzed article titles in the **tech** category by tokenizing and generating a word cloud based on token frequency.

### 3. Data Formatting
- Split dataset into training and test sets.
- Converted to `.jsonl` format for compatibility with the OpenAI API.

### 4. Creating the Fine-Tuning Job
- Uploaded the preprocessed dataset to OpenAI.
- Fine-tuning was performed using the `gpt-3.5` base model.

### 5. Evaluation
- Compared the performance of the fine-tuned model with the base model using **accuracy** as the evaluation metric.

| Model           | Accuracy |
|----------------|----------|
| Base (gpt-3.5) | 82%      |
| Fine-tuned     | 94%      |

📈 **Net Accuracy Improvement**: **+12%**

---

## 📝 Notes
- Preprocessing included tokenization and visualization via word clouds.
- Evaluation was conducted using a held-out test dataset.
---


