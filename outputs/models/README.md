# Trained Models Directory

## Purpose
This directory contains trained clustering models, model artifacts, and model metadata for deployment and future use.

## Model Files

### 1. **Trained Clustering Models**
- `kmeans_model.pkl`: Best performing K-Means clustering model
- `hierarchical_model.pkl`: Hierarchical clustering model
- `dbscan_model.pkl`: DBSCAN clustering model
- `ensemble_model.pkl`: Combined model approach (if applicable)

### 2. **Model Metadata**
- `model_performance_metrics.json`: Performance scores and validation metrics
- `model_hyperparameters.json`: Optimal hyperparameters for each model
- `model_training_log.txt`: Training history and configuration
- `model_version_info.md`: Version details and training date

### 3. **Model Artifacts**
- `feature_scaler.pkl`: StandardScaler used for feature normalization
- `pca_transformer.pkl`: PCA transformation if dimensionality reduction applied
- `feature_selector.pkl`: Feature selection model (if applicable)
- `model_pipeline.pkl`: Complete preprocessing and modeling pipeline

### 4. **Model Evaluation**
- `model_comparison_results.json`: Detailed comparison across all models
- `cross_validation_scores.json`: Cross-validation performance metrics
- `stability_analysis_results.json`: Model stability across multiple runs
- `business_metrics_evaluation.json`: Business-relevant performance indicators

## File Formats
- **Pickle (.pkl)**: Serialized Python objects
- **JSON**: Configuration and metadata
- **Markdown**: Documentation and notes
- **Text**: Logs and training history

## Model Information
- **Best Model**: K-Means clustering
- **Optimal Clusters**: 2
- **Performance**: High silhouette scores
- **Stability**: Consistent across multiple runs
- **Business Applicability**: High

## Usage
- Load models for prediction on new data
- Use for model comparison and analysis
- Reference for hyperparameter tuning
- Deployment in production systems

## Model Loading Example
```python
import pickle

# Load the best model
with open('kmeans_model.pkl', 'rb') as f:
    model = pickle.load(f)

# Load the scaler
with open('feature_scaler.pkl', 'rb') as f:
    scaler = pickle.load(f)
```
