# 🚗 Suspension Ride Quality Analysis Using MATLAB

## 📌 Project Overview
This project presents a comprehensive quantitative analysis of vehicle suspension ride quality using experimentally measured position and acceleration data. The objective is to evaluate how suspension response and perceived ride comfort vary under low-frequency and high-frequency excitation conditions using MATLAB.

This work was originally completed as an **assignment project** for the course **“Practical MATLAB Skills” by MathWorks (Coursera)**. While the core analysis follows the project outline and requirements specified in the course, the study was **significantly extended beyond the assignment scope** through additional metrics, visualizations, and engineering interpretation to demonstrate deeper technical understanding and independent analytical effort.

---

## 🎓 Academic Context and Original Contribution

### Course Context
- **Course:** Practical MATLAB Skills  
- **Provider:** MathWorks (Coursera)  
- **Project Type:** Applied engineering assignment  
- **Primary Focus:** MATLAB-based data analysis and engineering interpretation  

### Independent Extensions Beyond Coursework
In addition to implementing all required project steps, the following **original analytical extensions** were introduced:

- Extended statistical performance metrics beyond basic RMS analysis  
- Peak and peak-to-peak response evaluation  
- Quantitative comparison using ratios and percentage changes  
- A combined comfort index capturing both displacement and acceleration effects  
- Advanced comparative visualizations for clearer engineering interpretation  
- Physics-based explanation of frequency-dependent behavior  
- Design-oriented conclusions and engineering recommendations  

These additions reflect **independent problem-solving, critical thinking, and professional engineering judgment** beyond the original assignment requirements.

---

## 🧪 Experimental Setup
The experimental system consists of a vehicle suspension assembly mounted on vertically actuated platforms. The platforms undergo sinusoidal motion while sensor data are recorded at a fixed reference point on the suspension.

Two sensors are used:
- **Position sensor** – measures vertical displacement  
- **Acceleration sensor** – measures vertical acceleration  

The experiment runs for **30 seconds**, divided into three phases:

| Time Interval (s) | Condition | Excitation Frequency |
|------------------|----------|----------------------|
| 0 – 10 | Active motion | 0.5 Hz (Low frequency) |
| 10 – 20 | Stationary | No motion |
| 20 – 30 | Active motion | 5 Hz (High frequency) |

---

## 🧾 Data Import and Preprocessing
Raw sensor outputs were provided as voltage measurements and imported into MATLAB as column vectors. To ensure reproducibility and clean execution, the data were stored in a `.mat` file and reloaded within a structured MATLAB Live Script.

Sensor voltages were converted into physically meaningful quantities using provided calibration relationships:
- **Position:** centimeters (cm)  
- **Acceleration:** gravitational units (G)  

Sensor offsets were removed prior to scaling to ensure accurate zero-reference measurements.

---

## ✂️ Test Segmentation
To focus on dynamic behavior, only the active excitation intervals were extracted:
- Low-frequency response (0.5 Hz)  
- High-frequency response (5 Hz)  

A dedicated test-time vector (0–10 s) was constructed to ensure consistent alignment across datasets and visualizations.

---

## 📈 Time-Domain Response Analysis
Position and acceleration responses were visualized for both excitation frequencies to assess qualitative suspension behavior.

Key observations:
- Low-frequency excitation produced larger, smoother displacement oscillations  
- High-frequency excitation produced smaller displacements but significantly higher acceleration fluctuations  

These observations motivated further quantitative analysis.

---

## 📊 Quantitative Performance Metrics

### Required Coursework Analysis
As specified in the course outline, the following metrics were computed:
- Root-mean-square (RMS) position  
- Root-mean-square (RMS) acceleration  
- Frequency-based comparison of RMS values  

### Additional Independent Analysis
To deepen the evaluation, the following metrics were added:
- Absolute peak response values  
- Peak-to-peak amplitudes  
- RMS ratios and percentage changes between excitation conditions  
- A combined comfort index incorporating both displacement and acceleration effects  

These metrics enable a more complete assessment of both sustained ride comfort and transient vibration severity.

---

## 📉 Comparative Visualization
Multiple visualization techniques were employed to support engineering interpretation:
- Overlaid time-domain plots  
- Aligned subplots for position and acceleration comparison  
- Grouped bar charts for RMS-based performance comparison  

These visualizations emphasize design-oriented insight rather than raw signal inspection alone.

---

## 🧠 Engineering Interpretation
The analysis shows that suspension acceleration increases sharply with excitation frequency despite a reduction in displacement. This behavior is consistent with vibration principles, where acceleration is strongly influenced by excitation frequency. Consequently, high-frequency inputs generate disproportionately larger inertial forces, leading to increased ride harshness.

---

## 🧩 Conclusions and Engineering Takeaways
- Low-frequency excitation results in larger suspension motion but relatively mild acceleration levels  
- High-frequency excitation significantly amplifies acceleration response while reducing displacement  
- Ride discomfort is governed primarily by acceleration rather than visible suspension motion  
- Acceleration-based metrics are more sensitive and reliable indicators of ride quality degradation  
- Suspension tuning efforts should prioritize mitigation of high-frequency acceleration transmission through damping and vibration isolation strategies  

---

## 🧰 Tools and Technologies
- MATLAB (Live Scripts)  
- Time-domain signal processing  
- Statistical performance analysis  
- Engineering data visualization  

---

## 📁 Repository Structure
# MATLAB-Project-1-Suspension-Ride-Quality-Analysis
An engineering analysis of suspension ride quality using experimental data, conducted in MATLAB and extended beyond coursework requirements for deeper technical insight.
