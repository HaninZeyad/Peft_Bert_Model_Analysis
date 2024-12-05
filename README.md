## Intent Classification: Efficiency vs Quality
This project explores the tradeoff between model efficiency and quality for intent classification using the English portion of the Massive dataset. We experiment with different BERT-like models and training approaches to uncover insights into the relationship between these factors.

Task Overview
We treat intent classification as a text classification task, focusing on the ('utt', 'intent') columns. Model efficiency is evaluated in terms of:

### Training time: Time to train the model.
### Model size: Number of parameters.
### Inference time: Time to generate predictions for new inputs.
Model quality is measured by:

### F1-score: To handle the imbalanced dataset.
### Classification accuracy: Overall prediction correctness.
Training Approaches
Fine-tuning pretrained BERT.
Training BERT-like model from scratch.
Soft-label distillation: Distilling a fine-tuned BERT model to a smaller model.
LoRa (Low-Rank Adaptation): Efficient fine-tuning with fewer parameters.
Objective
We aim to understand how different model sizes and training methods affect both performance (F1-score, accuracy) and efficiency (training time, inference time).

Dataset
The Massive dataset consists of user utterances and their corresponding intents, used for training and evaluating the models.# Peft_Bert_Model_Analysis
