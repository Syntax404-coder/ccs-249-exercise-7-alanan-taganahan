## Trigram Language Model

- **Purpose:** Predict the next word in a sentence.
- **Accuracy:** 12.66%
- **Generated Sentence:** Mostly incoherent or generic (`-DOCSTART-`, `international`, `<unk>`, etc.).
- **Limitations:** Not designed for NER tasks — it's a language model, not a sequence labeler.

---

## Hidden Markov Model 

- **Purpose:** Predict NER tags (like `B-LOC`, `I-PER`, `O`, etc.) for each word.
- **Accuracy:** *(Not explicitly printed in the shared output, but computed using tag-level correctness)*
- **Tagging Sentence:** Appears to provide valid NER tag predictions (though no exact accuracy reported in this snippet).

---

## Comparison

| Model        | Purpose            | Accuracy      | Relevance to NER     | Evaluation             |
|--------------|--------------------|---------------|-----------------------|-------------------------|
| Trigram LM   | Predict next word  | 12.66%        | [X] Not for NER         | Weak for NER tasks      |
| HMM_NER      | Predict NER tags   | *(Not shown)* | [/] Designed for NER    | Likely much better      |
