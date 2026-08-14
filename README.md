# Pandas Data Analysis Project

A comprehensive learning and analysis project exploring pandas data manipulation, exploratory data analysis (EDA), and data visualization using Python.

---

## 📁 Project Structure

```
02_pandas/
├── README.md                  # This file
├── pandas_basics.ipynb       # Introductory pandas concepts
├── titanic_analysis.ipynb    # Real-world analysis of Titanic dataset
└── train.csv                 # Titanic dataset (~890 passengers)
```

---

## 🎯 Project Overview

This project is divided into two main components:

### 1. **Pandas Basics** (`pandas_basics.ipynb`)
An introductory notebook covering fundamental pandas operations:

- **Series**: Working with 1D labeled arrays
  - Creating Series from lists
  - Basic operations on Series data

- **DataFrames**: Working with 2D tabular data
  - Creating DataFrames from dictionaries
  - Selecting columns (single and multiple)
  - Selecting rows using `.iloc[]`
  - Inspecting data structure and properties
  - Getting data types and statistical summaries

**Key Topics Covered:**
- DataFrame creation and structure
- Column and row selection
- Data exploration (shape, columns, dtypes)
- Statistical summaries using `.describe()`

---

### 2. **Titanic Dataset Analysis** (`titanic_analysis.ipynb`)
A comprehensive real-world analysis of the Titanic passenger dataset:

#### **Data Loading & Exploration**
- Loading data from CSV
- Viewing dataset structure (head, tail, shape)
- Examining columns and data types
- Statistical summaries

#### **Data Analysis**
- **Passenger Statistics:**
  - Total number of passengers
  - Passenger class distribution
  - Gender distribution
  - Age statistics (mean, median)
  - Fare statistics (min, max, mean)

- **Survival Analysis:**
  - Overall survival counts and percentages
  - Survival rate by passenger class
  - Survival rate by gender
  - Survival rate by age groups

#### **Data Cleaning**
- Identifying missing values
  - Percentage of missing data per column
  - Handling missing Age values using median imputation
  - Validation of cleaning process

#### **Data Visualization**
- **Bar Charts:** Passenger survival, class distribution, gender distribution
- **Histograms:** Age distribution with various bin configurations
- **Scatter Plots:** Relationship between Age and Fare
- **Grouped Analysis:** Survival rates by class, gender, and age groups

#### **Feature Engineering**
- Creating age groups using `.pd.cut()` for stratified analysis
- Grouping and aggregation using `.groupby()`

---

## 📊 Dataset Overview

**Titanic Dataset (`train.csv`)**

The Titanic dataset contains information about passengers aboard the RMS Titanic:

**Key Columns:**
| Column | Description | Data Type |
|--------|-------------|-----------|
| PassengerId | Unique identifier | Integer |
| Survived | Survival status (0=No, 1=Yes) | Integer |
| Pclass | Passenger class (1=First, 2=Second, 3=Third) | Integer |
| Name | Passenger name | String |
| Sex | Gender (male/female) | String |
| Age | Age in years | Float |
| SibSp | Number of siblings/spouses aboard | Integer |
| Parch | Number of parents/children aboard | Integer |
| Ticket | Ticket number | String |
| Fare | Ticket fare | Float |
| Cabin | Cabin number | String |
| Embarked | Port of embarkation | String |

**Dataset Insights:**
- ~890 passengers in the dataset
- Missing values in Age, Cabin, and Embarked columns
- 38% survival rate overall
- Significant variation in survival by passenger class and gender

---

## 🔧 Technologies & Libraries

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **matplotlib**: Data visualization
- **Jupyter Notebook**: Interactive computing environment

---

## 📖 How to Use This Project

### Prerequisites
```bash
pip install pandas matplotlib jupyter
```

### Running the Notebooks

1. **Navigate to the project directory:**
   ```bash
   cd "D:\DATA SCENCE\02_pandas"
   ```

2. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

3. **Open and run notebooks in order:**
   - Start with `pandas_basics.ipynb` to understand fundamental concepts
   - Then explore `titanic_analysis.ipynb` for advanced analysis

### Executing Cells
- Click on a cell and press `Shift + Enter` to execute
- Or use the Run button in the toolbar
- Run cells sequentially from top to bottom

---

## 🔍 Key Learnings

### Pandas Operations Demonstrated

1. **Data Loading**
   - Reading CSV files with `pd.read_csv()`

2. **Data Exploration**
   - `.head()`, `.tail()` - View first/last rows
   - `.shape` - Dimensions
   - `.columns` - Column names
   - `.info()` - Data types and non-null counts
   - `.describe()` - Statistical summary

3. **Data Selection & Manipulation**
   - Column selection: `df["column"]` or `df[["col1", "col2"]]`
   - Row selection: `df.iloc[index]`
   - `.unique()` - Unique values
   - `.value_counts()` - Frequency counts

4. **Data Cleaning**
   - Missing value detection: `.isnull().sum()`, `.isnull().mean()`
   - Imputation: `.fillna()`

5. **Aggregation & Grouping**
   - `.groupby()` - Group by column(s)
   - `.mean()`, `.sum()`, `.count()` - Aggregate functions

6. **Feature Engineering**
   - `.pd.cut()` - Create categorical bins from continuous data

7. **Visualization**
   - Bar charts, histograms, scatter plots
   - Plot customization (titles, labels, legends)

---

## 📈 Key Insights from Titanic Analysis

1. **Class Impact**: First-class passengers had significantly higher survival rates (~63%) compared to third-class (~24%)

2. **Gender Impact**: Females had much higher survival rates (~74%) compared to males (~19%)
   - Reflects the "women and children first" evacuation protocol

3. **Age Distribution**: Most passengers were in the 20-40 age range

4. **Fare Range**: Significant variation in ticket prices (£0-£512)

5. **Missing Data**: Age was the most problematic column with ~20% missing values

---

## 💡 Next Steps & Extensions

To extend this project, consider:

1. **Advanced Visualizations**
   - Heatmaps for correlation analysis
   - Multi-variable visualizations

2. **Statistical Analysis**
   - Chi-square tests for categorical relationships
   - Correlation analysis between numerical features

3. **Predictive Modeling**
   - Build a survival prediction model using classification algorithms
   - Train/test split and model evaluation

4. **Additional Datasets**
   - Apply learned techniques to other datasets
   - Compare analysis approaches

---

## 📝 Notes

- The Titanic dataset is a classic in data science education and machine learning
- It demonstrates real-world data quality issues (missing values, outliers)
- The survival distribution shows clear patterns based on socioeconomic and demographic factors
- This project provides a solid foundation for more advanced data analysis and machine learning

---

## 📚 Resources

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Documentation](https://matplotlib.org/contents.html)
- [Titanic Dataset Info](https://www.kaggle.com/c/titanic)
- [Jupyter Notebook Guide](https://jupyter-notebook.readthedocs.io/)

---

## ✅ Status

This project serves as:
- ✅ Learning resource for pandas fundamentals
- ✅ Example of exploratory data analysis workflow
- ✅ Foundation for data visualization techniques
- ✅ Stepping stone to machine learning projects

---

**Happy Learning! 🚀**
