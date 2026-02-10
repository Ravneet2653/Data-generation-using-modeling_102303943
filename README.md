# Data-generation-using-modeling_102303943
# Data Generation using Modelling and Simulation for Machine Learning

## 📌 Overview
This project demonstrates how synthetic data can be generated using modelling and simulation techniques and then used to train and evaluate machine learning models.

A physics-based **projectile motion simulator** was developed in Python, and the generated dataset was used to compare the performance of multiple regression algorithms.

---

## 🎯 Objectives
- Design a simulation-based data generation system  
- Perform **1000 simulations** using randomly generated physical parameters  
- Apply and compare multiple machine learning regression models  
- Identify the best-performing model using evaluation metrics  

---

## 🛠 Step 1: Simulation Tool Selection
A custom physics-based simulation tool was built using:

- **Python**
- **NumPy** for numerical computations
- **Pandas** for data handling
- **Matplotlib** for visualization

Python with NumPy is widely used in scientific and engineering simulations, making it a reliable environment for this project.

---

## ⚙️ Step 2: Environment Setup and Execution
The simulator and ML pipeline were implemented and executed using **Google Colab**.

- Required libraries were imported  
- Simulation functions were tested  
- Parameter values were varied to observe their impact  

No manual installation was required as Google Colab provides a pre-configured environment.

---

## 📐 Step 3: Parameter Selection and Bounds

| Parameter     | Description                       | Lower Bound | Upper Bound |
|---------------|-----------------------------------|-------------|-------------|
| Velocity      | Initial velocity (m/s)            | 10          | 100         |
| Angle         | Launch angle (degrees)            | 10          | 80          |
| Gravity       | Gravitational acceleration (m/s²) | 9.5         | 10.5        |
| AirResistance | Air resistance coefficient        | 0.0         | 0.1         |

These bounds were selected based on realistic physical constraints.

---

## 🔁 Step 4 & Step 5: Data Generation Using Simulation

- Random values were generated within the defined parameter ranges  
- Each parameter set was passed to the simulator  
- The **horizontal range** of the projectile was calculated  
- A total of **1000 simulations** were performed  
- The generated dataset was saved as `data.csv`  

---

## 📊 Dataset Preview

| Velocity | Angle | Gravity | AirResistance | Range  |
|----------|-------|---------|---------------|--------|
| 84.24    | 27.43 | 9.52    | 0.080         | 562.38 |
| 33.50    | 19.26 | 10.30   | 0.042         | 65.03  |
| 84.01    | 64.44 | 10.46   | 0.061         | 494.19 |
| 95.42    | 13.03 | 9.63    | 0.014         | 409.70 |
| 27.63    | 54.65 | 10.28   | 0.043         | 67.15  |

---

## 🤖 Step 6: Machine Learning Models Used
The following regression models were trained and evaluated:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Support Vector Regressor (SVR)  
- K-Nearest Neighbors (KNN) Regressor  

---

## 📈 Evaluation Metrics
Each model was evaluated using:

- **Mean Absolute Error (MAE)**
- **Root Mean Square Error (RMSE)**
- **R² Score**

---

## 🏆 Model Comparison Results

| Model                    | MAE    | RMSE   | R² Score |
|--------------------------|--------|--------|----------|
| Linear Regression        | 75.97  | 101.85 | 0.8129   |
| Decision Tree Regressor  | 21.15  | 31.30  | 0.9823   |
| Random Forest Regressor  | 12.18  | 18.04  | 0.9941   |
| Support Vector Regressor | 104.32 | 156.60 | 0.5577   |
| KNN Regressor            | 14.62  | 22.74  | 0.9907   |

---

## 📉 Result Visualization
A bar graph comparing the **R² scores** of all models was plotted. The visualization clearly shows that the **Random Forest Regressor** outperforms the other models.

---

## ✅ Conclusion
- Simulation-based data generation is effective when real-world data is unavailable  
- Machine learning models can successfully learn from synthetic data  
- The **Random Forest Regressor** achieved the best performance  
- This approach is scalable and can be applied to other simulation-based domains  

---

## 👤 Author
Ravneet Kaur
