#  accelerated_network_SoC – Collaborator: Donia

This repository showcases my **contributions as a collaborator** on the `accelerated_network_SoC` project: a **CNN-based image classification system** for 24 types of Mars rover instruments.  
The baseline CNN I implemented achieved **90.47% test accuracy** on the dataset.

---

##  My Key Contributions

1. **Data Analysis & Exploration**  
   - Explored the dataset of 24 classes (64×64 grayscale images)  
   - Documented class distribution, sample images, and imbalances  

2. **Model Architecture Design**  
   - Built a **minimal CNN**: 2 Conv layers + 2 Dense layers  
   - Total parameters: **407,832**  
   - Designed for fast training and reproducibility  

3. **Training Pipeline**  
   - Developed `02-Training/train_baseline.py`  
   - Implemented **training with validation** achieving **91% accuracy**  
   - Logged training history for analysis  

4. **Evaluation & Metrics**  
   - Developed `03-Evaluation/evaluate_baseline.py`  
   - Evaluated model on **test set**  
   - Generated **confusion matrix, per-class analysis, and summary reports**  

5. **Documentation & Reproducibility**  
   - Added clear explanations of results, configuration, and scripts  
   - Ensured others can **reproduce training and evaluation** easily  

---

## 📊 Baseline CNN Performance

| Metric                | Result |
|-----------------------|--------|
| Test Accuracy         | 90.47% |
| Model Size            | 1.56 MB |
| Training Time/Epoch   | ~15 seconds |
| Best Class            | apxs cal target (100%) |
| Worst Class           | chemcam cal target (33%) |

---

##  Project Structure (Your Contributions Highlighted)
accelerated_network_SoC/ ├── models/ # Saved models │ ├── baseline/ # minimal_cnn.h5 (90.47% accuracy) │ ├── optimized/ # Future optimized models │ └── transfer_learning/ # Transfer learning models ├── results/ # Evaluation results │ ├── baseline/ # Baseline evaluation │ ├── optimized/ # Future optimized results │ └── comparisons/ # Model comparisons ├── scripts/ # Python scripts │ ├── train_baseline.py # Train minimal CNN │ └── evaluate_baseline.py # Evaluate model ├── utils/ # Utility functions ├── notebooks/ # Jupyter notebooks ├── training/ # Training logs/history ├── evaluation/ # Evaluation metrics ├── config.py # Project configuration └── requirements.txt # Dependencies


> ⚠️ Full dataset not included due to size; small sample images provided for reference.

---

##  Dependencies

- Python 3.10+  
- TensorFlow / Keras  
- NumPy, Matplotlib, Seaborn, PIL  
- See `requirements.txt` for full list

---

## 🚀 Quick Start

```bash
# 1. Activate virtual environment
venv\Scripts\activate   # Windows
source venv/bin/activate  # Linux / Mac

# 2. Install dependencies
pip install -r requirements.txt

# 3. Train baseline model
python 02-Training/train_baseline.py

# 4. Evaluate baseline model
python 03-Evaluation/evaluate_baseline.py

📈 Dataset Statistics (Summary)

Total Classes: 24

Image Size: 64×64 grayscale

Training Images: ~4700

Test Images: 1028

Class Distribution: Highly imbalanced (15 to 1878 samples)

✅ Skills Demonstrated

Python & TensorFlow/Keras

Convolutional Neural Networks (CNNs)

Model training, evaluation, and metrics

Data preprocessing and visualization

Collaborative project workflow
