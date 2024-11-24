# **PCA Image Classification & Compression**

A Python project that demonstrates the power of Principal Component Analysis (PCA) for two major tasks:
1. **Image Classification**: Recognize and classify similar faces based on a dataset.
2. **Image Compression**: Compress color and gray images effectively while retaining visual quality.

---

## **Features**
- **Face Recognition**: Classify faces from the ORL Database of Faces using PCA-based dimensionality reduction.
- **Image Compression**: Apply PCA to compress high-resolution images (both gray and color) while maintaining clarity and minimizing storage.

---

## **Datasets**
### **Face Recognition Dataset**
- **Source**: [ORL Database of Faces](https://www.kaggle.com/kasikrit/att-database-of-faces/download)
- **Description**: Contains gray images of 40 individuals, each with 10 pictures, for a total of 400 images.
- **Application**: Used to demonstrate PCA-based face recognition by extracting principal components from facial features.

### **Image Compression Dataset**
- **Source**: [Unsplash](https://unsplash.com)
- **Description**: Sample images from Unsplash are used to showcase the effectiveness of PCA for compressing both gray and color images.

---

## **How It Works**
### **Face Recognition**
1. **Dataset Preparation**: The ORL dataset is preprocessed to standardize the images.
2. **PCA Application**: PCA reduces the dimensionality of the image data, retaining the most significant features for classification.
3. **Face Classification**: Using the reduced components, the system classifies faces based on their similarity.

### **Image Compression**
1. **Input Images**: High-resolution images are resized and standardized for processing.
2. **PCA Transformation**:
   - For **gray images**: PCA reduces the pixel matrix to principal components.
   - For **color images**: PCA is applied to each color channel (RGB) independently.
3. **Reconstruction**: Images are reconstructed from the principal components, significantly reducing their size while maintaining quality.

---

## **Requirements**
- Python 3.x
- Libraries Need to be installed: NumPy, OpenCV, matplotlib, scikit-learn

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/PCA-Image-Analysis.git
   cd PCA-Image-Analysis
   ```
2. or Download it as a zip file, then extract the folder
3. Run the first block of Jupiter Notebook which will install the required libraries
    - NB: if you have a Windows machine, change the code from `!pip3 ...` to `!pip ...` without the 3 number.
---

## **Usage**
### **Face Recognition**
1. the ORL dataset is already in the `assets` folder.
2. Run the classification jupiter notebook:

### **Image Compression**
1. Optionally place your preferred image in the `assets` folder.
2. change the `img_path` and `save_path` variable to the path of your preferred image. For example, change `img_path` variable
    - From: `img_path = '../assets/dog.jpg'`
    - to: `img_path = '../assets/{your image name with extension name}'`
    - NB: change the `{your image name with extension name}` to the name of your actual image
2. Run the jupiter notebook

---

## **Examples**
### **Face Recognition**
- Check the jupiter notebook.

### **Image Compression**
- check the `dog.jpg` image from the `assets` folder, and its corresponding compressed versions in `processed_images` folder.

---

## **Resources**
- **ORL Database of Faces**: [Download from Kaggle](https://www.kaggle.com/kasikrit/att-database-of-faces/download)
- **Example Images**: [Unsplash](https://unsplash.com)

---

## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## **Contributions**
Contributions are welcome! Feel free to submit issues or pull requests to enhance the project.
