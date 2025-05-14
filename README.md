## Trigram Language Model

- **Purpose:** Predict the next word in a sentence.
- **Accuracy:** 12.66%
- **Generated Sentence:** Mostly incoherent or generic (`-DOCSTART-`, `international`, `<unk>`, etc.).
- **Limitations:** Not designed for NER tasks — it's a language model, not a sequence labeler.

---

## Hidden Markov Model 

- **Purpose:** Predict NER tags (like `B-LOC`, `I-PER`, `O`, etc.) for each word.
- **Accuracy:** 68.27%
- **Tagging Sentence:** Provides valid though lackluster NER tag predictions.

---

## Comparison

| Model        | Purpose            | Accuracy      | Relevance to NER     | Evaluation             |
|--------------|--------------------|---------------|-----------------------|-------------------------|
| Trigram LM   | Predict next word  | 12.66%        | [X] Not for NER         | Weak for NER tasks      |
| HMM_NER      | Predict NER tags   | 68.27%        | [/] Designed for NER    | Likely much better      |

##Text Classification Using LSTM and Trigram LM

##Trigram
Evaluation Metrics:
Accuracy         : 12.66%
Top-3 Accuracy   : 16.79%
Perplexity       : 12401.77

##LSTM
LSTM Evaluation Metrics:
Accuracy         : 15.22%
Top-3 Accuracy   : 25.31%
Perplexity       : 1258.34

LSTM Performs Better
Higher Accuracy → LSTM makes more correct predictions overall.

Higher Top-3 Accuracy → LSTM better captures multiple likely options.

Much Lower Perplexity → LSTM produces much more confident and coherent word distributions.

