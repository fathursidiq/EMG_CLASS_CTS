# 🧠 Four-Class EMG Signal Classification Using Deep Learning

<p align="center">
  <strong>A Deep Learning-Based Framework for Neuromuscular Signal Analysis and Classification</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Biomedical%20Signal%20Processing-blue">
  <img src="https://img.shields.io/badge/Task-4--Class%20Classification-purple">
  <img src="https://img.shields.io/badge/Signal-EMG-orange">
  <img src="https://img.shields.io/badge/Framework-Deep%20Learning-green">
  <img src="https://img.shields.io/badge/Research-Experimental-informational">
</p>

---

## 1. Research Overview

This research investigates the application of deep learning techniques for automated classification of Electromyography (EMG) signals into four distinct diagnostic classes.

The study focuses on extracting discriminative information from neuromuscular electrical activity through multi-channel signal representation and comparative deep learning experiments.

The proposed framework incorporates:

- Multi-channel EMG signal representation.
- F-wave as the primary electrophysiological examination.
- Diagnosis-oriented Nerve Conduction Velocity (NCV) signal selection.
- Patient-level dataset partitioning.
- Comparative evaluation of five deep learning models.
- Quantitative performance assessment for four-class classification.

The primary objective is to investigate how deep learning models can identify different neuromuscular patterns from electrophysiological signals.

## 2. Research Dataset

The experimental dataset consists of EMG-related electrophysiological recordings collected from more than 100 patients.

| Dataset characteristic | Description |
|---|---|
| Data modality | Electrophysiological signals |
| Primary examination | F-wave |
| Additional examination | NCV |
| Classification task | Four classes |
| Signal representation | Five-channel representation |
| Patient population | More than 100 patients |
| Data normalization | Applied |
| Data splitting | Patient-level partitioning |

### Dataset Distribution

The dataset is divided using a patient-level partitioning strategy to minimize data leakage between training, validation, and testing subsets.

```mermaid
flowchart TD
    A["Original Patient Dataset<br/>100+ Patients"] --> B["Patient-Level Partitioning"]
    B --> C["Training Set<br/>70%"]
    B --> D["Validation Set<br/>15%"]
    B --> E["Testing Set<br/>15%"]
    C --> F["Model Training"]
    D --> G["Hyperparameter Monitoring"]
    E --> H["Final Model Evaluation"]
    style A fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style C fill:#dcfce7,stroke:#16a34a,color:#14532d
    style D fill:#fef3c7,stroke:#d97706,color:#78350f
    style E fill:#fce7f3,stroke:#db2777,color:#831843
```

*Note: The percentages refer to patient-level allocation, not individual signal segments.*

## 3. Electrophysiological Signal Processing

The research utilizes F-wave and NCV recordings as complementary sources of electrophysiological information.

### Signal Acquisition Strategy

```mermaid
flowchart TB
    A["Electrophysiological Examination"] --> B["F-wave Recording"]
    A --> C["NCV Recording"]
    B --> D["Primary Signal Input"]
    C --> E["Diagnosis-Oriented Selection"]
    E --> F["Right Median / Left Median"]
    E --> G["Right Ulnar / Left Ulnar"]
    D --> H["Multi-Channel Representation"]
    F --> H
    G --> H
    H --> I["Signal Normalization"]
    I --> J["Classification Dataset"]
```

### Signal Processing Pipeline

The preprocessing stage focuses on preparing the electrophysiological recordings for deep learning analysis.

```mermaid
flowchart LR
    A["Raw EMG Data"] --> B["Signal Organization"]
    B --> C["Channel Representation"]
    C --> D["Normalization"]
    D --> E["Dataset Partitioning"]
    E --> F["Deep Learning Input"]
```

The preprocessing strategy is designed to preserve the original electrophysiological information while ensuring consistent input representation for model training.

## 4. Proposed Deep Learning Framework

Five model configurations (M1–M5) are investigated to provide a comparative analysis of deep learning performance.

```mermaid
flowchart TB
    A["Multi-Channel EMG Input"] --> B["Input Preparation"]
    B --> C1["Model M1"]
    B --> C2["Model M2"]
    B --> C3["Model M3"]
    B --> C4["Model M4"]
    B --> C5["Model M5"]
    C1 --> D["Four-Class Prediction"]
    C2 --> D
    C3 --> D
    C4 --> D
    C5 --> D
    D --> E["Comparative Evaluation"]
```

### Model Comparison

| Model | Configuration | Purpose |
|---|---|---|
| M1 | Deep Learning Model 1 | Baseline experiment |
| M2 | Deep Learning Model 2 | Comparative experiment |
| M3 | Deep Learning Model 3 | Comparative experiment |
| M4 | Deep Learning Model 4 | Comparative experiment |
| M5 | Deep Learning Model 5 | Comparative experiment |

*The exact architecture names and layer configurations will be documented according to the final experimental implementation.*

### Training Configuration

| Parameter | Configuration |
|---|---|
| Number of models | 5 |
| Maximum training epochs | 1,000 |
| Classification output | 4 classes |
| Data normalization | Applied |
| Training split | 70% |
| Validation split | 15% |
| Testing split | 15% |
| Data partitioning | Patient-level |

## 5. Classification and Evaluation

The framework evaluates the capability of each model to distinguish the four electrophysiological classes.

The evaluation stage focuses on:

- Accuracy
- Precision
- Recall (Sensitivity)
- Specificity
- F1-score
- Confusion matrix
- Class-wise classification performance

### Classification Workflow

```mermaid
flowchart TD
    A["Trained Deep Learning Model"] --> B["EMG Signal Input"]
    B --> C["Feature Representation"]
    C --> D["Classification Layer"]
    D --> E["Predicted Class"]
    E --> F["Ground Truth Comparison"]
    F --> G["Confusion Matrix"]
    F --> H["Performance Metrics"]
    G --> I["Model Comparison"]
    H --> I
```

### Confusion Matrix

A confusion matrix is used to evaluate the classification performance across all four classes.



*The actual numerical results will be populated from the final testing experiments.*


<p align="center">
  <strong>Biomedical Signal Processing | Electrophysiology | Deep Learning | EMG Classification</strong>
</p>
