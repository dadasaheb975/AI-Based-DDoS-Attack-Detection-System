# DDoS-Detection-using-ML
DDoS Detection using various ML models(Decision tree, Random Forest, Support Vector Machine(SVM), KNN, Neural Network, Gradient Boosting tree)

To use this dataset you might need an account of Kaggle or you can make changes in code for accessing dataset that is availabe in Datasets folder. In order to access dataset from Kaggle you might need to upload your API token(kaggle.json). In order to get your API token you can go to the Account tab of your user profile and select Create API Token.
AI-Based DDoS Attack Detection System


1️) What is a DDoS Attack?

A Distributed Denial of Service (DDoS) attack occurs when multiple compromised systems (botnets) simultaneously send a huge amount of traffic to a target server or network.

Effects of DDoS attack:

Server becomes slow or unavailable

Legitimate users cannot access services

Website or network goes down

2️) Why Traditional Detection Methods Fail

Traditional detection techniques include:

Signature-based detection

Rule-based systems

Threshold-based methods

Limitations:

Cannot detect new or unknown attacks

High false positive rate

Not suitable for large-scale traffic

 Hence, AI and Machine Learning are used.

3️) What is an AI-Based DDoS Detection System?

An AI-Based DDoS Detection System analyzes network traffic using Machine Learning models to classify traffic as:

Normal traffic

DDoS attack traffic

It can detect attacks in real time and adapt to new attack patterns.

* System Architecture / Workflow
Network Traffic
      ↓
Data Collection
      ↓
Feature Extraction
      ↓
Machine Learning Model
      ↓
Attack Detection
      ↓
Alert & Mitigation

4️) System Modules
🔹 1. Data Collection

Traffic data is captured from the network, such as:

Source IP address

Destination IP address

Packet size

Protocol (TCP, UDP, ICMP)

Packet rate and flow duration

Common tools & datasets:

Wireshark

CICIDS2017 Dataset

NSL-KDD Dataset

🔹 2. Feature Extraction

Raw network data cannot be used directly for ML models.

Important features:

Packets per second

Bytes per flow

Flow duration

SYN packet count

IP address entropy

Feature extraction improves detection accuracy.

🔹 3. Machine Learning Models Used

Commonly used algorithms:

Algorithm	Purpose
Random Forest	High accuracy, robust
Decision Tree	Simple and interpretable
Support Vector Machine (SVM)	Binary classification
K-Nearest Neighbors (KNN)	Pattern similarity
Neural Networks	Complex attack detection

* Random Forest is most preferred because:

Reduces overfitting

Combines multiple decision trees

Provides high accuracy

🔹 4. Training Phase

Dataset is divided into training and testing sets

Model learns patterns of normal and attack traffic

🔹 5. Detection Phase

Live network traffic is fed into the trained model

Model predicts:

Normal Traffic

DDoS Attack

🔹 6. Alert and Mitigation

When an attack is detected:

Alert is sent to the administrator

Malicious IP addresses are blocked

Traffic rate limiting is applied

Firewall rules are updated

5️) Why AI-Based Detection is Better
Traditional Methods	AI-Based Methods
Static rules	Adaptive learning
Low detection accuracy	High accuracy
Detects known attacks only	Detects unknown attacks
Manual updates	Automatic model updates
6️) Advantages

✅ Real-time attack detection
✅ High accuracy and low false positives
✅ Scalable for large networks
✅ Automatically adapts to new attacks

7️) Applications

Cloud computing environments

Banking and financial systems

E-commerce platforms

Government and defense networks

IoT and smart networks

8️) Tools & Technologies (Example)

Programming Language: Python

Libraries: Scikit-learn, Pandas, NumPy

Dataset: CICIDS2017

Operating System: Linux / Kali Linux

9️) Future Enhancements

Deep Learning models (CNN, LSTM)

Real-time deployment using cloud platforms

Automatic mitigation using Software Defined Networking (SDN)
# Datasets
1. Dataset taken from Kaggle by YASHWANTH REDDY KUMBAM (https://www.kaggle.com/datasets/yashwanthkumbam/apaddos-dataset)
2. Dataset taken from Kaggle by PREETI (https://www.kaggle.com/datasets/preeti5607/ddos-attack-prevention)
