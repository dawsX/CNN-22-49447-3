# CNN-Based Handwritten Digit Classification

**CSC 4254 — Computer Vision & Pattern Recognition**  
**Student ID:** 22-49447-3

A custom two-block convolutional neural network trained to recognize ten handwritten digit classes using the public optical handwritten digits dataset bundled with scikit-learn. The Jupyter notebook includes executed training output and evaluation figures.

## Files
- `CNN_22-49447-3.ipynb` — fully executed assignment notebook with code, outputs, and figures
- `CNN_22-49447-3_weights.pth` — trained CNN parameters
- `training_curves.png` — training and validation loss/accuracy
- `confusion_matrix.png` — test-set confusion matrix
- `sample_predictions.png` — example held-out predictions
- `classification_report.txt` — per-class metrics
- `results.json` — evaluation metrics
- `requirements.txt` — dependencies

## Reproduce
Install the packages in `requirements.txt`, then open `CNN_22-49447-3.ipynb` in Jupyter Notebook or [Google Colab](https://colab.research.google.com/) and run cells sequentially. No Kaggle API key or external files are required.

## Dataset
[scikit-learn: Optical Recognition of Handwritten Digits](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html), 1,797 grayscale 8×8 images in 10 classes. A stratified 70/15/15 split is used for training/validation/testing. Images are normalized and resized to 32×32.

## Results
- Test accuracy: **97.41%** (measured during notebook execution)
- Training and validation curves and detailed metrics are saved above.

## GitHub submission
Create a public repository under your own GitHub account and upload these files. Submit the resulting **real repository URL** and the executed `.ipynb` through the instructor's submission form. A repository cannot be created by merely placing a GitHub URL in the notebook.
