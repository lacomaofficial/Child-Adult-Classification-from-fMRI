# Age Classification on fMRI with Support Vector Machine

## Project Overview

This project aims to classify individuals as children or adults based on resting-state fMRI (functional Magnetic Resonance Imaging) signal patterns using a Support Vector Classifier (SVC). The dataset includes individuals across a wide age range, from children (ages 3-13) to young adults (ages 18-39).

## Project Structure

The project code is organized into several sections, each serving a specific purpose:

1. **Importing Necessary Libraries**: Importing the required Python libraries for data manipulation, visualization, and machine learning.

2. **Data Exploration**:
   - Loading and inspecting the dataset.
   - Checking for duplicate entries, data types, and missing values.
   - Exploring the target variable, which is whether an individual is a child or an adult.

3. **Feature Extraction with Nilearn Masker**:
   - Loading an atlas for defining regions of interest (ROIs).
   - Initializing a masker to extract features from fMRI data.
   - Calculating connectivity features using correlation measures for each subject.

4. **Data Preparation for Machine Learning**:
   - Mapping class labels (child/adult) to numerical labels (0/1).
   - Splitting the dataset into training and testing sets, ensuring class balance using SMOTE (Synthetic Minority Over-sampling Technique).

5. **Model Building and Evaluation**:
   - Building an SVC model with hyperparameter tuning using GridSearchCV.
   - Training the model on the resampled training data.
   - Making predictions on the test set.
   - Evaluating the model's performance using accuracy and generating a classification report.
   - Visualizing the confusion matrix.

6. **Interpreting Model Feature Importance**:
   - Extracting the coefficients (weights) of the linear SVM model.
   - Visualizing feature importances.
   - Plotting the connectome map to explore which regions contribute to classification.

![output](https://github.com/lacomaofficial/Child-Adult-Classification-from-fMRI/assets/132283879/2a0534eb-3025-4057-bec6-c72cd235d975)

