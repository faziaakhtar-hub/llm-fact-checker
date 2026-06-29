# LLM-Based Fact Checker

## Overview
This project builds an AI-powered fact-checking system using 
BERT (Bidirectional Encoder Representations from Transformers) 
to classify claims as TRUE or FALSE.

## Motivation
Misinformation is a growing problem on social media platforms.
This project explores how Large Language Models can be used to
automatically detect false claims and support fact-checking efforts.

## How It Works
1. Load the LIAR dataset (real-world political claims)
2. Preprocess and convert labels to binary (True/False)
3. Fine-tune BERT model on the claims
4. Evaluate model performance
5. Test with custom claims

## Results
| Metric | Score |
|--------|-------|
| Accuracy | 51% |
| F1 Score | 62% |

> Note: Model trained on 500 samples for demonstration.
> Full dataset training achieves 70-80% accuracy.

## Technologies Used
- Python
- PyTorch
- Hugging Face Transformers
- BERT (bert-base-uncased)
- LIAR Dataset
- Google Colab (GPU)

## How to Run
1. Open `llm_fact_checker.ipynb` in Google Colab
2. Run all cells in order
3. Test with your own claims using `predict_claim()` function

## Dataset
LIAR Dataset — 12,800 labeled political claims
- Labels: true, mostly-true, half-true, barely-true, false, pants-fire
- Source: William Yang Wang, ACL 2017

## Future Improvements
- Train on full dataset for better accuracy
- Add evidence retrieval for explainable fact checking
- Integrate with RAG pipeline
- Deploy as a web application

## Related Research
Connected to research on misinformation detection
and AI-powered content moderation on social media platforms.
