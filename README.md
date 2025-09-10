🤖 Task 5: Auto Tagging Support Tickets Using LLM
🎯 Objective

Automatically tag support tickets into relevant categories using a local Large Language Model (LLM) pipeline with prompt engineering, fine-tuning, and few-shot learning techniques.

📂 Dataset

A small synthetic support ticket dataset consisting of free-text issue descriptions labeled with one or more tags:

Example tags:

Billing

Sales

Technical Issue

Account Management

🔧 Steps Performed

Prompt Engineering (Zero-Shot Inference)

Used zero-shot-classification pipeline from Hugging Face to generate tag predictions without training.

Returned top 3 most probable tags for each ticket.

Fine-Tuning a Text Classifier

Vectorized the text using TF-IDF

Used LogisticRegression for multi-label classification

Trained on the ticket dataset and evaluated using classification metrics

Few-Shot Learning Simulation

Augmented training with a small number of labeled examples to improve performance

Added synthetic few-shot prompts to enhance context for the model

Performance Comparison

Compared predictions from:

Zero-shot classification

Fine-tuned classifier

Displayed true labels, predicted zero-shot tags, and fine-tuned top-3 tags for each test ticket

📈 Evaluation Metrics

Precision

Recall

F1-Score

Top-3 Accuracy

Comparison Table of Predictions

💡 Key Highlights
Feature	Implemented
Zero-shot classification	✅
Fine-tuning on labeled dataset	✅
Few-shot learning enhancement	✅
Multi-label output (Top-3 tags)	✅
Local model only (No API needed)	✅
🧪 Technologies Used

Python 3.x

Scikit-learn

Transformers (Hugging Face)

MultiLabelBinarizer

TF-IDF Vectorization

Pandas, Numpy

🚀 Skills Gained

Prompt engineering and LLM integration

Zero-shot vs fine-tuned model comparison

Few-shot learning for improved accuracy

Multi-label classification and ranking

Practical experience with NLP for support automation

Author : 
Muhammad Mustaqeem Javed
