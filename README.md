# 📊 README.md

# TAYLOR FRY MARATHON PREDICTOR
**MACHINE LEARNING • INJURY PREDICTION • MEDICAL PLANNING • XGBOOST**

![Model Accuracy](https://img.shields.io/badge/Model%20Accuracy-84.8%25-green) ![Data Science](https://img.shields.io/badge/Data%20Science-XGBoost-orange) ![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📅 Project Timeline
- **Development Period**: July 2025
- **Target Event**: 2025 Marathon Season
- **Model Training**: Historical Marathon Dataset (2020-2024)

## 📋 Background

### 🎯 Rationale
Marathon events require significant medical resource planning to ensure runner safety. Traditional approaches rely on historical averages and rough estimates, leading to either over-provisioning (costly) or under-provisioning (dangerous) of medical staff and equipment.

### 🚀 Getting Started
This project leverages machine learning to predict:
1. **Medical Attention Risk**: Which runners are likely to need medical attention
2. **Injury Location**: At what kilometer mark injuries are most likely to occur

### 📦 Data Sources
- Historical marathon dataset (2020-2024)
- Runner demographics and training history
- Event conditions (weather, course elevation, facilities)
- Medical intervention records

### 🔧 Technical Interface
- **Primary Model**: XGBoost Classifier & Regressor
- **Programming Language**: Python
- **Key Libraries**: XGBoost, Pandas, Scikit-learn
- **Input Format**: CSV files with runner and event data
- **Output Format**: Prediction CSV files for race organizers

## 📋 Task Breakdown

### 🧪 Implementation

#### 📊 Model Development
- **Medical Attention Prediction**
  - ✅ Binary classification using XGBoost
  - ✅ Feature engineering (demographics + event conditions)
  - ✅ Threshold optimization for precision/recall balance
  - ✅ Cross-validation and hyperparameter tuning

- **Injury Location Prediction**
  - ✅ Regression model to predict kilometer of medical intervention
  - ✅ Multi-feature approach combining runner and environmental factors
  - ✅ Residual analysis and model validation

#### 🎯 Model Performance
- **Medical Attention Model**:
  - Best Accuracy: **84.8%** (at threshold 0.7455)
  - Best F1-Score: **0.4208** (at threshold 0.5500)
  - Optimized for minimizing false negatives (missed injuries)

- **Injury Location Model**:
  - Mean Absolute Error: **7.85 km**
  - Mean Squared Error: **90.31 km²**
  - Residual analysis shows balanced distribution

#### 🔍 Feature Analysis
**Key Predictive Features**:
- Runner demographics (age, gender, BMI)
- Training history (weekly km, marathon experience)
- Personal best times and injury history
- Event conditions (temperature, humidity, elevation)
- Course logistics (hydration stations, crowding density)

### 📈 Testing
#### 💡 Model Validation
- Cross-validation on historical data (2020-2024)
- Threshold optimization for operational requirements
- Feature importance analysis for interpretability

#### 🔧 Implementation Details
- **XG-Boost.ipynb**: Main classification model for medical attention prediction
- **injury_loc.ipynb**: Regression model for injury location prediction
- Automated preprocessing and feature engineering pipelines

### 🏃‍♂️ Deployment Pipeline
- Data preprocessing and cleaning
- Model training with hyperparameter optimization
- Prediction generation for 2025 marathon cohort
- Output generation: `Medical_attn_preds.csv` and `injury_loc.csv`

### 📊 API Integration
- Batch prediction capabilities
- Feature importance reporting
- Model performance metrics
- Threshold sensitivity analysis

## 📤 Submission Deliverables

### 📁 Output Files
- **Medical_attn_preds.csv**: Binary predictions for medical attention needs
- **injury_loc.csv**: Predicted kilometer locations for potential injuries
- **Feature importance reports**: Top predictive factors analysis

### 📋 Model Documentation
- Complete Jupyter notebooks with methodology
- Performance metrics and validation results
- Feature engineering documentation
- Deployment guidelines for race organizers

## 📚 Additional Information

### 🔧 Technical Requirements
```python
# Core Dependencies
- xgboost>=1.6.0
- pandas>=1.3.0
- scikit-learn>=1.0.0
- numpy>=1.21.0
- matplotlib>=3.4.0
