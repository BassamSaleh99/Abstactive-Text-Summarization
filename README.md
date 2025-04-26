# Abstactive-Text-Summarization

---

### Project Overview

This project implements an **abstractive text summarization** model using a **Seq2Seq architecture with attention mechanism** based on LSTM layers.

- **Model Type**: Encoder-Decoder with Attention (Stacked LSTMs)
- **Training Framework**: TensorFlow / Keras
- **Evaluation Metric**: ROUGE scores (ROUGE-1, ROUGE-2, ROUGE-L)

### Dataset

The dataset used is moderately noisy, containing some irrelevant or low-quality text data. This has an impact on the final quality of generated summaries.

### Results

After training, the model achieved the following ROUGE F1-scores on the validation set:

- **ROUGE-1 F1 Score**: 0.1646
- **ROUGE-2 F1 Score**: 0.0202
- **ROUGE-L F1 Score**: 0.1275

### Challenges

- **Limited Data Quality**: The dataset includes noise and inconsistencies, affecting model learning.
- **Training Time**: Due to the model’s size and computational complexity, training is very slow and requires a lot of time. Therefore, it was not feasible to experiment with many hyperparameter configurations.
- **Model Simplicity**: The current architecture is relatively simple compared to state-of-the-art models like Transformers, which limits performance.

### Future Improvements

- Use larger and cleaner datasets.
- Switch to Transformer-based architectures.
- Fine-tune hyperparameters if more computational resources become available.