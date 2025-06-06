# Exploratory Data Analysis (EDA) Project: Answering Questions through Data Visualization

## Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** on a dataset to uncover insights, understand data distributions, and identify relationships between variables. The primary goal was to answer specific questions related to the dataset by meticulously analyzing both categorical and numerical features and presenting findings through various visualization techniques.

## Key Activities

The project involved a comprehensive approach to data understanding and visualization, broken down into the following key areas:

### 1. Categorical Data Analysis

For categorical features within the dataset, I utilized various plotting techniques to understand the distribution and frequency of different categories.

* **Countplot:**
    * **Purpose:** Visualizing the frequency of each unique category in a categorical column.
    * **Example:** `sns.countplot(df['Embarked'])` was used to understand the distribution of passengers boarding from different embarkation points.

* **Pie Chart:**
    * **Purpose:** Displaying the proportion of each category relative to the whole.
    * **Example:** `df['Sex'].value_counts().plot(kind='pie', autopct='%.2f')` was used to visualize the gender distribution within the dataset.

### 2. Numerical Data Analysis

For numerical features, a range of statistical and visualization methods were employed to understand their distribution, central tendency, spread, and potential outliers.

* **Histogram:**
    * **Purpose:** Showing the distribution of a numerical variable by dividing it into bins and counting the number of observations in each bin.
    * **Example:** `plt.hist(df['Age'], bins=5)` was used to visualize the age distribution, segmented into 5 intervals.

* **Distplot (Distribution Plot):**
    * **Purpose:** A more advanced way to visualize the distribution of a numerical variable, often combining a histogram with a Kernel Density Estimate (KDE) plot.
    * **Example:** `sns.distplot(df['Age'])` provided a smooth representation of the age distribution.

* **Boxplot (Box and Whisker Plot):**
    * **Purpose:** Displaying the distribution of a numerical variable and highlighting its median, quartiles, and potential outliers.
    * **Example:** `sns.boxplot(df['Age'])` was used to quickly identify the central tendency, spread, and any outliers in the age data.
    * **Statistical Insights derived from Boxplot/Numerical Analysis:**
        * Minimum Age: `df['Age'].min()` = 0.42
        * Maximum Age: `df['Age'].max()` = 80.0
        * Mean Age: `df['Age'].mean()` = 29.699
        * Skewness of Age: `df['Age'].skew()` = 0.389 (indicating a slight positive skew in age distribution)

## Technologies Used

* **Python**
* **Pandas:** For data manipulation and analysis.
* **Matplotlib:** For fundamental plotting and customization.
* **Seaborn:** For creating aesthetically pleasing statistical graphics.

