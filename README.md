
---
# 🧾 Animal Classification – Image-Based Deep Learning Model
---

_Identifying animal species from images using Convolutional Neural Networks (CNNs), data augmentation, and transfer learning for robust classification._

---

## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
- <a href="#dashboard">Graphs/Plots</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#author--contact">Author & Contact</a>

---
<h2><a class="anchor" id="overview"></a>Overview</h2>

This project classifies animals based on image inputs using a deep learning pipeline built with TensorFlow and Keras. It leverages transfer learning with pre-trained models to achieve high accuracy across multiple species, and includes visualizations for performance metrics and prediction confidence

---
<h2><a class="anchor" id="business-problem"></a>Project Problem</h2>

Accurate animal classification is essential for wildlife monitoring, conservation, and educational tools. This project aims to:
- Automate species identification from images
- Reduce manual effort in ecological surveys
- Improve classification accuracy across diverse animal categories
- Enable real-time prediction for deployment in mobile/web apps

---
<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- Image dataset stored in /data/ folder with subfolders per class (e.g., lion, elephant, zebra)
- Includes training, validation, and test sets
- Augmented using rotation, zoom, flip, and brightness adjustments

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- Python (TensorFlow, Keras, OpenCV, Matplotlib)
- Google Colab (GPU acceleration)
- GitHub
- Streamlit (for deployment)

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
animal_classification/
│
├── README.md
├── .gitignore
├── requirements.txt
├── Classification of animals.pdf
│
├── notebooks/                                # Jupyter notebooks
│   ├── exploratory_data_analysis.ipynb
│   ├── animal-img-clsf.ipynb
│
├── summery/                  
│   ├── animal_classifier_model.pkl
│   └──classification_report.txt
│
├── Outputs/                  # visuals file
│   └── airborne.png
│    └── aquatic.png
```

---
<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

- Removed corrupted or mislabeled images
- Resized all images to 224x224 pixels
- Applied data augmentation to balance classes
- Encoded labels and split into train/val/test sets

---
<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

**Class Distribution:**
- 10 animal classes with varying image counts
- Balanced using augmentation for minority classes

**Image Quality Checks:**
- Verified resolution consistency
- Removed grayscale and low-contrast images

**Sample Visuals:**
- Grid plots of sample images per class
- Distribution bar chart of image counts

---
<h2><a class="anchor" id="research-questions--key-findings"></a>Research Questions & Key Findings</h2>

- Model Accuracy: Achieved 94.2% accuracy on test set using ResNet50
- Misclassifications: Most confusion between tiger vs. leopard due to similar patterns
- Augmentation Impact: Improved accuracy by 7.5% on minority classes
- Confidence Scores: Average prediction confidence = 0.91
- Real-Time Prediction: Streamlit app delivers <1s prediction latency

---
<h2><a class="anchor" id="dashboard"></a>Graphs/Plots</h2>

![Aquatic_Animal graphs](https://github.com/SBanditaDas/Real-Time-Image-Classification-of-Animals/blob/main/aquatic.png)
![Airborne_Animal graphs](https://github.com/SBanditaDas/Real-Time-Image-Classification-of-Animals/blob/main/airborne.png)
---
<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

1. Clone the repository:
```bash
git clone https://github.com/SBanditaDas/animal-classification.git
```
2. Open and run notebooks:
   - `animal-img-clsf.ipynb`
     
3. View results:
   
> Check - predictions.csv
        - classification_report.txt
  

---
<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

**Sushree Bandita Das**  

  <a href="https://twitter.com/S_Bandita_Das" target="blank">
    <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="S_Bandita_Das" height="30" width="40" />
  </a>
  <a href="http://www.linkedin.com/in/sushree-bandita-das-160651309" target="blank">
    <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="sushree-bandita-das-160651309" height="30" width="40" />
  </a>
  <a href="https://github.com/SBanditaDas" target="blank">
    <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg" alt="SBanditaDas" height="30" width="40" />
  </a>
  <a href="https://www.kaggle.com/dasbanditasushree" target="blank">
    <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/kaggle.svg" alt="dasbanditasushree" height="30" width="40" />
  </a>

</p>
