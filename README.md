# Question Answering with Transformers

An extractive Question Answering project that uses pretrained Transformer models to identify answers from a given passage of text.

The project explores and compares four models fine-tuned for Question Answering using the SQuAD dataset.

## Models Compared

- DistilBERT
- BERT
- RoBERTa
- ALBERT

## Dataset

[Stanford Question Answering Dataset (SQuAD)](https://www.kaggle.com/datasets/stanfordu/stanford-question-answering-dataset)

The notebook uses SQuAD v1.1, which contains passages, questions, and their corresponding answers.

## Project Workflow

1. Download and explore the SQuAD dataset.
2. Load a sample of question-answering examples.
3. Load pretrained Transformer models and their tokenizers.
4. Generate answers using Hugging Face Question Answering pipelines.
5. Evaluate predictions using Exact Match (EM) and F1 Score.
6. Compare model performance.

## Model Evaluation

The notebook compares the models using a sample of 30 question-answering examples.

| Model | Exact Match | F1 Score |
|---|---:|---:|
| DistilBERT | 90.00% | 92.67% |
| BERT | 86.67% | 96.10% |
| RoBERTa | 93.33% | 97.43% |
| ALBERT | 76.67% | 79.33% |

RoBERTa achieved the highest Exact Match and F1 scores in this sample evaluation.

**Note:** These results are based on a small sample and should not be interpreted as a full benchmark of the models.

## Technologies

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Evaluate
- Hugging Face Datasets
- KaggleHub

## Notebook

The `notebook.ipynb` file contains the complete implementation, including dataset loading, sample predictions, model evaluation, and model comparison.
