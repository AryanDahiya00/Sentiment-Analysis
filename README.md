# Emotion Classification Project Report

## Project Overview
Deep learning project for classifying emotions in text using BERT-based sequence classification.

## Data Preprocessing
- **Dataset**: Smile Annotations CSV
- **Preprocessing Steps**:
  - Removed entries with multiple emotions or 'nocode'
  - Created label dictionary mapping emotions to numeric values
  - Stratified train-test split (85% train, 15% validation)

## Model Architecture
- **Model**: BERT for Sequence Classification
- **Pretrained Model**: bert-base-uncased
- **Configuration**:
  - Number of labels: Based on unique emotion categories
  - Max sequence length: 256 tokens

## Training Parameters
- **Optimizer**: AdamW
- **Learning Rate**: 5e-5
- **Batch Size**: 32
- **Epochs**: 10
- **Device**: CUDA (GPU) if available

## Performance Metrics
- **Evaluation Method**: 
  - F1 Score (weighted)
  - Per-class accuracy
- **Key Metrics**: 
  - Tracked training and validation loss
  - Calculated F1 score for each epoch

## Key Libraries
- PyTorch
- Transformers (Hugging Face)
- Pandas
- Scikit-learn

## Challenges Addressed
- Class imbalance
- Emotion classification complexity
- Handling variable-length text inputs

## Conclusion
Successfully implemented a BERT-based model for multi-class emotion classification with nuanced performance tracking.
