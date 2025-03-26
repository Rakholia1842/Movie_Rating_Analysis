# **Movie Rating Analysis 🎬📊**  
🔍 **Unveiling Insights from Movie Ratings & Box Office Performance**  
![Dashboard](https://github.com/Rakholia1842/Movie_Rating_Analysis/blob/main/Visulization/Movie_Rating_Analysis.png?raw=true)

## **📖 Project Overview**  
The **Movie Rating Analysis** project aims to analyze movie performance, trends, and audience preferences using **Python, SQL, and Power BI**. It provides insights into **ratings, revenue patterns, and genre success** through **data visualization and analytics**.  

## **🛠 Technologies Used**  
- **Python** (pandas, NumPy, Matplotlib)  
- **SQL** (SQLite for data storage & queries)  
- **Power BI** (interactive dashboard creation)  

## **📂 Project Structure**  
```
Movie-Rating-Analysis/
│── data/
│   ├── raw/                  # Original dataset
│   ├── cleaned_movies.csv     # Processed dataset
│── notebooks/
│   ├── data_cleaning.ipynb    # Data cleaning & preprocessing
│   ├── sql_queries.ipynb      # SQL analysis
│   ├── visualizations.ipynb   # Matplotlib visualizations
│── reports/
│   ├── PowerBI_Dashboard.pbix # Power BI report
│── README.md                 # Project documentation
│── requirements.txt          # Python dependencies
│── LICENSE                   # Project license
```

## **📊 Data Insights & Visualizations**  
✔ **Ratings Distribution**: Understanding audience ratings using histograms.  
✔ **Genre Performance**: Identifying **best-performing movie genres**.  
✔ **Revenue Analysis**: Comparing **box office success by release year**.  
✔ **SQL Queries**: Extracting **actionable insights** from structured data.  

## **🚀 How to Run the Project**  

### **1️⃣ Install Dependencies**  
```bash
pip install pandas numpy matplotlib sqlalchemy jupyter
```

### **2️⃣ Load and Clean Data**  
```python
import pandas as pd
df = pd.read_csv('data/movies.csv')
df_cleaned = df.dropna().copy()
```

### **3️⃣ Run SQL Queries**  
```python
import sqlite3
conn = sqlite3.connect('movies.db')
df_cleaned.to_sql('movies', conn, if_exists='replace', index=False)
```

### **4️⃣ Generate Visualizations**  
```python
import matplotlib.pyplot as plt
df_cleaned['Rating'].hist(bins=20)
plt.show()
```
![Average Rating by Genre](https://github.com/Rakholia1842/Movie_Rating_Analysis/blob/main/Visulization/Average%20Rating%20by%20Genre.png?raw=true)

![Total Box Office Revenue Over Years](https://github.com/Rakholia1842/Movie_Rating_Analysis/blob/main/Visulization/Total%20Box%20Office%20Revenue%20Over%20Years.png?raw=true)


### **5️⃣ Open Power BI Dashboard**  
- Import **cleaned_movies.csv** into Power BI.  
- Use **bar charts, line charts, and slicers** to explore the data.  

## **🤝 Contributing**  
Contributions are welcome! Feel free to submit **pull requests** with improvements.  

---

This **README** will ensure **clarity and professionalism** for your **GitHub project**, making it easy to showcase to recruiters and collaborators. 🚀 Let me know if you need refinements! 😊
