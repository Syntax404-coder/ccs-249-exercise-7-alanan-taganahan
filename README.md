# HMM-Based NER

A minimal implementation of a Hidden Markov Model for Named Entity Recognition, from data loading through Viterbi decoding.

## Features
- **Data Prep**: Load CSV with `Sentence` (words) and `Tag` (lists of labels).  
- **HMM Class**:  
  - Tag transition, emission, and start probability estimation  
  - Viterbi algorithm for best-tag sequence  
- **Evaluation**: 80/20 train/test split, reports accuracy.  
- **Demo**: Predict tags for `["Manila", "is", "the", "capital", "of", "the", "Philippines"]`

## Usage
1. Install dependencies: `pandas`.  
2. Place `ner.csv` in working dir.  
3. Run the notebook or `python your_notebook.py`.

## Next
- Handle unknown words via suffix/prefix features  
- Compare with CRF models  
