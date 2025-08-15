# 🏃 Human Activity Recognition from Multi-Sensor Data

This project implements a machine learning pipeline to classify human activities using wearable sensor data. It includes data preprocessing, feature extraction, model training, evaluation, and visualization of results. Sensor data comes from accelerometers, gyroscopes, magnetometers, and pressure sensors collected from multiple users.

---

## 📁 Directory Structure
```
Sensor_Data_Classification/
├── Colab Notebooks/
│ ├── Sensor Data Analysis.ipynb     # Exploratory data analysis, preprocessing, and visualization
│ └── Sensor Data Classifier.ipynb   # Model training, evaluation, and results visualization
├── DataSet/                         # Sensor CSV files and processed feature datasets
│ ├── User13/ ... User27/            # Raw sensor CSVs per user
│ ├── W100_O25_Features.csv
│ ├── W200_O25_Features.csv
│ ├── ...                            # Other WXXX feature files
│ ├── feature_file.csv               # Combined or processed feature dataset
│ ├── full_dataset.csv               # Full merged dataset for modeling
│ └── data_collection.csv            # Metadata used during preprocessing
└── README.md
```
---

## 🧩 Setup Instructions

1. **Clone the repository**  

```bash
git clone https://github.com/yourusername/Sensor_Data_Classification.git
cd Sensor_Data_Classification
```

2. **Load the dataset**

- Ensure the `DataSet/` folder contains all user subfolders, feature files, and CSVs.  
- The notebooks automatically load all CSVs and feature datasets using relative paths.

3. **Run exploratory data analysis and preprocessing**

- Open `Colab Notebooks/Sensor Data Classifier.ipynb`  
- Clean, filter, normalize, and extract features from raw sensor data.  
- Use `data_collection.csv` for preprocessing metadata and mappings.

4. **Train and evaluate models**

- Open `Colab Notebooks/Sensor Data Analysis.ipynb`  
- Train classification models (e.g., Logistic Regression, Random Forest, SVM).  
- Evaluate using accuracy, F1-score, and confusion matrices.  
- Results and visualizations are displayed **within the notebook**.

5. **Visualize results**

- Confusion matrices, decision boundaries, and evaluation metrics are shown inline in the notebooks.

---

## 📌 Notes

- The pipeline is modular; preprocessing, feature extraction, and model training can be rerun independently.  
- Supports multiple users and multiple sensor types.  
- Dataset includes both raw CSVs (`User13-User27`) and aggregated feature files (`W100`, `feature_file.csv`, `full_dataset.csv`).  
- Designed for easy extension to additional users or new sensors.
