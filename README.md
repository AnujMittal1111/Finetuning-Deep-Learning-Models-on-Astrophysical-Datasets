# Finetuning Deep Learning Models on Astrophysical Datasets

This project focuses on finetuning deep learning models on large-scale astrophysical image datasets to classify galaxy morphologies.  
The work involves transfer learning, lightweight finetuning techniques, and decision threshold optimization to improve model accuracy and stability.

This project was carried out under the Physics and Astronomy Club, IIT Roorkee.

## Project Summary

- Trained and finetuned MobileNetV1 on more than 70,000 galaxy image samples.
- Applied transfer learning and lightweight finetuning to reduce overfitting and improve generalization.
- Introduced threshold tuning to improve decision boundaries.
- Achieved an accuracy improvement from 78 percent to 89 percent after initial finetuning.
- Further optimized the model to reach 92 percent accuracy with stable inference and lower variance.

## Repository Structure

finetune_mobilenet.py                 : Script for finetuning MobileNetV1  
galaxy_classification.ipynb           : Complete training and evaluation notebook  
models/                                : Saved model checkpoints  
data/                                  : Dataset directory (not included due to size)  
README.md                              : Project documentation  

## Tech Stack Used

### Languages and Tools
- Python  
- Jupyter Notebook  

### Libraries
- PyTorch  
- torchvision  
- timm  
- NumPy  
- Matplotlib  

### Techniques
- Transfer Learning  
- Lightweight Finetuning  
- Low-rank adaptation (LoRA-inspired)  
- Decision Threshold Optimization  
- Early Stopping  
- Learning Rate Scheduling  

## Model Performance

- Initial transfer learning accuracy: 78 percent  
- After classifier-level finetuning: 89 percent  
- After threshold optimization: 92 percent  
- Improved stability across validation folds and reduced overfitting  

## Key Insights

- Pretrained backbones deliver strong results even with limited astrophysical data.
- Threshold tuning significantly enhances class separation in noisy datasets.
- Lightweight finetuning allows effective training with reduced computational cost.

## How to Run

1. Install required libraries:

   pip install torch torchvision timm numpy matplotlib

2. Place the dataset in the following format:

   data/  
       train/  
           class1/  
           class2/  
       val/  
           class1/  
           class2/  

3. Run the finetuning script:

   python finetune_mobilenet.py

4. The best model checkpoint will be saved in the models/ directory.

## Documentation

This project demonstrates how transfer learning and lightweight finetuning can be effectively applied to noisy astrophysical datasets to achieve high accuracy and stable inference.

## Author

Anuj Mittal  
IIT Roorkee  
