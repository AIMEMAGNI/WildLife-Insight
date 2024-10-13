# WildLife Insight

## Overview

WildLife Insight is a machine learning project aimed at predicting the conservation status of species based on specific input features. By utilizing neural networks, the project implements two models: a simple baseline model and an advanced model incorporating multiple optimization techniques. This assignment demonstrates the process of building and refining machine learning models for classification tasks.

## Dataset

The dataset used in this project is sourced from the **IUCN Red List** of Threatened Species. It contains information on various species, including attributes such as:
- `speciesName`: The name of the species.
- `systems`: Habitat or system associated with the species.
- `scopes`: Specific geographical or ecological scope related to the species.
- `Category`: The target variable indicating the conservation status of the species.

The dataset contains 69,253 species, providing a rich variety of information for classification tasks.

**Data Source**: [IUCN Red List](https://www.iucnredlist.org/)

### Attribution

The dataset and species information used in this project are sourced from the **IUCN Red List of Threatened Species**, an important resource for biodiversity conservation. Please ensure proper acknowledgment when utilizing or referencing this dataset. For more information, visit [IUCN Red List](https://www.iucnredlist.org/).

## Objective

The primary objective of this project is to demonstrate the application of neural networks to predict species' conservation categories. Specifically:
1. Build a simple neural network without optimizations to serve as a baseline.
2. Develop an optimized neural network using regularization, early stopping, and learning rate adjustments.
3. Compare and analyze the performance of both models.

## Project Structure

```
WildLife_Insight/
├── Aime_Magnifique_NDAYISHIMIYE_Model_Training_and_Evaluation.ipynb       # The main project notebook containing code and analysis
├── species_data.csv      # The Dataset
├── saved_models/
│   ├── model1_simple.h5   # The simple/Vanilla model
│   ├── model2_optimized.h5  # The advanced, optimized model
│   └── ...
└── README.md            # Project overview, objectives, and findings
```

## Implementation

The project follows these key steps:
1. **Data Preparation**: Preprocess the dataset, including encoding categorical features and scaling the data.
2. **Model 1: Baseline Neural Network**:
   - Implemented without optimizations.
   - Simple architecture with basic layers.
   - Used for comparative analysis.
3. **Model 2: Optimized Neural Network**:
   - Includes regularization, learning rate scheduling, and early stopping.
   - Adjusted hyperparameters to improve convergence and performance.
4. **Evaluation**:
   - Compared both models using metrics like Accuracy, F1 Score, and Confusion Matrix.
   - Analyzed the results to understand the impact of the optimizations.

## Key Findings

- **Baseline Model**: Achieved a certain level of accuracy, performing relatively well on the dataset.
- **Optimized Model**: Applied advanced techniques like regularization, early stopping, and learning rate adjustments. However, the overall improvement in accuracy was minimal, with both models yielding similar results. This indicates that the baseline architecture might already have been sufficiently robust for this specific dataset, or the optimizations did not address the key challenges.

## Usage Instructions

1. Clone the repository:
    ```
    git clone https://github.com/yourusername/WildLife_Insight.git
    ```
2. Navigate to the project directory:
    ```
    cd WildLife_Insight
    ```
3. Install required dependencies:
    ```
    pip install -r requirements.txt
    ```
4. Open the notebook:
    ```
    jupyter notebook notebook.ipynb
    ```
5. Run the cells sequentially to reproduce the results.

## Libraries Used

- **Pandas**: For data manipulation and preprocessing.
- **NumPy**: For numerical operations.
- **Scikit-learn**: For encoding, scaling, and model evaluation.
- **TensorFlow / Keras**: For building and training neural networks.
- **Matplotlib & Seaborn**: For visualizing data and results.

## Results & Analysis

Both models were evaluated on a test set, and despite the use of optimization techniques in the second model, there was no significant improvement over the baseline. This outcome suggests that the dataset and task might not benefit much from the added complexity or that further adjustments to the architecture and hyperparameters are required to see a difference.

## Conclusion

This project demonstrates the process of building and experimenting with neural networks for classification. The similar performance of both the baseline and optimized models suggests that more sophisticated optimization techniques may not always yield improved results, especially when the baseline model is already well-tuned for the task. Future work could explore different model architectures, feature engineering, or alternative data sources to gain further insights.
