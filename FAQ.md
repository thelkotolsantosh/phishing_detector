# FAQ — phishing_detector

## 1. What is this phishing_detector project about?

This project is an ML-based phishing website detection system that classifies URLs as:

* Legitimate
* Phishing

The system uses URL-derived lexical and structural features without relying on external APIs or online threat intelligence services.

---

## 2. What problem does this project solve?

Phishing websites imitate legitimate websites to steal:

* Passwords
* Banking details
* Credentials
* Personal information

This project helps automatically identify suspicious URLs using machine learning techniques.

---

## 3. What technologies are used in this project?

### Core Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* YAML

### Machine Learning & Analysis

* Random Forest Classifier
* Feature Engineering
* Exploratory Data Analysis (EDA)

### Development Tools

* Jupyter Notebook
* Logging
* Pickle Serialization

---

## 4. What machine learning model is used?

The project primarily uses a:

* Random Forest Classifier

for phishing URL classification.

---

## 5. Why was Random Forest chosen specifically?

Random Forest was selected because it:

* Handles tabular URL features efficiently
* Reduces overfitting
* Performs well on classification tasks
* Handles nonlinear feature relationships
* Provides feature importance rankings

It is widely used in phishing detection research and security analytics.

---

## 6. What features are extracted from the URLs?

Typical extracted features include:

* URL length
* Number of dots (`.`)
* Number of special characters
* Presence of IP addresses
* HTTPS usage
* Suspicious keywords
* Subdomain count
* URL shortening service usage

These structural patterns help detect phishing behavior.

---

## 7. Does this project require internet access for detection?

No.

The model uses:

* URL lexical analysis
* Structural feature extraction

without depending on external APIs, WHOIS lookups, or online reputation services.

---

## 8. What type of dataset is used?

The project contains a labeled phishing dataset (~2000 rows) consisting of:

* Legitimate URLs
* Phishing URLs
* Extracted feature vectors
* Binary classification labels

---

## 9. What is the purpose of feature engineering in this project?

Feature engineering converts raw URLs into numerical patterns that machine learning models can understand.

Without feature engineering:

* ML models cannot effectively learn phishing characteristics.

---

## 10. What is EDA in this project?

EDA stands for:

* Exploratory Data Analysis

The notebook includes:

* Class distribution plots
* Correlation heatmaps
* Feature distribution charts
* ROC curves
* Confusion matrices

to analyze dataset behavior and model performance.

---

## 11. What evaluation metrics are used?

The project uses common ML evaluation metrics such as:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC
* Confusion Matrix

These metrics help measure phishing detection quality and classification performance.

---

## 12. Why is phishing detection important in cybersecurity?

Phishing attacks are among the most common cybersecurity threats and are responsible for:

* Credential theft
* Financial fraud
* Identity theft
* Malware and ransomware delivery

ML-based phishing detection helps automate threat detection and defensive security analysis.

---

## 13. Does the project support batch prediction?

Yes.

The project supports:

* Single URL prediction
* Batch inference

through the prediction pipeline.

---

## 14. What is stored in the `models/` folder?

The `models/` folder contains:

* Trained Random Forest model
* Scaler objects
* Serialized ML artifacts

stored using Pickle serialization.

---

## 15. What is the purpose of `config.yaml`?

The `config.yaml` file stores:

* Hyperparameters
* File paths
* Training settings
* Preprocessing configurations

This makes the ML pipeline easier to manage and scale.

---

## 16. Can this project be converted into a web application?

Yes.

Possible upgrades include:

* Flask API
* FastAPI backend
* Streamlit dashboard
* Browser extension
* Chrome phishing detector
* Real-time URL scanner

---

## 17. Can deep learning models be added later?

Yes.

Possible future models include:

* LSTM
* Transformer models
* BERT-based URL analysis
* Autoencoders
* Graph Neural Networks (GNNs)

for advanced phishing detection systems.

---

## 18. Is this project useful for cybersecurity portfolios?

Absolutely.

This project demonstrates:

* Cybersecurity knowledge
* ML pipeline engineering
* Feature engineering
* Security analytics
* EDA skills
* Production-style project organization

making it valuable for cybersecurity and data science portfolios.

---

## 19. What future features can improve this project?

Possible roadmap improvements:

* Real-time URL scanning
* WHOIS lookup integration
* Threat intelligence APIs
* Browser plugin
* URL screenshot analysis
* DNS reputation scoring
* Phishing email analysis
* Deep learning ensemble models

---

## 20. How do I run this project on Windows and Linux?

### 🪟 Windows Setup

#### Step 1 — Clone Repository

```bash
git clone https://github.com/thelkotolsantosh/phishing_detector-.git
cd phishing_detector-
```

#### Step 2 — Create Virtual Environment

```bash
python -m venv venv
```

#### Step 3 — Activate Environment

```bash
venv\Scripts\activate
```

#### Step 4 — Install Dependencies

```bash
pip install -r requirements.txt
```

#### Step 5 — Run the Project

```bash
python main.py
```

---

### 🐧 Linux Setup

#### Step 1 — Clone Repository

```bash
git clone https://github.com/thelkotolsantosh/phishing_detector-.git
cd phishing_detector-
```

#### Step 2 — Create Virtual Environment

```bash
python3 -m venv venv
```

#### Step 3 — Activate Environment

```bash
source venv/bin/activate
```

#### Step 4 — Install Dependencies

```bash
pip install -r requirements.txt
```

#### Step 5 — Run the Project

```bash
python3 main.py
```

---

## 21. Is this project defensive or offensive cybersecurity?

This project primarily belongs to:

* Defensive Cybersecurity (Blue Team)

It focuses on:

* Phishing prevention
* URL threat detection
* ML-based security analytics
* Educational cybersecurity research

---

## 22. What makes this project different from beginner phishing projects?

This repository includes:

* Structured ML pipeline
* Modular architecture
* Centralized logging
* Configuration management
* EDA workflows
* CLI inference support
* Production-style project organization

These features make it more professional than notebook-only beginner projects.
