# Data Wrangling Classwork

This repository contains Jupyter Notebook with beginner-friendly explanations for each step in the data wrangling process.  
It demonstrates common data cleaning tasks such as handling missing values, removing duplicates, merging datasets, and treating outliers using the Interquartile Range (IQR) method.

## Contents
- Annotated code cells with comments for easy understanding
- Example datasets (`hr_messy.csv`, `retail_classwork_messy.csv`)
- Outlier detection and treatment functions
- **NEW**: Practice assignments and tests for hands-on learning

## Datasets Available

### 1. HR Dataset (`hr_messy.csv`)
A messy HR dataset with 2,052 employee records containing:
- **Data Quality Issues**: Missing values, inconsistent formatting, outliers, duplicates
- **Columns**: EmployeeID, Name, Department, Gender, Age, Salary, PerformanceScore, JoinDate
- **Challenges**: Age values of 999, negative salaries (-10000), missing dates, inconsistent gender formats

### 2. Retail Dataset (`retail_classwork_messy.csv`)
A retail transaction dataset with 5,100 records containing:
- **Data Quality Issues**: Missing values, invalid data types, duplicates
- **Columns**: TransactionID, Store, Category, Date, Quantity, UnitPrice, Revenue

## Practice Assignments (HR Dataset)

### 🟢 Beginner Level (Start Here!)

#### Assignment 1: Basic Data Exploration
**Objective**: Learn to explore and understand messy data
```python
# Your tasks:
# 1. Load hr_messy.csv and display first 10 rows
# 2. Check dataset shape (rows and columns)
# 3. Identify data types of each column
# 4. Count missing values in each column
# 5. Generate summary statistics for numerical columns
```

#### Assignment 2: Missing Value Detection
**Objective**: Practice identifying and understanding missing data patterns
```python
# Your tasks:
# 1. Create a missing value heatmap
# 2. Calculate percentage of missing values in each column
# 3. Identify which departments have the most missing data
# 4. Check if missing values are random or follow a pattern
```

#### Assignment 3: Data Type Conversion
**Objective**: Learn to convert data types properly
```python
# Your tasks:
# 1. Convert JoinDate to datetime format
# 2. Convert Age and Salary to numeric types
# 3. Handle conversion errors gracefully
# 4. Verify data types after conversion
```

### 🟡 Intermediate Level

#### Assignment 4: Handling Missing Values
**Objective**: Practice different strategies for missing data
```python
# Your tasks:
# 1. Fill missing Age values using median (appropriate for age data)
# 2. Fill missing Salary values using mean (appropriate for salary data)
# 3. Fill missing JoinDate using mode (most common date)
# 4. Compare different filling strategies and their impact
```

#### Assignment 5: Data Standardization
**Objective**: Learn to clean and standardize text data
```python
# Your tasks:
# 1. Standardize Gender column (M/male → Male, F/female → Female)
# 2. Fix PerformanceScore typos (Excellnt → Excellent, G00d → Good)
# 3. Standardize Department names (remove extra spaces, consistent case)
# 4. Create a mapping dictionary for each standardization
```

#### Assignment 6: Duplicate Detection and Removal
**Objective**: Practice identifying and handling duplicates
```python
# Your tasks:
# 1. Find exact duplicate rows
# 2. Find duplicates based on EmployeeID
# 3. Find duplicates based on Name + Department combination
# 4. Decide which duplicates to keep and which to remove
```

### 🟠 Advanced Level

#### Assignment 7: Outlier Detection and Treatment
**Objective**: Master outlier identification and handling strategies
```python
# Your tasks:
# 1. Use IQR method to detect outliers in Age and Salary
# 2. Use Z-score method to detect outliers
# 3. Compare results from both methods
# 4. Implement three treatment strategies:
#    - Capping outliers (winsorization)
#    - Removing outliers completely
#    - Log transformation for salary
```

#### Assignment 8: Data Validation and Cleaning
**Objective**: Apply business logic to clean data
```python
# Your tasks:
# 1. Remove records with Age = 999 (invalid age)
# 2. Remove records with negative salaries
# 3. Validate that Age is between 18-70
# 4. Validate that Salary is between 20000-200000
# 5. Create a data quality report
```

#### Assignment 9: Advanced Data Transformation
**Objective**: Create new features and insights
```python
# Your tasks:
# 1. Calculate years of service from JoinDate
# 2. Create salary bands (Low: <40k, Medium: 40k-60k, High: >60k)
# 3. Calculate department-wise average salary
# 4. Create performance vs salary analysis
```

## 🧪 Practice Tests

### Test 1: Data Quality Assessment (15 minutes)
**Scenario**: You're a data analyst reviewing the HR dataset before analysis
```python
# Questions:
# 1. How many missing values are in the Age column?
# 2. What percentage of records have missing JoinDate?
# 3. How many unique departments are there?
# 4. What is the range of Age values (min to max)?
# 5. How many records have negative salaries?
```

### Test 2: Data Cleaning Implementation (20 minutes)
**Scenario**: Clean the HR dataset following best practices
```python
# Tasks:
# 1. Load and explore the data
# 2. Handle all missing values appropriately
# 3. Remove invalid data (Age=999, negative salaries)
# 4. Standardize text columns
# 5. Save cleaned dataset
# 6. Document your cleaning decisions
```

### Test 3: Outlier Analysis (15 minutes)
**Scenario**: Analyze and treat outliers in the salary data
```python
# Tasks:
# 1. Detect outliers using IQR method
# 2. Detect outliers using Z-score method
# 3. Compare the two methods
# 4. Choose and implement appropriate treatment
# 5. Justify your treatment choice
```

## 🎯 Learning Objectives

By completing these assignments, you will be able to:

### Technical Skills
- ✅ Load and explore messy datasets
- ✅ Identify and handle missing values
- ✅ Detect and treat outliers
- ✅ Standardize text and categorical data
- ✅ Remove duplicates and invalid data
- ✅ Convert data types appropriately
- ✅ Create data quality reports

### Analytical Thinking
- ✅ Choose appropriate cleaning strategies
- ✅ Understand the impact of cleaning decisions
- ✅ Document data cleaning processes
- ✅ Validate cleaning results
- ✅ Make business-appropriate decisions

### Best Practices
- ✅ Always explore data before cleaning
- ✅ Use appropriate methods for different data types
- ✅ Document your cleaning steps
- ✅ Validate results after cleaning
- ✅ Consider business context in decisions

## 📚 Additional Resources

### Data Quality Issues in HR Dataset
- **Missing Values**: Age (12%), Salary (20%), JoinDate (26%)
- **Invalid Data**: Age = 999, Negative salaries (-10000)
- **Inconsistent Formatting**: Gender (M/male/Male), PerformanceScore (Excellnt/G00d)
- **Duplicates**: Some employees appear multiple times

### Cleaning Strategies to Try
1. **Missing Values**: Mean, median, mode, forward fill, backward fill
2. **Outliers**: IQR method, Z-score method, capping, removal, transformation
3. **Text Cleaning**: String methods, regular expressions, mapping dictionaries
4. **Data Validation**: Business rules, range checks, format validation

## 🚀 Getting Started

1. **Clone this repository**:
   ```bash
   git clone https://github.com/baysquire/Data-Wrangling-Classwork.git
   ```

2. **Open Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

3. **Start with Beginner Assignments**:
   - Begin with Assignment 1 (Basic Data Exploration)
   - Progress through assignments sequentially
   - Complete practice tests to assess understanding

4. **Use the Demo Notebooks**:
   - `Data Wrangling [DEMO].ipynb` - Step-by-step explanations
   - `Data Wrangling [Classwork].ipynb` - Guided practice

## Requirements
- Python 3.x
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn

## 📝 Submission Guidelines

When completing assignments:
1. **Document your approach** - Explain why you chose each cleaning method
2. **Show your work** - Include intermediate steps and outputs
3. **Validate results** - Check that your cleaning actually improved data quality
4. **Reflect on decisions** - What would you do differently next time?

## 🤝 Contributing

Found an issue or have a suggestion? Feel free to:
- Open an issue
- Submit a pull request
- Suggest additional practice problems
- Share your solutions and insights

## License
This project is open-source and available under the MIT License.

---

**Happy Data Wrangling! 🎉**

*Remember: Clean data leads to better insights, and practice makes perfect!*
