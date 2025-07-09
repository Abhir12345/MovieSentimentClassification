# 🎬 MovieSentimentClassification

Sentiment classification on movie reviews using a Simple RNN model trained on transformer-generated embeddings.

---

## 🧾 Summary

- **Dataset**: [IMDB Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews), a balanced dataset of ~50,000 movie reviews.
- **Embeddings**: Used [`SentenceTransformer`](https://www.sbert.net/) with the `all-MiniLM-L6-v2` model (a distilled version of BERT) to generate 384-dimensional embeddings.
- **Model**: A `SimpleRNN` architecture with `Dropout` layers (dropout rate = 0.2).
- **Training**: 
  - Split into training and test sets.
  - Trained for **50 epochs**.
- **Note**: The transformer handled basic text cleaning internally while generating embeddings.

---

## 📈 Results

- **Training Accuracy**: ~90%
- **Validation Accuracy**: ~82%

---

## 🚀 Model Demo

🔗 [Live Model Here](https://abhinandan12345-simplemoviesentimentpredictor.hf.space/?__theme=system&deep_link=MfRyFAgZHP4)

---

## 📁 Files in Repo

- `notebook.ipynb`: Full implementation and training workflow.
- `RNNMODEL.keras`: Trained model file.
- `requirements.txt`: Dependencies for replicating the environment.

---

## 📌 Requirements

Install dependencies using:
```bash
pip install -r requirements.txt
