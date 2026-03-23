
# 🚑 AI-Based Emergency Department Flow Optimization System

AI-based system to optimize Emergency Department (ED) patient flow using predictive analytics and operational dashboards.


## 📌 Project Overview
This project explores how Artificial Intelligence can improve patient flow management in Emergency Departments, focusing on **operational efficiency** rather than clinical decision-making.

The system acts as a **digital operations assistant** to help hospitals reduce:
- Overcrowding  
- Waiting times  
- Trolley congestion  


## 🎯 Project Aim
To design and prototype an AI-driven operational intelligence system that:

- Improves Emergency Department patient flow  
- Reduces waiting and trolley times  
- Optimizes bed allocation  
- Supports clinical staff by reducing administrative workload  




## ⚠️ Key Challenges Addressed
- Emergency department overcrowding  
- Long waiting times for investigations and admission  
- Delayed bed allocation  
- Manual coordination between departments  

---

## 🧠 Core System Components

### 🔹 Patient Flow Prediction
- Predicts length of stay in ED  
- Estimates admission vs discharge likelihood  
- Identifies high-risk prolonged waiting cases  

### 🔹 Bottleneck Detection
Detects delays in:
- Radiology  
- Laboratory investigations  
- Specialist reviews  
- Bed assignment  

### 🔹 Intelligent Bed Management
- Predicts near-term bed availability  
- Detects delayed discharges  
- Suggests optimal admission pathways  

### 🔹 Automated Alerts & Coordination
- Automated alerts to departments  
- Escalation if delays exceed thresholds  

### 🔹 📊 Real-Time Operational Dashboard
Displays:
- ED occupancy  
- Waiting times by triage level  
- Trolley patient count  
- Predicted bed availability  



## 📂 Data Used
- Simulated or anonymised hospital operational data  
- No clinical or patient-identifiable data used  



## 🛠️ Technology Stack
- Python  
- Jupyter Notebook (Anaconda)  
- Pandas, NumPy  
- Machine Learning (classification & forecasting models)  
- Streamlit (for dashboard)  
- Data visualisation libraries (Matplotlib, etc.)

## Documentation
- [System Components](docs/system_components.md)
- [Ethics and Prototype Declaration](docs/ethics_and_prototype_declaration.md)



## ▶️ How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/abhishekbabu-git/ed-flow-optimization-ai
2.	Navigate to the project folder:
3.	cd ed-flow-optimization-ai
4.	Install required libraries:
5.	pip install pandas numpy matplotlib
6.	Open Jupyter Notebook:
7.	jupyter notebook
8.	Run the notebook:
o	Open the .ipynb file
o	Run all cells
________________________________________
📈 Sample Outputs
•	Patient count by department (bar chart)
•	Average waiting time
•	Maximum waiting time
•	Patients waiting over threshold (e.g., 3+ hours)
________________________________________
🔐 Ethics & Governance
•	No clinical decisions made by AI
•	Advisory-only recommendations
•	GDPR-compliant design
•	Transparent and explainable models
________________________________________
🚀 Expected Outcomes
•	Reduced ED waiting times
•	Improved bed turnaround
•	Lower trolley patient numbers
•	Improved patient experience
________________________________________
👨‍💻 Author
Abhishek Babu
Student | Aspiring Software Engineer
Ireland 🇮🇪
________________________________________
⭐ Future Improvements
•	Real-time hospital data integration
•	Advanced ML models for prediction
•	Live dashboard deployment (Streamlit Cloud)
•	Integration with hospital systems
________________________________________


