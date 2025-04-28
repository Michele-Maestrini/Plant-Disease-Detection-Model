**Plant Disease Detection using Few-Shot Learning with Siamese Networks, Triplet Loss & Optimized Transfer Learning**
---
To ensure sustainable agriculture by mitigating crop losses, requires effective detection of plant pathogens, particularly in remote areas with limited resources. Traditional deep learning models, which demand extensive datasets and computational power, are unsuitable for deployment on IoT devices like mobile phones.

The aim of this project is to develop a model that is efficient and capable of producing high levels of accuracy in plant disease detection, despite being constrained by low computational resources and limited data. To this end, the dataset that will be used to investigate if it is possible to create such a model is  [PlantVillage](https://www.kaggle.com/datasets/emmarex/plantdisease), which contains 20,638 images that have been taken in a controlled environment, namely, plants photographed with good lighting possessing minimal noise/interference from unwanted intrusions. Thus the goal is to obtain a reasonable level of predictive accuracy that suggests that the model can distinguish between whether a plant is healthy or not and have the possibility of not being restricted to the controlled conditions.

The ultimate objective is to create a scalable solution that bridges the gap between real-world usability and advanced detection techniques. By leveraging Few-Shot Learning (FSL), this project hopes to provide a robust approach to plant disease detection, focusing on models optimized for IoT platforms.

Key techniques include:

* Siamese Networks with Triplet Loss for efficient comparison-based learning.
* Random Search and Bayesian Optimization for hyperparameter-tuning.
* FSL within a 2-way, 5-shot framework to perform well on limited datasets.

Two stages will be implemented to develop two models:

**Stage 1 - Baseline Model (BLM)**: A foundational transfer learning model that will harness random search to obtain the optimal combination of hyperparameters. The results will provide the initial architectural conditions that will be placed on the next stage model development.

**Stage 2 - Few-Shot Learning Model (FSLM)**: Again a foundational transfer learning model will leverage the following advance techniques:
* Training the network using a Siamese Network setup with a triplet loss function that embraces the hyperparameters that were optimally generated in the previous stage.
* Hyperparameter-tuning using Bayesian optimization. The input for exploration/exploitation will come from three notable hyperparameters that are specific to Bayesian optimization and a component pertaining to the regularizer.
* Testing using a FSL environment.

# Gaining Access to the Implementation

This repository contains the `Plant_Disease_Detection_Model_Project.ipynb` notebook and supporting files. Below are multiple ways to download and run the notebook without needing access to Google Drive.

## 1. Clone the Repository

```bash
git clone https://github.com/Michele-Maestrini/Plant-Disease-Detection-Model.git
cd Plant-Disease-Detection-Model
```

The notebook `Plant_Disease_Detection_Model_Project.ipynb` will be in the project folder.

## 2. Download via Browser

1. Navigate to the repository on GitHub:  
   `https://github.com/Michele-Maestrini/Plant-Disease-Detection-Model`  
2. Click on `Plant_Disease_Detection_Model_Project.ipynb`.  
3. Click **Raw**, then right-click and select **Save As…** to download the file locally.

## 3. Download as ZIP

1. On the repository main page, click **Code** → **Download ZIP**.  
2. Unzip the downloaded archive:  
   ```bash
   unzip Plant-Disease-Detection-Model-main.zip
   cd Plant-Disease-Detection-Model-main
   ```

## 4. Open in Google Colab (via Badge)

Add this badge to your own fork or clone of the repo to enable one-click Colab access:

```markdown
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Michele-Maestrini/Plant-Disease-Detection-Model/blob/main/Plant_Disease_Detection_Model_Project.ipynb)
```

## 5. Requirements

- Python 3.7+  
- TensorFlow, Keras, OpenCV, and other dependencies listed in the notebook.  

You can install the Python dependencies with:

```bash
pip install -r requirements.txt
```

---

Repository maintained by Michele Maestrini.

