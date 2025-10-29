#  Flight Price Prediction Project

This project predicts airline ticket prices using real flight data.  
It includes Exploratory Data Analysis (EDA), feature preprocessing, and a Machine Learning regression model.

---

##  Dataset Description

| Feature | Description |
|--------|-------------|
| airline | Airline name |
| source_city | Departure city |
| destination_city | Arrival city |
| departure_time | Time of departure |
| arrival_time | Time of arrival |
| stops | Number of stops |
| class | Travel class (Business/Economy) |
| duration | Flight duration (hours) |
| days_left | Days before flight |
| price (target) | Ticket price |

---

##  EDA & Key Insights

✔ Ticket prices increase when fewer days are left  
✔ Business class flights are significantly more expensive  
✔ Flights with one stop are the most expensive
✔ Longer flight duration tends to increase price (but weak effect)
---

##  Machine Learning Approach

| Step       | Technique Used |
|------------|----------------|
| Data Split | Train/Test split |
| Categorical Features | OneHotEncoder |
| Numerical Features | SimpleImputer (median) |
| Models Tested | Linear Regression / Random Forest |
| Evaluation Metrics | MAE / MSE / RMSE / R² |

 Best model: **Random Forest Regressor**  
 Better handling of non-linear relationships in flight pricing

---

##  Model Performance (on Test Data)

| Model             | MAE ↓   | RMSE ↓ | R² ↑    |
|-------------------|---------|--------|---------|
| Linear Regression | 4553.29 | 6761.71 | 0.91   |
| Random Forest     | 1077.35 | 2786.68 | 0.98   |


---

##  Tech Stack

- Python
- Pandas, NumPy
- Scikit-Learn
- Matplotlib, Seaborn
- Jupyter Notebook

---
