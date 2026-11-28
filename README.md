# -DeOldify-Pro-Enhanced-Colorization-main-containing-all-the-tasks
# 🎨 AI-Based Historical Image Colorization System
### DeOldify Pro – Enhanced AI Colorization Pipeline with Six Experimental Extensions

## 📌 Project Overview

The **AI-Based Historical Image Colorization System** is a deep learning-based application designed to transform black-and-white and grayscale photographs into visually appealing color images.

The project uses the **DeOldify deep learning framework** as its primary colorization engine and enhances the output through image preprocessing, ensemble learning, LAB color-space blending, face-aware skin correction, and color grading.

In addition to the main colorization pipeline, the project incorporates six experimental AI-based extensions that explore different approaches to image colorization, including semantic segmentation, user-guided color hints, scene understanding, historical era detection, cross-domain image processing, and period-aware colorization.

The application provides an interactive interface built using **Gradio**, allowing users to upload images, configure processing parameters, generate colorized outputs, and compare different colorization methods.

## 🎯 Project Objectives

- To restore color to historical black-and-white photographs using artificial intelligence.
- To develop an enhanced image colorization pipeline using deep learning.
- To improve colorization quality through preprocessing and image enhancement techniques.
- To preserve original image structure, luminance, and important visual details.
- To explore object-aware, scene-aware, and historical period-based colorization.
- To provide multiple colorization approaches through a single interactive application.
- To evaluate and compare colorization outputs using image quality metrics.

## ✨ Key Features

### 1. DeOldify Pro – Main Colorization Pipeline

The primary module uses two pretrained DeOldify models:

- **Artistic Model:** Suitable for portraits, faces, and artistic colorization.
- **Stable Model:** Suitable for objects, buildings, and general photographs.
- **Ensemble Mode:** Combines both model outputs to produce an enhanced colorized result.

Additional image enhancement features include:

- Image denoising.
- Adaptive contrast enhancement (CLAHE).
- Image upscaling.
- LAB luminance restoration.
- Face-aware skin-tone correction.
- Temperature adjustment.
- Vibrance control.
- Shadow lifting.
- Output sharpening.

### 2. Six Experimental AI Extensions

**Task 1 – Real-Time Multi-Object Colorization**

Uses semantic segmentation to identify different objects and apply suitable color schemes.

Supported object categories include:
- Vehicles
- Trees and plants
- Grass and fields
- Buildings
- Sky
- Roads and ground
- Water
- People
- Mountains and rocks
- Other objects

Supports image, video, and webcam-based processing.

**Task 2 – Conditional Colorization Using Color Hints**

Allows users to guide the colorization process by providing color hints.

Features include:
- Manual color selection.
- Point-based color hints.
- Rectangle-based color hints.
- Automatic colorization without hints.
- User-controlled color guidance.

**Task 3 – Context-Aware Scene Colorization**

Uses scene-specific training to generate colors based on the visual context of an image.

Supports different scene categories and includes automatic scene detection to select or blend suitable scene-specific colorization outputs.

**Task 4 – Time-Based Historical Era Colorization**

Explores historical era-based colorization.

The model works with different historical periods and includes automatic era detection to select an appropriate colorization style.

**Task 5 – Cross-Domain Image Colorization**

Explores colorization across different image domains.

The module supports:
- Photographs.
- Pencil sketches.
- Infrared images.

It includes domain-specific image preprocessing and normalization to prepare different input types for the colorization model.

**Task 6 – Period-Aware Historical Colorization**

Uses historical period-specific training to generate colorized images based on a selected time period.

Supported periods:
- 1900s–1910s
- 1920s
- 1930s
- WWII–1940s
- 1950s

Users can select a historical period and compare colorization results generated using different period-specific models.

### 3. Experiment Lab

The Experiment Lab provides a comparison environment for evaluating the different colorization approaches.

The implemented evaluation metrics include:

| Metric | Purpose |
|---|---|
| Colorfulness | Measures the richness of generated colors. |
| Saturation | Measures the intensity of colors. |
| SSIM | Evaluates structural similarity. |
| Edge Preservation | Measures preservation of important image boundaries. |
| Skin Naturalness | Estimates the natural appearance of skin tones. |
| Processing Time | Measures the time taken for colorization. |

The lab compares the main DeOldify models and the six experimental extensions.

## 🛠️ Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Deep Learning | PyTorch |
| Pretrained Models | DeOldify |
| Computer Vision | OpenCV |
| Image Processing | PIL (Pillow), NumPy |
| Image Analysis | Scikit-image |
| Neural Network Models | Torchvision |
| AI Model Hosting | Hugging Face Hub |
| Semantic Segmentation | PyTorch-based segmentation models |
| User Interface | Gradio |
| Video Processing | FFmpeg |
| Development Environment | Google Colab |
| Storage | Google Drive |

## ⚙️ System Requirements

**Hardware Requirements**
- GPU-enabled environment recommended.
- Google Colab T4 GPU recommended.
- Sufficient RAM for image processing and model training.
- Internet connection for downloading pretrained models and dependencies.

**Software Requirements**
- Python 3
- Google Colab or a compatible Jupyter environment.
- PyTorch
- Gradio
- OpenCV
- Pillow
- NumPy
- Scikit-image
- Transformers
- FFmpeg

## 🚀 Installation and Execution

### Step 1: Open the Project

Upload `FinalAIProject.ipynb` to Google Colab.

### Step 2: Enable GPU

Navigate to:

Runtime → Change runtime type → T4 GPU → Save.

### Step 3: Install Dependencies

The notebook includes commands to install the required libraries and clone the DeOldify repository.

### Step 4: Download Pretrained Models

The notebook downloads the required DeOldify Artistic and Stable model weights through Hugging Face Hub.

### Step 5: Execute Notebook Cells

Run the notebook cells sequentially to:
1. Install dependencies.
2. Initialize DeOldify.
3. Load pretrained colorization models.
4. Initialize the enhanced image-processing pipeline.
5. Load the six experimental extensions.
6. Initialize the evaluation environment.
7. Launch the Gradio application.

### Step 6: Launch the Application

After initialization, the Gradio interface launches with the following sections:

- DeOldify Pro (Main Project)
- Experiment Lab
- Task 1: Real-Time Multi-Object
- Task 2: Conditional Colorization
- Task 3: Context-Aware Scenes
- Task 4: Time-Based Era
- Task 5: Cross-Domain
- Task 6: Period-Aware

### Step 7: Upload and Colorize

Upload a black-and-white or supported input image, select the required colorization method, adjust the available parameters, and generate the output.

For the experimental extensions that require custom training, upload the corresponding training images and train the model before using its colorization functionality.

## 📂 Project Structure

```text
FinalAIProject/
│
├── FinalAIProject.ipynb
│
├── Main Project/
│   ├── DeOldify Artistic Model
│   ├── DeOldify Stable Model
│   ├── Ensemble Colorization
│   ├── Image Preprocessing
│   ├── LAB Color Blending
│   └── Image Quality Evaluation
│
├── Experimental Tasks/
│   ├── Task 1 - Multi-Object Colorization
│   ├── Task 2 - Conditional Colorization
│   ├── Task 3 - Context-Aware Colorization
│   ├── Task 4 - Era-Based Colorization
│   ├── Task 5 - Cross-Domain Colorization
│   └── Task 6 - Period-Aware Colorization
│
└── Experiment Lab/
    ├── Colorfulness
    ├── Saturation
    ├── SSIM
    ├── Edge Preservation
    ├── Skin Naturalness
    └── Processing Time
```

*Note: The structure above represents the logical organization of the notebook. The modules are implemented as notebook cells rather than separate Python files.*

## 🔄 Methodology

The project follows these major processing stages:

1. **Input Image:** Upload a black-and-white or supported image.
2. **Preprocessing:** Perform image resizing, denoising, normalization, and enhancement where applicable.
3. **AI Colorization:** Process the image using the selected pretrained or trained deep learning model.
4. **Color Enhancement:** Apply LAB blending, color correction, and additional enhancement techniques where supported.
5. **Output Generation:** Generate the final colorized image.
6. **Evaluation:** Compare the output using the implemented image quality metrics.

## 📊 Expected Results

The system is designed to:

- Generate colorized versions of black-and-white photographs.
- Produce different colorization styles using Artistic, Stable, and Ensemble modes.
- Support object-specific and scene-specific colorization experiments.
- Allow user-guided colorization using manual hints.
- Explore historical colorization based on different eras and periods.
- Process photographs, sketches, and infrared images through the cross-domain extension.
- Compare different approaches using quantitative image quality metrics.

The actual output quality depends on the input image, pretrained models, training dataset, and selected parameters.

## ⚠️ Important Notes

- A GPU is recommended for faster processing and model training.
- Internet access is required for downloading dependencies and pretrained weights.
- Some experimental tasks require users to upload their own training datasets.
- Google Drive is used to store datasets and trained checkpoints when mounted successfully.
- Without Google Drive, temporary Colab storage is used, and files may be lost when the session ends.
- The historical period-specific outputs are AI-generated approximations, not verified reconstructions of historically accurate colors.
- The project requires the notebook cells to be executed in the appropriate sequence.

## 🔮 Future Enhancements

- Improve historical color accuracy using larger and more diverse datasets.
- Integrate more advanced deep learning architectures.
- Improve face detection and natural skin-tone preservation.
- Add more historical periods and domain categories.
- Improve real-time video colorization performance.
- Introduce additional evaluation metrics and benchmark datasets.
- Develop a standalone web application with image upload and download functionality.
- Explore deployment through cloud-based GPU infrastructure.

## 🎓 Conclusion

The AI-Based Historical Image Colorization System demonstrates the application of artificial intelligence and deep learning in restoring and enhancing historical photographs.

By combining the DeOldify framework with advanced image-processing techniques and six experimental colorization extensions, the project explores multiple approaches to generating realistic and context-aware colorized images.

The integration of an interactive Gradio interface and an Experiment Lab makes it possible to explore different colorization techniques and evaluate their performance within a unified application.

This project highlights the potential of deep learning, computer vision, and image processing in historical photograph restoration and intelligent visual enhancement.

---

**Project Type:** Artificial Intelligence / Deep Learning / Computer Vision

**Primary Framework:** DeOldify + PyTorch

**Development Environment:** Google Colab

**Interface:** Gradio
