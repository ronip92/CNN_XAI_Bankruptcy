# CNN_XAI_Bankruptcy
This study employs the Explainable Artificial Intelligence (XAI) approach, utilizing a Convolutional Neural Network model (CNN) to forecast company financial conditions based on their financial ratios. By transforming financial data into images, we introduce a Bankruptcy Prediction Model (BPM) that enhances interpretability through techniques like Shapley Additive exPlanations (SHAP) and Local Interpretable Model-Agnostic Explanations (LIME). These XAI methods aim to clarify AI decisions in the BPM, addressing the ongoing debate within the financial research community regarding the most informative ratios for bankruptcy prediction. This research marks a significant advancement in financial accounting by merging the transparency of XAI with effective bankruptcy prediction, offering a more comprehensive understanding of financial ratio analysis.
The models included in this project are:

-  Convolutional Neural Network (CNN)
-  Additionally, SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations) analysis is conducted to interpret the CNN model.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

1. Python Environment: Make sure you have Python installed. You can download it from python.org.
2. Use the requirements.txt file to install all necessary packages.

## Getting the Data

The example dataset used for this project can be downloaded from the following Google Drive link (10% of original dataset) and we rename original name of our feature with X1, X2,X.....:

- [Download Dataset](https://drive.google.com/file/d/1CYNhKvNkQYZ55GPYuLZ4y_lLxTNafi3s/view?usp=sharing)

## Usage

### Results

Detailed results and analysis can be found in the notebook. Key findings include:

1. **Feature Selection Rank - 36month.ipynb**
   Feature selections:Identification of the most important financial ratios that contribute significantly to bankruptcy prediction, using feature selection techniques.

2. **Images Generating Bankrupt - Lasso.ipynb**
   **Images Generating NonBankrupt - Lasso.ipynb**
   
   **Image Generation:** Conversion of financial data into greyscale pixel images representing financial ratios, providing a novel approach to visualizing and analyzing financial data.
   
4. **CNN Model.ipynb** - Original Dataset FS0 (2,180:11,972)
   **CNNFS_balanced_1_1.ipynb** - Original Dataset FS1 (2,180:2,180)
   **CNNFS_balanced_1_2.ipynb** - Original Dataset FS2 (2,180:4,360)
   **CNNFS_balanced_2_all_nonbankrupt.ipynb** - Original Dataset FS3 (4,360:11,972)
   **CNNFS_balanced_equal_a half.ipynb** - Original Dataset FS4 (5,986:5,986)

#### Trained model
   
   **CNNFS.h5** - Original Dataset FS0 (2,180:11,972)
   **CNNFS_balanced_1_1.h5** - Original Dataset FS1 (2,180:2,180)
   **CNNFS_balanced_1_2.h5** - Original Dataset FS2 (2,180:4,360)
   **CNNFS_balanced_2_all_nonbankrupt.h5** - Original Dataset FS3 (4,360:11,972)
   **CNNFS_balanced_equal_a half.h5** - Original Dataset FS4 (5,986:5,986)
   
   **Prediction Accuracy of the CNN Model:** The outcomes of the classification algorithm are detailed across five different datasets, designated FS0 through FS4, tailored to explore the effects of class       
     imbalance on model performance. . Performance metrics of the Convolutional Neural Network, including accuracy, precision, recall, and F1-score, demonstrating the model's effectiveness in predicting 
     bankruptcy.

#### Interpretability insights using SHAP and LIME.

- **CNN SHAP-FS0.ipynb**
- **CNN LIME-Class.ipynb**
