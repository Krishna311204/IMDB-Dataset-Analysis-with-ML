**IMDb Top 5000 TV Shows — ML Analysis**

This project performs a machine learning-based data analysis on the IMDb Top 5000 TV Shows dataset. Using a Random Forest Regressor model, we predict average ratings of TV shows based on attributes such as title, start year, genre, number of votes, and more.

---

**Dataset**

- File: `imdb_top_5000_tv_shows.csv`  
- Rows: 5000  
- Columns: 12  
- Key Features:  
  - `primaryTitle`: Name of the TV show  
  - `startYear`, `endYear`  
  - `averageRating`, `numVotes`  
  - `directors`, `writers`, `genres`  

---

**Workflow**

1. **Data Cleaning**  
   - Removed unnecessary columns (IDs, HTML links)  
   - Dropped rows with missing values  

2. **Encoding**  
   - Encoded `primaryTitle`, `directors`, `writers`, `genres` using LabelEncoder  

3. **Model Building**  
   - Model: RandomForestRegressor  
   - Split: 80% training, 20% testing  
   - Evaluation: Mean Squared Error (MSE), R² Score  

4. **Results**  
   - MSE: ~0.0201  
   - R² Score: ~0.8921  

---

**Visualizations**

- Actual vs Predicted Ratings (scatter plot)  
- Feature Importance (bar plot)  

These visualizations help understand model accuracy and the most influential features.

---

**How to Run**

1. Upload the dataset to your environment (e.g., Google Colab)  
2. Copy and paste the code from the provided notebook or script  
3. Run all cells to preprocess, train the model, and visualize results  

---

**Requirements**

Install the required Python libraries:

```
pip install pandas scikit-learn seaborn matplotlib
```

---

**Future Enhancements**

- Try deep learning models for better predictions  
- Analyze trends over years  
- Genre-based insights  
- Build an interactive dashboard using Streamlit or Plotly  

---
