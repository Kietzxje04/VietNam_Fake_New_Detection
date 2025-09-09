# VietNam_Fake_New_Detection

Deep learning project for Vietnamese fake news detection using Transformer models, especially **BERT**.  
This project provides datasets, preprocessing scripts, and training notebooks for research and practical applications in combating misinformation.  

---

## 📌 Dataset

We provide the **Vietnamese Fake News Dataset - Version 3**, which contains both **real** and **fake** news articles.  
This dataset is an extension of the previous version: [Vietnamese News Dataset Version 2](https://github.com/huynhtuan0106/Vietnamese-News-Dataset-Version2).

**Structure:**
- `processed/real.csv` → Real news articles
- `processed/fake.csv` → Fake news articles
- `deduplicated_articles_real.csv` → Deduplicated real articles
- `deduplicated_articles_fake.csv` → Deduplicated fake articles
- `url/` → Source URLs for real and fake news

---

## ⚙️ Models

This project implements multiple deep learning models for fake news detection:
- **BERT**
- **PhoBERT**
- **RoBERTa**
- Hybrid models (TF-IDF + PhoBERT, Word2Vec + PhoBERT, etc.)

Training notebooks are provided in the repo:
- `fake_news_detection_BERT.ipynb`
- `fake_news_detection_PhoBERT.ipynb`
- `fake_news_detection_RoBERTa.ipynb`
- `fake_news_detection_PhoBERT_TFIDF.ipynb`
- `fake_news_detection_PhoBERT_Word2Vec.ipynb`

---

## 🚀 How to Use

### 1. Clone the repository
```bash
git clone https://github.com/Kietzxje04/VietNam_Fake_New_Detection.git
cd VietNam_Fake_New_Detection
2. Install dependencies
It is recommended to use a virtual environment. Install required libraries:

bash
Copy code
pip install -r requirements.txt
(You may need to create requirements.txt with packages like torch, transformers, scikit-learn, pandas, etc.)

3. Run notebooks
Open Jupyter Notebook or VS Code and run the provided notebooks for training and evaluation.

📊 Results
Transformer-based models achieve significantly higher accuracy compared to traditional methods.

BERT and PhoBERT demonstrate strong performance for Vietnamese fake news detection.

(You can update this section later with your experiment results and evaluation metrics like Accuracy, F1-score, etc.)

📖 Citation
If you use this dataset or code in your research, please cite:

java
Copy code
@dataset{vietnam_fake_news_v3,
  author    = {Kietzxje04},
  title     = {Vietnamese Fake News Dataset - Version 3},
  year      = {2025},
  url       = {https://github.com/Kietzxje04/VietNam_Fake_New_Detection}
}
📜 License
This project is licensed under the MIT License.
You are free to use, modify, and distribute this work, provided proper attribution is given.

🙌 Acknowledgements
Dataset Version 2: huynhtuan0106

HuggingFace Transformers library for pre-trained models
