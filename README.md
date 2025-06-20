# 🛡️ Cybersecurity Project: Suspicious Web Threat Interactions

# 🌐 Project Overview

With the surge in cyber threats targeting cloud infrastructure, this project focuses on detecting suspicious web interactions using logs collected from AWS CloudWatch. By analyzing traffic features such as IP addresses, timestamps, byte flow, and detection types, the project aims to uncover malicious behavior and support early threat detection.

# 🎯 Objective

To detect and classify suspicious web activities using data analysis, anomaly detection, and machine learning techniques, and to provide actionable insights through data visualization and pattern recognition.

# 🛠️ Steps Involved

Data Exploration & Cleaning

Feature Engineering

Exploratory Data Analysis (EDA)

Anomaly Detection

Machine Learning Model Evaluation

Data Visualization

# 📁 Dataset

File: CloudWatch_Traffic_Web_Attack.csv

Source: AWS CloudWatch Logs

Key Fields: source_ip, destination_ip, bytes_in, bytes_out, timestamp, country, detection_type, is_suspicious

# 📊 Key Analyses & Visualizations

Detection types across countries (Treemaps, Bar Charts)

Time-series trends of traffic

Correlation heatmap of features

Byte-in vs Byte-out scatter plots

Network graph of source and destination IP clusters

# 🤖 Models & Techniques

Anomaly Detection: Isolation Forest flagged ~5% of traffic as abnormal

Classification Models: Random Forest, Multilayer Perceptron (MLP)

Note: Classification was skipped due to class imbalance (only one label: is_suspicious = 1)

Visual Pattern Recognition: Network graphs for traffic clusters

# 💡 Insights

A few countries were consistently associated with abnormal traffic.

Strong correlation between bytes_in and bytes_out—typical of bidirectional session flow.

Isolation Forest effectively identified anomalies despite label imbalance.

Dense IP clusters in network graphs revealed frequent threat origins or communication hubs.

Class imbalance in the dataset limited the usefulness of supervised classification.

# 🧠 Technologies Used

Python (Pandas, Seaborn, Scikit-learn, Matplotlib, NetworkX)

Jupyter Notebook



