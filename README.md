# Olympic Data Analysis Project

This project is a comprehensive data science and data analysis project focused on exploring Olympic data. The aim was to learn and apply various data preprocessing, cleaning, and visualization techniques using Python in a Jupyter Notebook environment.

---

## Project Overview

The project involves analyzing Olympic participation and performance data stored in a Parquet file. The main goals were to:
- Clean and preprocess the dataset by handling missing values, renaming columns, adjusting data types, and removing duplicate records.
- Perform exploratory data analysis (EDA) to uncover trends and insights.
- Visualize the data using various types of plots to illustrate participation trends, medal distributions by country and discipline, and performance patterns over time.

---

## Data Preprocessing and Cleaning

1. **Data Loading & Column Renaming:**  
   The dataset was loaded from a Parquet file using the `pyarrow` and `pandas` libraries. Columns were renamed to provide clear, descriptive titles for each variable.

2. **Missing Value Handling:**  
   Missing values were identified and addressed:
   - Numeric columns (e.g., `year` and `place`) were filled using their median values.
   - Categorical columns (e.g., `type`, `discipline`, and `noc`) were filled using their mode (most frequent value).
   - For the `team` column, missing entries were replaced with "Unknown".
   - The `medal` column missing values were replaced with "No Medal".

3. **Data Type Conversion:**  
   To ensure the accuracy of subsequent analyses, data types were explicitly converted (e.g., converting `year` and `place` to integers, and changing the `tied` column from boolean to integer).

4. **Duplicate Removal:**  
   Duplicate records were detected and removed to maintain data integrity.

---

## Exploratory Data Analysis (EDA)

After cleaning, the dataset was explored to answer key questions such as:
- How has Olympic participation changed over the years?
- Which countries have the highest number of medals?
- What are the most successful sports in terms of medal counts?
- How have medal distributions evolved across different countries over time?
- Who are the top-performing athletes based on their medal counts?

This stage laid the groundwork for insightful visualizations by grouping and aggregating data appropriately.

---

## Visualizations

The analysis was complemented by a series of visualizations created with **Matplotlib** and **Seaborn**:
- **Yearly Participation Trends:** A bar chart visualizing the number of participants each year.
- **Medals by Country:** A bar chart showcasing the top 10 countries with the most medals.
- **Medals by Discipline:** A bar chart highlighting the top 10 sports by medal count.
- **Heatmap of Medals Over Time:** An annotated heatmap representing the medal distribution by year for the top 20 countries.
- **Top Athletes:** A horizontal bar chart showing the top 10 athletes with the most medals.

These visualizations not only illustrate the key findings of the project but also provide a clear picture of how Olympic trends have evolved over time.

---

## Project Conclusions

The analysis demonstrated:
- A noticeable trend in Olympic participation, with fluctuations over the years.
- A concentration of medals among a few leading countries.
- Variability in success across different sports disciplines.
- Clear patterns in how countries' performances have changed over time.
- Insights into individual athlete achievements, emphasizing the importance of individual performances.

Overall, this project successfully applied data cleaning, EDA, and visualization techniques to extract meaningful insights from Olympic data, serving as an effective learning tool for data science practices.

---

## Technologies Used

- **Python:** Primary programming language for data manipulation and analysis.
- **Pandas:** Data processing and manipulation.
- **PyArrow:** Reading Parquet file formats.
- **Matplotlib & Seaborn:** Data visualization libraries.
- **Jupyter Notebook:** Interactive coding and analysis environment.

---

