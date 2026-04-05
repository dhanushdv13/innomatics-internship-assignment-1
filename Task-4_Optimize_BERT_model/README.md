# BERT Fine-Tuning for Sentiment Analysis

## 📌 Project Overview

This project demonstrates fine-tuning of a pre-trained BERT model for sentiment analysis using a real-world dataset. The objective is to classify text reviews into positive or negative sentiments using transformer-based deep learning techniques.

---

##  Objectives

- Understand how BERT works for text classification
- Perform fine-tuning using Hugging Face Transformers
- Apply tokenization using pre-trained models
- Evaluate model performance using classification metrics
- Conduct experiments and analyze results

---

## Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- Scikit-learn
- Jupyter Notebook

---

## Dataset

- Dataset Used: IMDb Movie Reviews Dataset
- Source: Kaggle
- Contains 50,000 movie reviews labeled as positive or negative

---

## Implementation Steps

1. Data Preprocessing
   - Cleaned text (removed HTML, special characters)
   - Converted labels to numeric format

2. Data Splitting
   - Train: 80%
   - Validation: 10%
   - Test: 10%

3. Tokenization
   - Used `bert-base-uncased` tokenizer
   - Applied padding and truncation

4. Model Building
   - Used `AutoModelForSequenceClassification`
   - Loaded pre-trained BERT model

5. Fine-Tuning
   - Optimizer: AdamW
   - Learning Rate: 2e-5
   - Epochs: 1 (CPU-based training)

6. Evaluation
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Confusion Matrix

---

## Experiments

- Full BERT fine-tuning (all layers trained)
- Conceptual comparison with:
  - Freezing BERT layers
  - Fine-tuning last few layers

---

## Results

- Training Loss: ~0.33
- Model shows strong learning capability even with limited training
- BERT outperforms traditional ML models due to contextual understanding

---

## Limitations

- Training performed on CPU (high execution time)
- Limited epochs due to computational constraints
- Full evaluation on test set may be time-consuming

---

## Future Improvements

- Use GPU for faster training
- Increase number of epochs
- Try lightweight models like DistilBERT
- Apply hyperparameter tuning

---

## 📌 Conclusion

This project successfully demonstrates the implementation of BERT fine-tuning for sentiment analysis. It highlights the effectiveness of transformer-based models in understanding context and improving classification performance.

---

## 🔗 Repository Structure
```pre
GEN_AI_MODULE/
│
├── Task-1/
├── Task-2_Sentiment_Analysis/
├── Task-3_Chatbot_HuggingFace/
├── Task-4_Optimize_BERT_model/
│ └── bert_model_optimization.ipynb
│
└── README.md
```


---

## 📎 Notes

- Large files such as datasets and training outputs are excluded using `.gitignore`
- Ensure all dependencies are installed before running the notebook

---

## 👨‍💻 Author

Pavanchandra Devang L  
