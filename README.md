# Natural Images — Custom CNN Classification

**Course:** Computer Vision & Pattern Recognition (CSC 4254)  
**Student ID:** 22-49447-3  
**Notebook:** `CNN_22-49447-3.ipynb`

## Project

A custom PyTorch CNN classifies photos from the publicly available [Natural Images dataset](https://www.kaggle.com/datasets/prasunroy/natural-images), in eight classes: airplane, car, cat, dog, flower, fruit, motorbike and person (6,899 images).

The notebook uses a 70% / 15% / 15% stratified training / validation / test split, resized 96×96 RGB images, training augmentation, three convolution blocks, batch normalization, ReLU, max pooling, dropout, and a final eight-class classifier. Training uses Adam, cross-entropy loss, and 15 epochs.

## Saved notebook results

The uploaded notebook has recorded outputs from an earlier execution, including **94.30% test accuracy** and **0.1571 test loss**. These are the notebook's saved output values, not a new execution performed while packaging it.

| File | Purpose |
| --- | --- |
| `CNN_22-49447-3.ipynb` | Original executable notebook with saved outputs |
| `CNN_22-49447-3.pth` | Saved trained PyTorch model checkpoint (8 Natural Images classes) |
| `class_distribution.png` | Number of images per class |
| `sample_dataset_images.png` | Sample images from the dataset |
| `training_curves.png` | Training and validation loss / accuracy |
| `confusion_matrix.png` | Eight-class test confusion matrix |
| `sample_predictions.png` | Test-image predictions |
| `classification_report.txt` | Saved per-class precision, recall and F1 scores |
| `training_log.txt` | Recorded epoch-by-epoch training output |
| `requirements.txt` | Python dependencies |

## Run / reproduce

1. Open the notebook in Google Colab or another Python environment with PyTorch installed.
2. Run all cells in order. The notebook downloads the Natural Images dataset using `kagglehub`, so internet access is needed.
3. Re-running training can produce different metrics depending on device, library versions and nondeterminism.
4. The included `CNN_22-49447-3.pth` checkpoint can be loaded directly using the notebook’s model-loading section. Re-running and saving will overwrite it.

## Trained model checkpoint

The accompanying `.pth` checkpoint was supplied separately and checked with PyTorch (`weights_only=True`). It contains the eight Natural Images class names, 96-pixel image size, 15 epochs, model-state tensors consistent with the notebook’s `NaturalImageCNN` architecture, and a recorded test accuracy of approximately **94.30%**. This confirms file-format and architecture consistency; it is not an independent re-evaluation against the dataset.

## Assignment submission

Publish the files in a public GitHub repository, then submit the repository URL and the `.ipynb` notebook via the instructor's submission form. The repository URL is created by GitHub once published; no real URL is embedded here.
