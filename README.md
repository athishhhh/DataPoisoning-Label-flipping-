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

## 🏗 Model Architecture  

### **End-to-End Workflow for Fraud Detection Defense System**  
![Model Architecture](results/model_architecture.png)

```plaintext
                   ┌───────────────────────────────┐
                   │  🟪 Input: Credit Card Dataset │
                   └───────────────┬───────────────┘
                                   ↓
          ┌─────────────────────────────────────────┐
          │  🟥 Step 1: Label Flipping Attack (30%) │
          │  - Fraud labels changed to non-fraud   │
          └───────────────┬────────────────────────┘
                          ↓
     ┌─────────────────────────────────────────────┐
     │  🔷 Step 2: Detection (Isolation Forest)    │
     │  - Flags suspicious fraud transactions      │
     └───────────────┬────────────────────────────┘
                     ↓
      ┌───────────────────────────────────────────┐
      │  🟥 Step 3: Correction (Re-labeling)       │
      │  - Uses secondary model to fix labels    │
      └───────────────┬──────────────────────────┘
                      ↓
  ┌───────────────────────────────────────────────┐
  │  🟩 Step 4: Final Fraud Detection Model       │
  │  - Train model on cleaned data               │
  │  - Improve fraud detection accuracy          │
  └───────────────┬──────────────────────────────┘
                  ↓
  ┌───────────────────────────────────────────────┐
  │  🟪 Step 5: Evaluate Model Performance        │
  │  - Compare accuracy before & after defense   │
  │  - Fraud detection rate improvement          │
  └──────────────────────────────────────────────┘

