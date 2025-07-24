# Deep Learning Projects

Welcome to the **Deep Learning Projects** repository! This collection demonstrates practical applications of deep neural networks across computer vision, NLP, and retrieval-augmented generation. Each folder contains a brief README, a Jupyter notebook, and any required assets. Explore the summaries below and refer to each project’s subdirectory for details.

---

## Projects

### 1. Breast Cancer Detection using Neural Network
- **Purpose**: Classify tumor samples as benign or malignant.
- **Dataset**: UCI Breast Cancer Wisconsin Diagnostic Dataset.
- **Model**: Multi‑layer Perceptron (dense neural network).
- **Key Results**: Achieved > 96% test accuracy, with ROC AUC of 0.98.
- **Location**: `DeepLearning-Projects/Breast Cancer Detection using Neural network/`

### 2. Digit Recognition using Convolutional Neural Network
- **Purpose**: Recognize handwritten digits (0–9).
- **Dataset**: MNIST.
- **Model**: Convolutional Neural Network (2 conv layers + pooling + dense layers).
- **Key Results**: > 99% test accuracy.
- **Location**: `DeepLearning-Projects/Digit Recognization using Convolutional Neural Network/`

### 3. Object Detection using Convolutional Neural Network
- **Purpose**: Detect and localize objects in images.
- **Dataset**: Custom/COCO‑style sample images.
- **Model**: CNN backbone with bounding‑box regression head.
- **Key Results**: Mean Average Precision (mAP) ~ 0.75 on sample validation set.
- **Location**: `DeepLearning-Projects/Object Detection using Convolutional Neural Network/`

### 4. Natural Language Processing Models
- **Purpose**: Demonstrate tokenization, embedding, and sequence modeling.
- **Dataset**: IMDb movie reviews (sentiment) & custom text corpus.
- **Models**:  
  - Word‑level embedding + LSTM for sentiment classification  
  - Transformer‑style encoder for masked language modeling  
- **Key Results**:  
  - Sentiment accuracy ~ 88%  
  - Masked LM perplexity ~ 15  
- **Location**: `DeepLearning-Projects/Natural Language Processing Models/`

### 5. Sentiment Analysis without Using Pipeline
- **Purpose**: Fine‑tune a pretrained DistilBERT model for sentiment classification.
- **Dataset**: IMDb or SST‑2.
- **Model**: HuggingFace’s `distilbert-base-uncased` (no pipeline API).
- **Key Results**: Achieved ~ 90% accuracy after 3 epochs of fine‑tuning.
- **Location**: `DeepLearning-Projects/Sentiment analysis without using pipeline/`

### 6. Retrieval-Augmented Generation Implementation
- **Purpose**: Combine dense retrieval with a generative LLM for open‑domain QA.
- **Dataset**: Wikipedia passages (indexed) + custom question set.
- **Components**:  
  - Dense retriever (e.g. DPR)  
  - GPT‑style generator for answer synthesis  
- **Key Results**: Improved answer relevance by 15% vs. generation‑only baseline.
- **Location**: `DeepLearning-Projects/Retrieval-Augmented Generation Implementation/`

---

_For full instructions, code, and environment details, please open the README.md inside each project folder._  
