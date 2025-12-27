# SympTrack AI 🏥🤖

A comprehensive multi-disease prediction system powered by Machine Learning, providing accurate health assessments across 5 major disease categories through an intuitive Streamlit interface.

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-red.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0.2-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

## 🎯 Overview

SympTrack AI is an intelligent disease prediction system that leverages machine learning algorithms to provide accurate health risk assessments. This system achieves 85-96% accuracy across multiple disease categories, helping users make informed health decisions through an easy-to-use web interface.

### 🔗 Repository
[https://github.com/incursio-xd/AICTE-INTERNSHIP](https://github.com/incursio-xd/AICTE-INTERNSHIP)

## 🏥 Supported Diseases

| Disease | Algorithm | Accuracy | Features |
|---------|-----------|----------|----------|
| 🩺 **Diabetes** | Logistic Regression | ~85% | 8 parameters |
| ❤️ **Heart Disease** | Logistic Regression | ~82% | 13 parameters |
| 🧠 **Parkinson's Disease** | Support Vector Machine (SVM) | ~87% | 22 parameters |
| 🫁 **Lung Cancer** | Logistic Regression | ~94% | 15 parameters |
| 🦋 **Hypothyroid** | Logistic Regression | ~96% | 7 parameters |

## ✨ Key Features

- 🔬 **Multi-Model Architecture**: Specialized ML models for each disease category
- 📊 **High Accuracy**: 82-96% prediction accuracy across all categories
- 🎨 **Interactive UI**: User-friendly Streamlit interface with real-time predictions
- ⚡ **Fast Assessment**: Get predictions instantly
- 💡 **Input Tooltips**: Helpful guidance for each medical parameter
- 📈 **Comprehensive Analysis**: Detailed Jupyter notebooks for model training
- 🎯 **Color-Coded Results**: Easy-to-understand visual feedback
- 🔒 **Privacy Focused**: No data storage, all predictions in-memory

## 🛠️ Tech Stack

### Frontend
- **Streamlit** - Interactive web framework
- **streamlit-option-menu** - Enhanced navigation
- **Custom CSS** - Medical-themed styling

### Backend & ML
- **Python 3.9+** - Core programming language
- **scikit-learn 1.0.2** - Machine learning framework
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computations
- **matplotlib** - Data visualization
- **seaborn** - Statistical visualization
- **statsmodels** - Statistical modeling

### Machine Learning Models
- **Logistic Regression** - Diabetes, Heart Disease, Lung Cancer, Thyroid
- **Support Vector Machine (SVM)** - Parkinson's Disease

## 📋 Prerequisites

```bash
Python 3.9 or higher
pip (Python package manager)
Git
```

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/incursio-xd/AICTE-INTERNSHIP.git
cd AICTE-INTERNSHIP
```

### 2️⃣ Create Virtual Environment
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Verify Project Structure
```
AICTE-INTERNSHIP/
├── Models/              # Pre-trained models
├── Datasets/            # Training datasets
├── app.py              # Main application
└── requirements.txt    # Dependencies
```

### 5️⃣ Run the Application
```bash
streamlit run app.py
```

### 6️⃣ Access the Application
```
http://localhost:8501
```

## 💻 Usage Guide

### Quick Start

1. **Launch Application**
   ```bash
   streamlit run app.py
   ```

2. **Select Disease** - Choose from dropdown menu

3. **Enter Parameters** - Fill in medical data

4. **Get Results** - Click test button for instant prediction

## 📊 Model Information

### 1. Diabetes Prediction
**Algorithm**: Logistic Regression  
**Training Accuracy**: 85.13%  
**Test Accuracy**: 81.97%

**Input Parameters (8)**:
- Number of Pregnancies
- Glucose Level
- Blood Pressure
- Skin Thickness
- Insulin Level
- BMI (Body Mass Index)
- Diabetes Pedigree Function
- Age

**Dataset**: 303 samples (from diabetes_data.csv)

---

### 2. Heart Disease Prediction
**Algorithm**: Logistic Regression  
**Training Accuracy**: 85.12%  
**Test Accuracy**: 81.97%

**Input Parameters (13)**:
- Age
- Sex (1=Male, 0=Female)
- Chest Pain Type (0-3)
- Resting Blood Pressure
- Serum Cholesterol (mg/dl)
- Fasting Blood Sugar (>120 mg/dl)
- Resting ECG Results (0-2)
- Maximum Heart Rate
- Exercise Induced Angina (1=Yes, 0=No)
- ST Depression (Oldpeak)
- Slope of Peak Exercise ST
- Number of Major Vessels (0-3)
- Thalassemia (0-2)

**Dataset**: 303 samples

---

### 3. Parkinson's Disease Prediction
**Algorithm**: Support Vector Machine (Linear Kernel)  
**Training Accuracy**: 87.18%  
**Test Accuracy**: 87.18%

**Input Parameters (22)**: Voice measurement features
- MDVP:Fo(Hz), Fhi(Hz), Flo(Hz)
- MDVP:Jitter(%), Jitter(Abs), RAP, PPQ
- Jitter:DDP
- MDVP:Shimmer, Shimmer(dB)
- Shimmer:APQ3, APQ5, APQ, DDA
- NHR, HNR, RPDE, DFA
- Spread1, Spread2, D2, PPE

**Dataset**: 195 samples

---

### 4. Lung Cancer Prediction
**Algorithm**: Logistic Regression  
**Training Accuracy**: 93.52%  
**Test Accuracy**: 93.52%

**Input Parameters (15)**:
- Gender (1=Male, 0=Female)
- Age
- Smoking (1=Yes, 0=No)
- Yellow Fingers (1=Yes, 0=No)
- Anxiety (1=Yes, 0=No)
- Peer Pressure (1=Yes, 0=No)
- Chronic Disease (1=Yes, 0=No)
- Fatigue (1=Yes, 0=No)
- Allergy (1=Yes, 0=No)
- Wheezing (1=Yes, 0=No)
- Alcohol Consumption (1=Yes, 0=No)
- Coughing (1=Yes, 0=No)
- Shortness of Breath (1=Yes, 0=No)
- Swallowing Difficulty (1=Yes, 0=No)
- Chest Pain (1=Yes, 0=No)

**Dataset**: 309 samples

---

### 5. Hypothyroid Prediction
**Algorithm**: Logistic Regression  
**Training Accuracy**: 95.62%  
**Test Accuracy**: 95.63%

**Input Parameters (7)**:
- Age
- Sex (1=Male, 0=Female)
- On Thyroxine (1=Yes, 0=No)
- TSH Level
- T3 Measured (1=Yes, 0=No)
- T3 Level
- TT4 Level

**Dataset**: 3,772 samples

## 📁 Project Structure

```
AICTE-INTERNSHIP/
│
├── .ipynb_checkpoints/              # Jupyter checkpoints
│
├── Datasets/                        # Training datasets
│   ├── diabetes_data.csv
│   ├── heart_disease_data.csv
│   ├── hypothyroid.csv
│   ├── parkinsons_data.csv
│   ├── prepocessed_hypothyroid.csv
│   ├── prepocessed_lungs_data.csv
│   └── survey_lung_cancer.csv
│
├── Models/                          # Trained ML models
│   ├── diabetes_model.sav
│   ├── heart_disease_model.sav
│   ├── lungs_disease_model.sav
│   ├── parkinsons_model.sav
│   └── Thyroid_model.sav
│
├── project2/                        # Additional resources
│
├── Notebooks/                       # Training notebooks
│   ├── Heart_Disease_Prediction.ipynb
│   ├── Lung_Cancer.ipynb
│   ├── Parkinson's_Disease_Detection.ipynb
│   └── Thyroid.ipynb
│
├── app.py                          # Main Streamlit app
├── requirements.txt                # Dependencies
└── README.md                       # Documentation
```

## 📦 Dependencies

```txt
streamlit==1.28.0
scikit-learn==1.0.2
pandas==1.5.3
numpy==1.23.5
matplotlib==3.7.1
seaborn==0.12.2
statsmodels==0.14.0
streamlit-option-menu==0.3.6
```

**Install all dependencies:**
```bash
pip install -r requirements.txt
```

## 🔧 Model Training Process

### Data Preprocessing
1. **Missing Value Handling**
   - SimpleImputer for numerical features
   - Mean/median imputation strategies

2. **Feature Encoding**
   - LabelEncoder for categorical variables
   - Binary encoding for Yes/No fields

3. **Data Splitting**
   - 80% Training / 20% Testing
   - Stratified split for balanced classes

### Model Training
1. **Algorithm Selection**
   - Logistic Regression (4 models)
   - SVM with linear kernel (1 model)

2. **Model Evaluation**
   - Accuracy score
   - Training vs Testing performance
   - No overfitting observed

3. **Model Serialization**
   - Saved using pickle (.sav format)
   - Ready for production deployment

## 🎨 UI Features

- 🎭 **Medical Theme**: Professional healthcare design
- 📱 **Responsive Layout**: Works on all devices
- 🔽 **Dropdown Navigation**: Easy disease selection
- 💡 **Input Tooltips**: Contextual help for parameters
- ✅ **Input Validation**: Number inputs with step controls
- 🎨 **Custom Styling**: Dark theme with medical background
- 🎯 **Color-Coded Results**: 
  - ✅ Green for negative (healthy)
  - ⚠️ Red for positive (disease detected)

## 📈 Performance Metrics

| Metric | Value |
|--------|-------|
| Average Prediction Time | < 1 second |
| Overall Accuracy Range | 82-96% |
| Models Deployed | 5 |
| Total Input Parameters | 65+ |
| Training Samples | 5,080 total |

## 🚧 Future Enhancements

- [ ] Add confidence scores with probabilities
- [ ] Implement more disease categories
- [ ] Deep learning models (CNN, LSTM)
- [ ] Mobile application (Flutter)
- [ ] PDF report generation
- [ ] Multi-language support
- [ ] User authentication system
- [ ] Medical history tracking
- [ ] Integration with wearable devices
- [ ] Real-time model retraining
- [ ] RESTful API development
- [ ] Doctor consultation integration

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. **Fork the Project**
   ```bash
   git clone https://github.com/incursio-xd/AICTE-INTERNSHIP.git
   ```

2. **Create Feature Branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit Changes**
   ```bash
   git commit -m 'Add AmazingFeature'
   ```

4. **Push to Branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Open Pull Request**

### Guidelines
- Follow PEP 8 style guide
- Write clear commit messages
- Add comments for complex logic
- Update documentation
- Test thoroughly before PR

## 📄 License

This project is licensed under the MIT License.

```
MIT License

Copyright (c) 2024 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

## 👨‍💻 Author

**Your Name**

- 🌐 GitHub: [@incursio-xd](https://github.com/incursio-xd)
- 💼 LinkedIn: [Your Profile](https://linkedin.com/in/incursio)
- 📧 Email: amannathjha14@gmail.com
- 🌍 Portfolio: [yourportfolio.com](https://incursio-xd.github.io/portfolio2/)

## 🙏 Acknowledgments

- **AICTE** for internship opportunity
- **Scikit-learn** community
- **Streamlit** framework team
- **UCI ML Repository** for datasets
- **Kaggle** community
- **Stack Overflow** community

## 📚 References

- [Scikit-learn Docs](https://scikit-learn.org/)
- [Streamlit Docs](https://docs.streamlit.io/)
- [UCI ML Repository](https://archive.ics.uci.edu/ml/)
- [Kaggle Datasets](https://www.kaggle.com/datasets)

## 📞 Support

- 📧 Email: your.email@example.com
- 🐛 Issues: [GitHub Issues](https://github.com/incursio-xd/AICTE-INTERNSHIP/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/incursio-xd/AICTE-INTERNSHIP/discussions)

## ⚠️ Medical Disclaimer

**IMPORTANT**: This application is for **educational purposes only**.

- ❌ NOT for clinical diagnosis
- ❌ NOT a substitute for professional medical advice
- ❌ NOT validated for medical use
- ✅ Educational demonstration only
- ✅ Always consult healthcare professionals

**Key Points:**
- Based on limited datasets
- Should not be used for self-diagnosis
- Does not replace clinical judgment
- Seek professional medical consultation

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/incursio-xd/AICTE-INTERNSHIP?style=social)
![GitHub forks](https://img.shields.io/github/forks/incursio-xd/AICTE-INTERNSHIP?style=social)

---

<div align="center">

**Made with ❤️ for healthcare innovation**

⭐ Star this repo if you find it helpful!

[Report Bug](https://github.com/incursio-xd/AICTE-INTERNSHIP/issues) · [Request Feature](https://github.com/incursio-xd/AICTE-INTERNSHIP/issues)

</div>

---

**Last Updated**: December 2024  
**Version**: 1.0.0  
**Status**: ✅ Active Development
