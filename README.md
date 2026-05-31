# MSCS_634_Lab_1

## Advanced Big Data and Data Mining

### Lab 1: Data Visualization, Data Preprocessing, and Statistical Analysis

## Purpose of the Lab

The purpose of this lab was to gain hands-on experience with data visualization, data preprocessing, and statistical analysis using Python, Pandas, and Jupyter Notebook. The lab focused on exploring a real-world dataset, identifying patterns through visualizations, preparing data for analysis, and calculating important statistical measures.

The Titanic dataset was used to practice essential data mining and data preparation techniques. These techniques are important because real-world data is often incomplete, inconsistent, and contains outliers that can affect analysis results. Through this lab, I learned how to clean data, visualize trends, detect outliers, and summarize data using statistical methods.

---

## Dataset Used

**Dataset:** Titanic Passenger Dataset

The dataset contains information about passengers aboard the Titanic, including:

* Passenger ID
* Survival status
* Passenger class
* Name
* Gender
* Age
* Number of siblings/spouses aboard
* Number of parents/children aboard
* Ticket information
* Fare paid
* Cabin information
* Port of embarkation

---

## Data Visualization Performed

Several visualizations were created to better understand the dataset:

### 1. Histogram – Age Distribution

A histogram was created to visualize the distribution of passenger ages.

**Insight:**

* Most passengers were between 20 and 40 years old.
* There were fewer passengers at very young and very old ages.

### 2. Bar Chart – Passenger Class Distribution

A bar chart was created to compare the number of passengers in each travel class.

**Insight:**

* Third-class passengers represented the largest group.
* First-class and second-class passengers were fewer in comparison.

### 3. Pie Chart – Gender Distribution

A pie chart was used to show the proportion of male and female passengers.

**Insight:**

* Approximately 65% of passengers were male.
* Approximately 35% of passengers were female.

### 4. Box Plot – Fare Distribution

A box plot was created to examine the spread of passenger fares and identify potential outliers.

**Insight:**

* Most fares were relatively low.
* Several extreme fare values were identified as outliers.

---

## Data Preprocessing Activities

### Handling Missing Values

Missing values were identified using the `isnull()` function. Missing values in the Age column were replaced using the column mean.

**Reason:**
Replacing missing values with the mean helps preserve records while reducing data loss.

### Outlier Detection

The Interquartile Range (IQR) method was used to identify outliers in the Fare column.

**Result:**
Several fare values were identified as outliers because they were significantly higher than the majority of fares.

### Data Reduction

Random sampling was used to reduce the dataset size by selecting 50% of the records.

**Reason:**
Data reduction can improve processing speed while maintaining a representative sample of the dataset.

### Data Scaling and Discretization

Min-Max Scaling was applied to normalize age values between 0 and 1.

Age values were also discretized into categories:

* Young
* Adult
* Senior

**Benefit:**
Scaling improves consistency for machine learning algorithms, while discretization simplifies analysis and interpretation.

---

## Statistical Analysis Performed

### General Data Exploration

The dataset was examined using:

* `df.info()`
* `df.describe()`

These functions provided information about data types, missing values, and summary statistics.

### Central Tendency Measures

The following measures were calculated:

* Minimum
* Maximum
* Mean
* Median
* Mode

**Insight:**
These measures helped identify the typical age of passengers and summarize the dataset's central values.

### Dispersion Measures

The following measures were calculated:

* Range
* Quartiles (Q1 and Q3)
* Interquartile Range (IQR)
* Variance
* Standard Deviation

**Insight:**
These measures showed how spread out the age values were and helped identify variability within the dataset.

### Correlation Analysis

A correlation matrix was generated for numerical variables.

**Insight:**
The correlation matrix helped identify relationships between variables such as age, fare, passenger class, and survival status.

---

## Key Insights

* Most Titanic passengers were between 20 and 40 years old.
* Third-class passengers made up the largest portion of the dataset.
* Male passengers significantly outnumbered female passengers.
* Passenger fares contained several extreme outliers.
* Missing values were present and required preprocessing before analysis.
* Statistical measures provided useful summaries of passenger characteristics.
* Correlation analysis helped reveal relationships among numerical variables.

---

## Challenges Faced

The primary challenge during this lab was setting up the Python environment and ensuring that all required libraries, including Pandas, Matplotlib, Seaborn, and Scikit-learn, were installed correctly in Jupyter Notebook.

Another challenge was understanding how to interpret visualizations and statistical outputs as a beginner. Through practice and experimentation, I learned how each visualization and preprocessing technique contributes to data preparation and analysis.

---

## Conclusion

This lab provided practical experience with the fundamental steps of data mining and data preparation. By working with the Titanic dataset, I learned how to explore data visually, clean and preprocess datasets, identify outliers, normalize data, and perform statistical analysis. These skills form an important foundation for future coursework and real-world data analytics projects.
