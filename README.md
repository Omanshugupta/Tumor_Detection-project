# Tumor Detection Project

## Objective
The goal of this project is to classify tumors as **malignant (M)** or **benign (B)** using a dataset of tumor characteristics. This is achieved through data preprocessing, exploratory data analysis (EDA), and applying a **Random Forest Classifier** machine learning model.

## Dataset
**Filename:** `Tumor_Detection.csv`  

### Features
The dataset includes 30 numeric features derived from digitized images of a breast mass (e.g., radius, texture, perimeter, area, smoothness, etc.).

### Target
- `diagnosis`:
  - `M` = Malignant
  - `B` = Benign

## Steps Performed

### 1. **Data Loading & Cleaning**
- Loaded the CSV file into a pandas DataFrame
- Dropped irrelevant columns: `id`, `Unnamed: 32`
- Handled missing values

### 2. **Exploratory Data Analysis (EDA)**
- Visualized distribution of diagnosis labels
- Plotted a correlation heatmap to observe feature relationships
- Identified highly correlated features

### 3. **Preprocessing**
- Converted categorical target labels to binary (M → 1, B → 0)
- Applied `StandardScaler` to normalize the data
- Split the dataset into training and test sets (80-20 split)

### 4. **Modeling**
- Used a `RandomForestClassifier` from scikit-learn
- Trained the model on the training data
- Evaluated using accuracy, confusion matrix, and classification report

### 5. **Results**
- Achieved high accuracy on the test set (typically > 95%)
- Confusion matrix showed minimal false positives/negatives


##  Results Summary

- **Model Used:** Random Forest Classifier
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score
- **Visualizations:** Count plot, Correlation heatmap, Confusion matrix


## File Structure
Tumor_Detection-project/
│
├── Tumor_Detection.ipynb # Jupyter Notebook with full analysis
├── Tumor_Detection.csv # Dataset file
└── README.md # Project documentation

## How to Run

1. Clone the repo or download the `.zip` file.
2. Open `Tumor_Detection.ipynb` in Jupyter Notebook.
3. Run all cells in order for full execution.
4. Ensure required Python libraries are installed: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.

## Conclusion

- The model effectively classifies tumors with high accuracy.
- EDA helped understand the feature relationships and importance.
- This workflow demonstrates a real-world medical ML pipeline from raw data to prediction.


