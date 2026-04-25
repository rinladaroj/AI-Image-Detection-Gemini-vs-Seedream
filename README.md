# Comparative Analysis of Deep Learning Model Performance for AI-Generated Image Detection
### Case Study: Google Gemini vs. Seedream

## Project Overview
This study evaluates the effectiveness of Deep Learning in distinguishing between authentic photography and AI-generated imagery. The project specifically compares the realism of outputs from **Google Gemini** and **Seedream**.

## Technical Implementation

### **Model Architecture: ResNet50**
We utilized **ResNet50**, a Convolutional Neural Network (CNN) featuring a **Residual Learning architecture (Skip Connections)**.
**Feature Extraction**: The model captures intricate deep features at the pixel level to distinguish subtle synthetic artifacts.
**Transfer Learning**: A pre-trained ResNet50 was fine-tuned specifically on a hybrid dataset to specialize in detecting Gemini and Seedream signatures.

### **Data Strategy**
**Hybrid Dataset**: A total of 2,000 images, consisting of 50% existed Kaggle data (Cash Bowman) and 50% custom-generated images.
**Training Process**: The model was trained over 6 epochs using **Fastai** and **PyTorch**, achieving stable convergence.

---

## Key Results & Insights

### **Model Performance**
**Overall Accuracy**: The model achieved a high performance of **93% accuracy** across all major metrics.

**The "Undetectable" Cases**: 30 images successfully bypassed detection (False Negatives), with Seedream accounting for 22 of these cases compared to Gemini's 8.

### **Realism Comparison**
**Seedream (Complex Realism)**: Produces "messy" textures and natural noise (e.g., fur, rough surfaces) that effectively mask AI artifacts, making it harder to detect.

**Gemini (Hyper-Realistic Perfection)**: Outputs often appear "too clean" with unnatural sharpness or invisible **SynthID watermarks**, providing stronger AI signals for the detector.

**Primary Blind Spot**: Photorealistic animal textures (e.g., tiger stripes, elephant skin) represent the highest false negative rates due to their high natural entropy.

---

## Academic Context
* **Institution:** Fudan University
* **Course:** Intro to Computer Science (Fall 2026)
* **Instructor**: Dr. XU, Hui (徐輝)
* **Authors:** Rinlada Rojchnaphakul & Napakpabha Lertapirangsi
