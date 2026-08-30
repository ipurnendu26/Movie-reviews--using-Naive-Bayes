# Movie Review Sentiment with Naive Bayes

A Jupyter notebook that builds a classical NLP sentiment classifier for movie reviews using text preprocessing, bag-of-words features, and Naive Bayes.

## Project file

- `Movie reviews.ipynb`: exploratory analysis, vectorization, training, and evaluation

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

## Skills demonstrated

- Text cleaning and tokenization
- Sparse feature construction
- Probabilistic text classification
- Confusion-matrix and classification-metric interpretation

## Limitations

This is a learning baseline. Reported notebook results, if any, apply only to its exact split and preprocessing. A stronger study would document data provenance, prevent duplicate-review leakage, use stratified cross-validation, compare TF-IDF and linear baselines, analyze negation and domain shift, and test calibration.

## License

[MIT](LICENSE)
