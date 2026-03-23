# System Components Overview

This document explains the key components of the AI-Based Emergency Department Flow Optimization System.


## 1. Data Input Layer

This component handles the input data required for the system.

**Source:**
- CSV file containing patient data

**Columns used:**
- patient_id
- arrival_time
- triage_level
- department
- doctor
- wait_time_minutes
- treatment_time_minutes
- total_time_minutes
- outcome


## 2. Data Preprocessing

This step prepares raw data for analysis.

**Tasks:**
- Handle missing values
- Convert time fields into usable format
- Categorize triage levels
- Clean inconsistent entries


## 3. Feature Engineering

New features are created to improve predictions.

**Examples:**
- Waiting time category (Short / Medium / Long)
- Peak hour indicator
- Patient load per department

---

## 4. Prediction Module

This is the core AI logic.

**Function:**
- Predict if a patient will experience delay

**Approach:**
- Simple rule-based or ML model (if added later)

**Example Logic:**
- If wait_time_minutes > threshold → Delay
- Else → No Delay

---

## 5. Visualization Dashboard

Displays insights using charts.

**Tools used:**
- Matplotlib / Pandas

**Visuals:**
- Patient wait time distribution
- Delay prediction results (bar chart)

---

## 6. Output Layer

Final results presented to users.

**Outputs:**
- Delay predictions
- Charts and graphs


---

## 7. Future Enhancements

- Real-time data integration
- Advanced ML models
- Web-based dashboard
- Integration with hospital systems

---

## 8. Bottleneck Detection

This component identifies delays in the Emergency Department workflow by analyzing patient waiting and treatment times.

### Purpose
To find where patients are experiencing the longest delays so that hospital staff can take action.

### How It Works

The system analyzes key time metrics:
- wait_time_minutes
- treatment_time_minutes
- total_time_minutes

### Simple Detection Logic

A bottleneck is identified when:
- Waiting time exceeds a defined threshold (e.g., 60 minutes)
- Certain departments consistently show higher delays
- Specific doctors are overloaded with patients

### Example Rules

- If wait_time_minutes > 60 → Mark as "High Delay"
- If many patients in one department have high delays → Department bottleneck
- If a doctor handles too many patients → Resource bottleneck

### Output

The system highlights:
- High delay patients
- Departments with congestion
- Overloaded doctors

### Visualization

Bottlenecks can be shown using:
- Bar charts (delay counts)
- Department-wise comparison charts
- Time-based trends

### Benefits

- Helps reduce patient waiting time
- Improves resource allocation
- Supports better decision-making

---

## 9. Dashboard Concept

### Overview
The dashboard provides a visual representation of Emergency Department data to help users quickly understand patient flow, delays, and system performance.

### Purpose
The main goal of the dashboard is to:
- Monitor patient waiting times
- Identify delays and bottlenecks
- Support decision-making for hospital staff

### Key Features

#### 1. Wait Time Visualization
- Displays patient waiting times using charts
- Helps identify long waiting periods

#### 2. Delay Prediction Results
- Shows number of patients with predicted delays vs no delays
- Typically displayed as a bar chart

#### 3. Department Workload
- Compares number of patients across departments
- Helps identify overloaded departments

#### 4. Bottleneck Indicators
- Highlights areas with high delays
- Supports quick action

### Tools Used
- Python libraries such as:
  - Pandas (data handling)
  - Matplotlib (charts and graphs)

### Example Visuals
- Bar chart: Number of Patients by Department
- Bar chart: Average Waiting Time by Department

### How It Works

1. Data is loaded from CSV
2. Processed and analyzed
3. Predictions are generated
4. Results are displayed as charts

### Benefits
- Easy to understand insights
- Real-time decision support (future scope)
- Improves operational efficiency

---

## Conclusion

The system combines data processing, prediction logic, and visualization to improve patient flow and reduce waiting times in the Emergency Department.
