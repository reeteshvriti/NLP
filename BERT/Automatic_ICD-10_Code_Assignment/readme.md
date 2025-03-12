Problem Statement: Automatic ICD-10 Code Assignment Using ClinicalBERT
Background:
The International Classification of Diseases, 10th Revision (ICD-10) is widely used in healthcare for documenting diagnoses and procedures. Assigning ICD-10 codes manually is a time-consuming, error-prone, and labor-intensive task for medical coders and clinicians. Automating this process can enhance efficiency, reduce coding errors, and improve patient record management.

Problem Description:
Given a patient’s discharge summary or clinical notes, the task is to develop an AI-based system that automatically predicts the most relevant ICD-10 codes. This is a multi-label classification problem where a single document can correspond to multiple ICD-10 codes.

Challenges:
High Dimensionality: ICD-10 consists of thousands of unique codes.
Multi-label Nature: A single clinical document can be associated with multiple labels.
Data Imbalance: Some ICD codes are very frequent, while others are rare.
Clinical Language Complexity: Clinical notes contain abbreviations, domain-specific terminology, and unstructured text.

Proposed Solution:
This project aims to fine-tune ClinicalBERT, a domain-specific transformer model pre-trained on medical text, to automatically predict ICD-10 codes from discharge summaries. The model will be trained using a supervised learning approach, leveraging multi-label classification techniques such as sigmoid activation and binary cross-entropy loss.

Expected Outcomes:
A trained ClinicalBERT model capable of predicting ICD-10 codes with high accuracy.
Performance evaluation using Precision@k, Recall@k, and F1-score.
A user-friendly interface (API/Web App) for healthcare professionals to input clinical text and receive automated ICD-10 code predictions.
