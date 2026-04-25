# Comparative Analysis of Deep Learning Model Performance for AI-Generated Image Detection
### Case Study: Google Gemini vs. Seedream

## Project Overview
This study evaluates the effectiveness of Deep Learning in distinguishing between authentic photography and AI-generated imagery. The project specifically compares the realism of outputs from **Google Gemini** and **Seedream**.

## Technical Implementation

### **Model Architecture: ResNet50**
The core detection engine utilizes **ResNet50**, a Convolutional Neural Network (CNN) designed for high-performance image classification.

**Residual Learning**: It employs "Skip Connections" to capture intricate deep features at the pixel level without performance degradation.

**Transfer Learning**: We leveraged a pre-trained ResNet50 model and fine-tuned it specifically on our hybrid dataset to specialize in detecting subtle AI artifacts.

### **Data Strategy**
**Hybrid Dataset**: The model was trained on 2,000 images, consisting of a 50/50 split between existing Kaggle data (Cash Bowman) and our custom-generated dataset.
**Training Process**: The model was fine-tuned over **6 epochs** using **Fastai** and **PyTorch** to reach stable convergence.

### **Development Workflow: Vibe Coding**
This project’s technical pipeline was developed through an **AI-assisted development workflow**:
* **Vibe Coding Implementation**: The computational logic, including data allocation and the training pipeline, was architected and executed via **AI Coding Agent**.
* **Human-in-the-loop**: While the code was generated through AI, the strategic parameters—such as the **Data Strategy**, **Parameter Tuning** (6 epochs), and **Model Evaluation criteria**—were manually designed and directed.

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
