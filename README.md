# DataPoisoning-Label-flipping-
Detecting and preventing data poisoning in fraud detection using Label Flipping Attack defense.

#  Fraud Detection Vulnerabilities

->Data Poisoning Threat
Fraud detection models are exposed to data poisoning, leading to misclassification.
->Misclassification Impact
Increased fraudulent transactions are incorrectly classified as legitimate, worsening fraud cases.
->Label Flipping Attack
Implementing a label flipping attack on the fraud detection dataset to evaluate vulnerabilities.
->Detection Mechanism Development
Developing mechanisms to detect and identify poisoned data within the dataset.


#  Fraud Detection & Data Poisoning Defense  

**Detecting & Preventing Label Flipping Attack in Credit Card Fraud Detection**  

---

##  Project Overview  
Machine learning models, especially in **fraud detection**, are vulnerable to **data poisoning attacks**. This project focuses on **Label Flipping Attack**, where **fraudulent transactions are incorrectly labeled as non-fraudulent**, reducing the model’s ability to detect fraud.  

** Objectives:  
- Simulate a **Label Flipping Attack** in a fraud detection dataset.  
- Implement **anomaly detection (Isolation Forest)** to flag poisoned samples.  
- Develop a **correction mechanism** to restore mislabeled fraud cases.  
- Train a **robust fraud detection model** and compare its performance **before and after defense**.  

---

## Model Architecture  

### **End-to-End Workflow for Fraud Detection Defense System**  
![Model Architecture](Control-V.png)


##Label Flipping Attack Implementation
A Label Flipping Attack is a type of data poisoning attack where the attacker intentionally mislabels a subset of the training data to degrade the model’s performance.

 How the Attack Works
1️. Select a percentage of fraud samples (e.g., 30%)
2️. Flip their labels from fraud (1) to non-fraud (0)
3️. Train the fraud detection model on poisoned data
4️. Evaluate the model and observe the performance drop

# Expected Impact of the Attack
The fraud detection rate decreases because the model learns incorrect patterns.

The number of missed fraud cases (False Negatives) increases, making fraudsters harder to catch.

The accuracy might remain high due to data imbalance, but fraud detection effectiveness suffers significantly.

 Before vs. After Poisoning (Expected Results)
![Poisoning table](image.png)
![before](afterpoisoingconfusionmat.png)
![confafter](afterpoisoingconfusionmat.png)



