
# CNN_XAI_Bankruptcy

This study employs the Explainable Artificial Intelligence (XAI) approach, utilizing a Convolutional Neural Network model (CNN) to forecast company financial conditions based on their financial ratios. By transforming financial data into images, we introduce a Bankruptcy Prediction Model (BPM) that enhances interpretability through techniques like Shapley Additive exPlanations (SHAP) and Local Interpretable Model-Agnostic Explanations (LIME). These XAI methods aim to clarify AI decisions in the BPM, addressing the ongoing debate within the financial research community regarding the most informative ratios for bankruptcy prediction. This research marks a significant advancement in financial accounting by merging the transparency of XAI with effective bankruptcy prediction, offering a more comprehensive understanding of financial ratio analysis.

The models included in this project are:
- Convolutional Neural Network (CNN)
- Additionally, SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations) analysis is conducted to interpret the CNN model.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:
1. **Python Environment**: Make sure you have Python installed. You can download it from [python.org](https://www.python.org/).
2. **Dependencies**: Use the `requirements.txt` file to install all necessary packages.

   ```bash
   pip install -r requirements.txt
   ```

## Getting the Data

The example dataset used for this project can be downloaded from the following Google Drive link (10% of the original dataset). We have renamed the original names of our features to X1, X2, X3, etc.:

- [Download Dataset](https://drive.google.com/file/d/1CYNhKvNkQYZ55GPYuLZ4y_lLxTNafi3s/view?usp=sharing)

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ronip92/CNN_XAI_Bankruptcy.git
   cd CNN_XAI_Bankruptcy
   ```

2. **Run Jupyter Notebooks**:
   Open the Jupyter notebooks in the `notebooks/` directory to explore the data processing, model training, and explainability analysis.

   ```bash
   jupyter notebook
   ```

### Results

Detailed results and analysis can be found in the notebook. Key findings include:

1. **Feature Selection**:
   - **Notebook**: `Feature Selection Rank - 36month.ipynb`
   - **Description**: Identification of the most important financial ratios that contribute significantly to bankruptcy prediction, using feature selection techniques.

2. **Image Generation**:
   - **Notebooks**:
     - `Images Generating Bankrupt - Lasso.ipynb`
     - `Images Generating NonBankrupt - Lasso.ipynb`
   - **Description**: Conversion of financial data into greyscale pixel images representing financial ratios, providing a novel approach to visualizing and analyzing financial data.

3. **CNN Model Training and Evaluation**:
   - **Notebooks**:
     - `CNN Model.ipynb` - Original Dataset FS0 (2,180:11,972)
     - `CNNFS_balanced_1_1.ipynb` - Original Dataset FS1 (2,180:2,180)
     - `CNNFS_balanced_1_2.ipynb` - Original Dataset FS2 (2,180:4,360)
     - `CNNFS_balanced_2_all_nonbankrupt.ipynb` - Original Dataset FS3 (4,360:11,972)
     - `CNNFS_balanced_equal_a half.ipynb` - Original Dataset FS4 (5,986:5,986)

4. **Trained Models**:
   - **Files**:
     - `CNNFS.h5` - Original Dataset FS0 (2,180:11,972)
     - `CNNFS_balanced_1_1.h5` - Original Dataset FS1 (2,180:2,180)
     - `CNNFS_balanced_1_2.h5` - Original Dataset FS2 (2,180:4,360)
     - `CNNFS_balanced_2_all_nonbankrupt.h5` - Original Dataset FS3 (4,360:11,972)
     - `CNNFS_balanced_equal_a half.h5` - Original Dataset FS4 (5,986:5,986)
   - [Download Trained Models](https://drive.google.com/drive/folders/1dKGtxIEYNX1uOJ6WF1dxMSJnGrGc8Irg?usp=sharing)
   - **Description**: The outcomes of the classification algorithm are detailed across five different datasets, designated FS0 through FS4, tailored to explore the effects of class imbalance on model performance. Performance metrics of the Convolutional Neural Network, including accuracy, precision, recall, and F1-score, demonstrate the model's effectiveness in predicting bankruptcy.

5. **Model Interpretability**:
   - **Notebooks**:
     - `CNN SHAP-FS0.ipynb`
     - `CNN LIME-Class.ipynb`
   - **Description**: Explanation of the CNN model's predictions through SHAP and LIME, offering a transparent understanding of the decision-making process and highlighting the contribution of each feature to the final prediction.

## Repository Structure

- `notebooks/`: Contains the Jupyter notebooks for data preparation, model building, and explainability analysis.
- `models/`: Contains the saved models.
- `docs/`: Contains documentation files and images.
- `README.md`: Overview of the project.
- `requirements.txt`: List of dependencies required to run the notebook.
