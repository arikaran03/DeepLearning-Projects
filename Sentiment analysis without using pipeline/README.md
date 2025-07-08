# Sentiment Analysis using DistilBERT (Without Pipeline)

This project performs sentiment analysis on a given sentence using the Hugging Face Transformers library, specifically with the **DistilBERT** model. Instead of using the high-level `pipeline` API, the notebook manually handles tokenization, model inference, and interpretation of outputs.

## 📚 Model Used

- `distilbert-base-uncased-finetuned-sst-2-english`
  - A lightweight and efficient version of BERT, fine-tuned on the SST-2 dataset for binary sentiment classification (positive/negative).

## 🧪 Steps Performed

1. **Load Tokenizer and Model**
   - Used `AutoTokenizer` and `AutoModelForSequenceClassification` from Hugging Face Transformers.

2. **Tokenization**
   - The input sentence is tokenized using the loaded tokenizer and converted into PyTorch tensors.

3. **Model Inference**
   - The tokenized input is passed to the model to obtain raw logits.

4. **Softmax & Label Prediction**
   - Logits are converted to probabilities using `torch.softmax`.
   - The label is determined using `argmax` and mapped back using `model.config.id2label`.

5. **Result Display**
   - Printed the input sentence, predicted label (`POSITIVE` or `NEGATIVE`), and probability distribution.

## 🛠 Libraries Used

- `transformers`
- `torch`

## 📌 Example Output

```text
Sentence: I love this!
Label: POSITIVE
Probabilities: [[0.03, 0.97]]
