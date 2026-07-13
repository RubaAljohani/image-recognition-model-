# Package Damage Inspection using Teachable Machine 

## Task Overview

This task is building a  simple model for package quality inspection on teachable machine google.  
The model classifies package images into two classes:

- **Damaged**
- **Intact**

The model was trained using **Google Teachable Machine** and exported in **Keras format**.  
A Python script was then used to load the trained model, accept an input image, and predict whether the package is damaged or intact to evaluate the model performance even further than teachable machine overview.


## Classes

The model was trained using two image classes:

| Class | Description |
|---|---|
| Damaged | Packages that appear crushed, torn, broken, or not in good condition |
| Intact | Packages that appear clean, complete, and in good condition |

## Dataset

The dataset was found on kaggle( url: https://www.kaggle.com/datasets/rahulm7323/damaged-and-intact-packages), it  contains images of damaged and intact packages.  
To avoide making the training process baised to one class, the dataset was divided into training and testing folders with balanced classes.

The edited dataset structure:

```text
dataset/
├── train/
│   ├── damaged/
│   └── intact/
│
└── test/
    ├── damaged/
    └── intact/
```
## Results

The model was evaluated on the test dataset. The final evaluation result was:

| Metric | Value |
|---|---:|
| Total Test Images | 116 |
| Correct Predictions | 100 |
| Wrong Predictions | 16 |
| Accuracy | 86.21% |

### Output Screenshots

![Evaluation Output 1](Screenshot%202026-07-13%20180837.png)

![Evaluation Output 2](Screenshot%202026-07-13%20183308.png)
