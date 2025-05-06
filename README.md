# finalprojectstat

Selesai berpikir selama beberapa detik


The objective of this analysis was to evaluate and compare the sentiment‑classification performance of five neural‑network architectures—CNN, LSTM, BiLSTM, CNN‑LSTM and CNN‑BiLSTM—on user reviews of the “Access by KAI” mobile application, gathered from both the Google Play Store and the Apple App Store.

First, the raw review texts were collected and cleaned; then each review was tokenized and converted into vector embeddings. To address class imbalance, a random over‑sampling procedure was applied to create both balanced and unbalanced training sets. Five models were then trained and tested under both conditions:

1. **CNN**, for local feature extraction
2. **LSTM**, for modeling sequential dependencies
3. **BiLSTM**, for bidirectional context
4. **CNN‑LSTM**, combining convolutional feature extraction with LSTM sequence modeling
5. **CNN‑BiLSTM**, combining convolutional feature extraction with bidirectional LSTM

All models were evaluated using overall accuracy as well as F1‑scores for the positive and negative classes.

The hybrid **CNN‑LSTM** model achieved the best results in both scenarios. Without oversampling, it reached 91.66% accuracy, with F1‑scores of 63.82% (positive) and 95.28% (negative). With oversampling, it attained 90.76% accuracy, with F1‑scores of 61.70% (positive) and 94.76% (negative). These findings demonstrate that integrating CNN’s local‑feature capabilities with LSTM’s sequential‑modeling strengths yields superior sentiment‑classification performance compared to standalone or alternative hybrid architectures.
