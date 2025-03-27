# KNN Direct Marketing Campaigns Analysis

## Overview
This project applies the K-Nearest Neighbors (KNN) algorithm to analyze a direct marketing campaign dataset. The goal is to predict whether a client will subscribe to a term deposit based on various features.

## Dataset
- **File:** `bank_marketing.csv`
- **Format:** CSV with `;` as the delimiter
- **Target Variable:** `y` (whether the client subscribed to a term deposit)
- **Features:** Various attributes related to customer demographics, previous campaign interactions, and socioeconomic factors.

## Steps in Analysis

### 1. Importing Libraries and Loading Dataset
- Load necessary Python libraries (e.g., Pandas, NumPy, Matplotlib, Scikit-learn, Seaborn).
- Read the dataset and inspect its structure using `.head()` and `.tail()`.

### 2. Data Preprocessing
- Convert categorical features to numerical using **Label Encoding**.
- Standardize numerical features using **StandardScaler**.

### 3. Splitting Data
- Define features (`X`) and target variable (`y`).
- Split the dataset into **training (80%)** and **testing (20%)** subsets.

### 4. Finding Optimal K for KNN
- Perform **5-fold cross-validation** to determine the best value of `K`.
- Plot error rate vs. K and accuracy vs. K to visualize the best choice.
- Select the optimal `K` based on **minimum error rate**.

### 5. Training and Testing the KNN Model
- Train the **final KNN model** using the optimal `K`.
- Make predictions on the test set.
- Evaluate the model using **accuracy, classification report, and confusion matrix**.

### 6. Results and Insights
- Display feature importance based on correlation with the target variable.
- Visualize results using **heatmaps, bar charts, and performance plots**.

## Requirements
- Python 3.x
- Libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
  ```

## Usage
1. Run the script in a Python environment:
   ```bash
   python knn_marketing_analysis.py
   ```
2. The script will output evaluation metrics, visualizations, and feature analysis.

## Output
- **Optimal K value** for KNN model
- **Accuracy, classification report, and confusion matrix**
- **Visual plots** for model performance analysis
- **Feature correlation insights**
- <img width="472" alt="Screenshot 2025-03-27 154018" src="https://github.com/user-attachments/assets/2488ed6c-4ede-46d7-8472-bb96e0513d08" />
- <img width="470" alt="Screenshot 2025-03-27 154037" src="https://github.com/user-attachments/assets/03ee7de2-fd08-43ba-a149-dc55f4b305bb" />
- <img width="473" alt="Screenshot 2025-03-27 154113" src="https://github.com/user-attachments/assets/7520e5f4-389e-4f45-bae4-a68189895736" />
- <img width="444" alt="Screenshot 2025-03-27 154130" src="https://github.com/user-attachments/assets/0eca2b38-0fc9-486f-bc00-f34399b1612d" />
- <img width="471" alt="Screenshot 2025-03-27 154201" src="https://github.com/user-attachments/assets/f09c80ba-156d-45f1-9be7-574a06e7060c" />

## Author
Developed by Jeremy Martinez-Quinones.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

