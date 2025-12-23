# Task [X]: [Task Name]

*Student:* Aydın Məmmədli 
*ID:* S215  
*Seed:* 20240215

## Presentation
[View Presentation Slides](https://docs.google.com/presentation/d/1hOPQWgntzJMGkEM7OZ3foGuKy3kFIjhX/edit?usp=drive_link&ouid=103726477962169156363&rtpof=true&sd=true)

## Dataset
- *Name:* Rock Paper Scissors (Kaggle)
- *Classes:* 3 (Rock, Paper, Scissors)
- *Training samples:* 1750
- *Test samples:* 438

## Model Architecture
- *Type:CNN (RPSModel)
- *Convolutional layers:* 3 (Each followed by ReLU and MaxPool)
- *Fully connected layers:* 2 (One hidden layer with 128 units and one output layer with 3 units)
- *Total parameters:Calculated based on the "RPSModel" structure with 128 * 16 * 16 input to the first linear layer.

## Training Comparison

### Version 1
- *Learning rate:* 0.001
- *Batch size:* 32
- *Optimizer:* Adam
- *Test accuracy:* 97.72% (Result after 10 epochs)

### Version 2
- *Learning rate:* 0.0001
- *Batch size:* 32
- *Optimizer:* Adam
- *Test accuracy:* 96.12% (Result after 10 epochs)

### Best Result
- *Best version:* Version 1
- *Final test accuracy:* 98.40% (Peak accuracy reached during epochs 6 and 7)
- *Target accuracy:* 88.0%
- *Status:* ✓ Achieved 

## Analysis
- *Best performing class:* scissors
- *Worst performing class:* rock
- *Key observations:* A higher learning rate (0.001) resulted in faster convergence and higher test accuracy for this specific model and dataset. The model is capable of reaching a high success rate of 98% in a short period of 10 epochs.

## Files
- notebook.ipynb: Complete implementation with both training runs
- results/training_comparison.png: Comparison of Version 1 vs Version 2
- results/confusion_matrix.png: Confusion matrix from best model
- results/predictions.png: Sample predictions
