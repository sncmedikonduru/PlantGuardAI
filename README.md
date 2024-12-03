# PlantGuardAI Using Focal Models, Q-Metrics, and Synergistic Diversity (SQ)

## Overview

PlantGuardAI is an innovative AI-powered tool designed to detect plant diseases and nutrient deficiencies. By simply uploading an image of a leaf, our advanced algorithms analyze the visual patterns and identify potential issues, providing actionable insights to help maintain plant health. By leveraging **Focal Models**, **Q-Diversity Metrics**, and the novel **Synergistic Diversity (SQ)** metric, it enhances classification accuracy and robustness for plant leaf disease detection. The **SQ framework** optimizes ensemble diversity by capturing complementary capabilities among models, consistently outperforming traditional diversity metrics.

---

## Key Features

- **Focal Model-Based Diversity**:
  - Identifies challenging samples where individual models underperform.
  - Ensures ensemble members complement each other effectively.

- **Q-Diversity Metrics**:
  - **Cohen’s Kappa (CK)**: Measures agreement between models.
  - **Binary Disagreement (BD)**: Quantifies disagreements among ensemble members.
  - **Kohavi-Wolpert Variance (KW)**: Assesses variability across ensemble predictions.
  - **Generalized Diversity (GD)**: Evaluates overall diversity in ensemble errors.

- **Synergistic Diversity (SQ)**:
  - Integrates focal and non-focal model relationships.
  - Balances disagreement (diversity) and agreement (synergy) for optimal ensemble selection.

---

## Methodology

1. **Base Model Training**:
   - Train diverse deep learning models including DenseNet, EfficientNet, ResNet, and Vision Transformers (ViTs) on plant leaf image datasets.

2. **Diversity Metrics**:
   - Calculate Q-Diversity metrics (CK, BD, KW, GD) to assess pairwise and ensemble-wide diversity.

3. **Synergistic Diversity (SQ)**:
   - Compute SQ scores using:
     - Disagreement between focal and non-focal models.
     - Agreement among non-focal models.

4. **Ensemble Selection**:
   - Select high-performing ensembles based on SQ scores.
   - Optimize model combinations to maximize synergy and predictive accuracy.

5. **Evaluation**:
   - Validate ensemble performance on the PlantVillage dataset.
   - Compare SQ-based ensembles with traditional Q-metric-based ensembles.

---

## Results

- **Accuracy**: Achieved **99.80% accuracy** with SQ-based ensembles, outperforming Q-metric ensembles.
- **Correlation Analysis**:
  - SQ metric exhibited a **strong positive correlation** (0.549) with ensemble accuracy.
  - Traditional metrics (CK, BD, KW) showed weaker or negative correlations with accuracy.
- **Ensemble Robustness**:
  - SQ-based ensembles effectively corrected misclassifications from individual models.


