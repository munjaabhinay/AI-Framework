**AI-Driven Intrusion Detection: A Federated Learning Dataset for Cloud and Edge Security**

**Overview**

This project presents a Machine Learning-based Intrusion Detection System (IDS) designed to identify anomalous IoT network traffic associated with Mirai and BASHLITE botnet attacks.

With the rapid expansion of IoT ecosystems, network infrastructures have become increasingly vulnerable to large-scale Distributed Denial of Service (DDoS) and botnet-driven attacks. Traditional rule-based detection systems struggle to adapt to evolving attack patterns. This framework leverages supervised machine learning models to improve detection accuracy, scalability, and real-time monitoring capabilities.

**Problem Statement**

    IoT devices generate massive volumes of network traffic, making it difficult to distinguish legitimate behavior from malicious activity. Botnets such as Mirai and BASHLITE exploit insecure IoT devices to launch coordinated cyber-attacks.

**The objective of this project is to design and implement a scalable AI-driven framework capable of:**

    Detecting anomalous network traffic
    
    Classifying traffic into Normal, BASHLITE, and Mirai categories
    
    Improving detection accuracy while minimizing false positives
    
    Supporting deployment in real-time IoT environments
    
    Technologies Used
    
    Python
    
    Pandas & NumPy
    
    Scikit-learn
    
    Matplotlib & Seaborn
    
    SMOTE (Imbalanced Data Handling)
    
    Joblib (Model Persistence)
    
    Dataset
    
    Dataset Used: BoTNeTIoT-L01-v2

**The dataset contains real-world IoT network traffic features including:**

    Source and Destination IP
    
    Source and Destination Ports
    
    Protocol Type
    
    Flow Duration
    
    Packet Counts (Forward & Backward)
    
    Traffic Statistics
    
    Attack Label (Normal / BASHLITE / Mirai)

**Target Encoding:**

    0 → Normal
    
    1 → BASHLITE
    
    2 → Mirai

**Methodology**

**1. Data Preprocessing**

    Removal of irrelevant attributes
    
    Handling of missing values
    
    Label encoding of categorical variables
    
    Correlation analysis using heatmap
    
    Class imbalance handling using SMOTE
    
    Train-test split (70:30)

**2. Model Development**

    Two classification algorithms were implemented:
    
    Bernoulli Naive Bayes
    
    Random Forest Classifier

**3. Model Evaluation**

    Performance metrics used:
    
    Accuracy
    
    Precision
    
    Recall
    
    F1-Score

Confusion Matrix

**4. Model Persistence**

    Trained models were saved using Joblib for deployment and reuse.

**Results**

    The Random Forest Classifier demonstrated superior performance compared to Bernoulli Naive Bayes in detecting IoT botnet attacks.

**Key outcomes:**

    Improved classification accuracy
    
    Better handling of feature correlations
    
    Reduced false positives
    
    Strong generalization on unseen test data

**The model successfully classified network traffic into:**

    Normal
    
    BASHLITE
    
    Mirai
