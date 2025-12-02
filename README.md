# 🍷 Wine Dataset Logging Lab

**Student:** Lochan | **Course:** IE7305 MLOps | **Institution:** Northeastern University

## 📋 Overview

Python logging implementation with Wine dataset ML pipeline using RandomForestClassifier. Demonstrates all lab logging concepts in a production-ready workflow.

## 📊 Comparison Table

| Feature | Professor's Lab | My Lab |
|---------|----------------|--------|
| **Dataset** | None (simple print logs) | Wine dataset (`sklearn`) |
| **Model** | None | RandomForestClassifier |
| **Pipeline Logging** | ❌ | ✅ Full ML pipeline |
| **Exception Logging** | Basic | ✅ Multiple exceptions + traceback |
| **File Logging** | ❌ | ✅ Saves `.log` files |
| **Custom Logger** | Minimal | ✅ Named loggers (`data_processing`, `model_training`, `model_evaluation`, `multi_handler`) |
| **Handlers** | None | ✅ StreamHandler + FileHandler |

## 🗂️ Project Structure

```
├── wine_logging_demo.py       # Main script (11 sections)
├── wine_analysis.log          # File logging output
├── wine_multi_handler.log     # Multi-handler output
└── README.md
```

## 🚀 Features Implemented

1. ✅ Basic logging configuration with `basicConfig()`
2. ✅ All 5 log levels (DEBUG, INFO, WARNING, ERROR, CRITICAL)
3. ✅ Custom loggers for different modules
4. ✅ Exception logging with automatic tracebacks
5. ✅ File-based logging
6. ✅ Runtime log level control
7. ✅ Multiple handlers (Stream + File)
8. ✅ Real ML pipeline application

## 📈 ML Pipeline Results

- **Dataset:** 178 samples, 13 features, 3 classes
- **Model:** RandomForestClassifier
- **Accuracy:** 100%
- **Split:** 80-20 train-test with StandardScaler

## 🛠️ Quick Start

```bash
pip install numpy pandas scikit-learn
python wine_logging_demo.py
```

## 📝 Script Sections

1. Basic Logging Configuration
2. Logging Messages at All Levels
3. Custom Loggers
4. Wine Dataset Loading
5. Data Preprocessing
6. Exception Logging (3 types)
7. Model Training
8. Model Evaluation
9. File Logging
10. Log Level Control
11. Multiple Handlers

## 📤 Sample Output

```
2025-12-02 00:09:53,357 - data_processing - INFO - Dataset loaded: 178 samples, 13 features
2025-12-02 00:09:53,361 - data_processing - INFO - Train: 142, Test: 36
2025-12-02 00:09:53,474 - model_training - INFO - Model training completed
2025-12-02 00:09:53,478 - model_evaluation - INFO - Model Accuracy: 1.0000
```

## 🎯 Key Takeaways

- Modular logging with named loggers for each pipeline component
- Exception handling with full tracebacks
- Multiple output destinations (console + file)
- Production-ready logging practices for MLOps

---

**Course:** IE7305 MLOps | **Date:** December 2, 2025
