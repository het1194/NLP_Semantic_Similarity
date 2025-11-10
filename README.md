# Text Similarity Classification Project

This project uses an NLP model (**InferSent**) to determine whether two text descriptions refer to the same security instrument.

It works by converting each text description into a numerical vector (embedding) and then engineering features based on the mathematical similarity and distance between these vectors. A model is then trained on these features to make a final **"same"** or **"different"** prediction.

## How to Run

### 1. Install Dependencies

Make sure you have **Python 3** and the required libraries. You can install everything using:

```bash
pip install torch kagglehub nltk matplotlib seaborn scikit-learn xgboost lightgbm pandas numpy requests
```
## 2. Run the Jupyter Notebook

Open and run the cells in **`NLP_Sentiment_Analysis Project.ipynb`**.

## First-Time Setup (Downloads)

When you run the notebook for the first time, it will automatically download two required files. This may take several minutes:

- **InferSent Model:** `infersent2.pkl` (saved to `encoder/`)
- **Word Embeddings:** `crawl-300d-2M.vec.zip` (saved to `fastText/`)

## Output

After execution, the notebook will generate several performance plots and save the final test predictions to test_predictions_enhanced.csv
