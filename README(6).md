# Fa1eme_project2
PersianQuestionAnsweringProject

This project is a Persian Question Answering (QA) system designed to provide accurate answers to user queries.  
It utilizes the **PersianQA** dataset to evaluate different approaches and assess their accuracy, processing time, and generalization capabilities.  
The project aims to identify the most effective methods for Persian QA tasks and provides insights to support future work in Persian natural language processing.
## Features

- Provides accurate answers to Persian questions.  
- Compares different approaches to find the most effective solution.  
- Measures performance using **F1 score** and **Exact Match**.  
- Includes ready-to-use scripts for training, testing, and inference.  
## Installation

To run this project, you need Python 3.8+ and the following libraries:


```bash
pip install transformers datasets evaluate numpy
```
## Usage

After installing the required dependencies, simply run the main script to start the Persian Question Answering system. The script will handle training, evaluation, and computing performance metrics automatically.


```bash
python main.py
```
## Results

The models were evaluated on the PersianQA dataset.  
Results are reported separately for **All questions**, **Has Answer**, and **No Answer**.

| Model                        | All (F1 / EM) | Has Answer (F1 / EM) | No Answer (F1 / EM) |
|------------------------------|---------------|-----------------------|----------------------|
| BERT-base-fa-QA              | 85.36 / 70.53 | 82.54 / 61.32         | 91.90 / 91.90        |
| BERT-base-multilingual-cased | 67.01 / 51.08 | 65.01 / 42.24         | 71.68 / 71.68        |
| ALBERT-fa-base-v2            | 67.96 / 49.78 | 64.82 / 38.86         | 75.27 / 75.27        |
| XLM-RoBERTa-large-fa-QA      | 84.49 / 70.11 | 81.99 / 61.44         | 90.32 / 90.32        |
