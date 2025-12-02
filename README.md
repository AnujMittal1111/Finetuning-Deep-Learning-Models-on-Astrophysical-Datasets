# Finetuning Deep Learning Models on Astrophysical Datasets

This project focuses on finetuning deep learning models on large-scale astrophysical image datasets to classify galaxy morphologies.  
The work involves transfer learning, lightweight finetuning techniques, and decision threshold optimization to improve model accuracy and stability.

This project was conducted under the Physics and Astronomy Club, IIT Roorkee.

## Project Summary

- Trained and finetuned MobileNetV1 on more than 70,000 galaxy image samples.
- Applied transfer learning and lightweight finetuning to reduce overfitting.
- Introduced threshold tuning and model simplification to improve classification boundaries.
- Improved test accuracy from 78 percent to 89 percent through finetuning.
- Further optimized the model to reach 92 percent test accuracy with stable inference.

This repository includes the finetuning scripts and supporting files required to reproduce the results.

## Repository Structure

finetune_mobilenet.py                 : Script for finetuning MobileNetV1  
galaxy_classification.ipynb           : Notebook version (if included)  
models/                                : Saved model checkpoints  
data/                                  : Image dataset (train and validation folders, not included in this repo)  
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
- LoRA-inspired low-rank updates  
- Decision Threshold Optimization  
- Early Stopping  
- Learning Rate Scheduling  

## Model Performance

- Initial transfer learning accuracy: 78 percent  
- After finetuning with classifier layers: 89 percent  
- After threshold and boundary optimization: 92 percent  
- Improved inference stability and reduced overfitting across validation sets  

## Key Insights

- Finetuning pretrained backbones works well for limited astrophysical data.
- Threshold optimization significantly improves final predictions.
- Lightweight finetuning provides strong performance with lower computational cost.

## How to Run

1. Install required libraries:

   pip install torch torchvision timm numpy matplotlib

2. Prepare dataset in the following format:

   data/  
       train/  
           class1/  
           class2/  
       val/  
           class1/  
           class2/  

3. Run the finetuning script:

   python finetune_mobilenet.py

4. The best model checkpoint will be saved in the models/ folder.

## Documentation

This project demonstrates how transfer learning and lightweight finetuning can be applied to noisy astrophysical datasets to achieve high accuracy with stable inference.

## Author

Anuj Mittal  
IIT Roorkee  
