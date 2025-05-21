# 🌍 Sustainability Analytics in Global Logistics

This project aims to support Amazon’s 2040 net-zero carbon goal by analyzing and optimizing carbon emissions across global logistics operations. Using a data-driven approach, we explore emission patterns by transport mode, region, vehicle age, and other key factors to make strategic recommendations that reduce environmental impact.

---

## 📌 Project Objectives

- Analyze CO₂ emissions from transportation across different modes (Air, Sea, Land).
- Identify high-emission patterns based on distance, fuel usage, and efficiency.
- Predict CO₂ emissions using machine learning models.
- Recommend logistics optimizations to improve sustainability.

---

## 🗂 Dataset Overview

The project uses a simulated logistics dataset with the following features:

| Column                 | Description                                      |
|------------------------|--------------------------------------------------|
| `Transport_ID`         | Unique identifier for transport record           |
| `Mode`                 | Mode of transport: Air, Sea, or Land             |
| `Distance_km`          | Total travel distance in kilometers              |
| `Fuel_Used_L`          | Fuel consumed in liters                          |
| `CO2_Emissions_kg`     | Emissions in kilograms of CO₂                    |
| `Region`               | Region of operation (Asia, Europe, etc.)         |
| `Vehicle_Age`          | Age of the vehicle in years                      |
| `Load_Capacity_Ton`    | Capacity of the vehicle in tons                  |
| `Speed_kmph`           | Average speed during transit                     |

---

## ⚙️ Technologies Used

- **Python**: Core programming and analysis
- **Pandas, NumPy**: Data manipulation
- **Seaborn, Matplotlib**: Visualizations
- **Scikit-learn**: Machine learning models
- **Joblib**: Model serialization

---

## 🔍 Project Workflow

### 1. Data Cleaning
- Removed null values and ensured consistent types.

### 2. Feature Engineering
- Created `Fuel_Efficiency_km_per_l` and `Emission_per_km`.
- Applied one-hot encoding to categorical columns.

### 3. Exploratory Data Analysis
- Box plots of emissions by transport mode.
- Correlation heatmaps to identify strong predictors.

### 4. Predictive Modeling
- Trained a `RandomForestRegressor` model to predict `CO2_Emissions_kg`.
- Evaluated with RMSE and R² score.

### 5. Optimization Suggestions
- Identified transport IDs with below-average fuel efficiency.
- Suggested emissions improvements based on top-performing entries.

---

## 📈 Results

- 🚚 Land transport showed higher emission variability.
- 🌫️ Efficiency decreases in older vehicles and long-distance hauls.
- 🧠 Model R² Score: ~0.95 — Strong predictive performance.

---

## 📊 Visualizations

- Transport Mode vs Emission box plots
- Feature correlation heatmap
- Top emission contributors by region

---

## 🔮 Future Improvements

- Integrate real-world APIs for traffic and weather conditions.
- Add route clustering using geospatial analysis.
- Deploy as a dashboard using Streamlit or Tableau for real-time use.

---

## 📁 Files

- `transport_logistics.csv`: Input data
- `optimized_logistics_data.csv`: Post-processed results
- `optimization_suggestions.csv`: Suggested improvements
- `co2_emission_model.pkl`: Trained model

---

## 👨‍💻 Author

**Harsh Sonkar**  
Senior Data Engineer & Sustainability Analyst  
📧 contact.harshsonkar@gmail.com 
🌐 [LinkedIn](www.linkedin.com/in/harsh-sonkar-232573250/) | [Portfolio](https://hq969.github.io/harsh-sonkar-portfolio-hk/)

---

## 📜 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

