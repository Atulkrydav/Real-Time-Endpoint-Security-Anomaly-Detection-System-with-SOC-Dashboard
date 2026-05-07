# Real-Time-Endpoint-Security-Anomaly-Detection-System-with-SOC-Dashboard
A Cybersecurity monitoring system designed to detect abnormal endpoint behavior in real time using Machine Learning and visualize security events through an interactive SOC Dashboard.

This project focuses on proactive threat detection by identifying anomalies instead of relying only on traditional signature-based security methods. It helps security analysts monitor suspicious activities, detect potential attacks, and analyze endpoint telemetry efficiently.

# 📌 Features
🔍 Real-Time Endpoint Monitoring \
🤖 Machine Learning Based Anomaly Detection \
📊 Interactive SOC Dashboard \
🚨 Real-Time Alert Generation \
⚠️ Severity-Based Threat Classification \
🧪 Attack Simulation Support \
📈 Telemetry Data Visualization \
🧠 Deep Autoencoder Neural Network \
📂 CSV-Based Telemetry Processing 

# 🛡️ Problem Statement

Traditional security systems mainly depend on predefined signatures and rules to detect threats. These systems often fail against:

* Zero-Day Attacks 
* Unknown Malware 
* Insider Threats 
* Suspicious Behavioral Activities 

This project solves the problem by using Machine Learning to learn normal system behavior and identify deviations as anomalies.

# 🧠 Machine Learning Approach

The system uses a Deep Autoencoder Neural Network trained on normal endpoint activity data.

The model:

- Learns normal behavior patterns
- Reconstructs the input data
- Calculates reconstruction error
- Flags anomalies when the error exceeds a threshold
- Reconstruction Error Formula

$$
MSE = \frac{1}{n} \sum (x - x')^2
$$

Where:

- x = Original Input Data
- x' = Reconstructed Output
- n = Number of Data Points

The anomaly threshold is calculated using the 95th percentile of training error.

# 🏗️ System Architecture

``` text
+--------------------+
| Endpoint Telemetry |
+--------------------+
           |
           v
+--------------------+
| Data Preprocessing |
+--------------------+
           |
           v
+--------------------+
| Deep Autoencoder   |
| ML Model           |
+--------------------+
           |
           v
+--------------------+
| Reconstruction     |
| Error Calculation  |
+--------------------+
           |
           v
+--------------------+
| Anomaly Detection  |
+--------------------+
           |
           v
+--------------------+
| SOC Dashboard      |
+--------------------+
```
# 📊 SOC Dashboard Features

The Security Operations Center (SOC) Dashboard provides:

- Real-time anomaly monitoring
- Endpoint telemetry visualization
- Alert notifications
- Attack simulation controls
- Severity classification of threats
- Live security insights
