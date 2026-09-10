# CNN Face Mask Detection

This project is a **Convolutional Neural Network (CNN) based image classification system** designed to detect whether a person is wearing a face mask or not. The main goal of the project is to use deep learning and computer vision techniques to automatically classify facial images into two categories: **With Mask** and **Without Mask**.

The project uses the **Face Mask Detection Dataset** from Kaggle, which contains **7,553 images** divided into two classes: 3,725 images of people wearing masks and 3,828 images of people without masks. The dataset is organized into separate `with_mask` and `without_mask` folders, making it suitable for supervised image classification.

[Face Mask Detection Dataset – Kaggle](https://www.kaggle.com/datasets/omkargurav/face-mask-dataset?utm_source=chatgpt.com)

The images are first collected from their respective class folders and assigned numerical labels, where `0` represents **with mask** and `1` represents **without mask**. The dataset is then divided into **80% training data and 20% testing data** using a stratified split to maintain the class distribution. A fixed random state of 42 is used to make the data split reproducible.

For preprocessing, the images are resized to **64 × 64 pixels** and converted into numerical arrays. Pixel values are normalized from the original range of 0–255 to a range between **0 and 1**. This preprocessing helps prepare the images for efficient training and allows the CNN to learn visual patterns more effectively.

The project is implemented using **Python, TensorFlow, Keras, NumPy, Matplotlib, and Scikit-learn**. TensorFlow and Keras are used for building and training the CNN model, NumPy is used for numerical data processing, Matplotlib is used for visualizing images and results, and Scikit-learn is used for splitting the dataset.

The final dataset contains **6,042 training images** and **1,511 testing images**, with each image represented as a 64 × 64 RGB image. The trained CNN learns important visual features from the images and uses these features to distinguish between people wearing masks and people without masks.

This project demonstrates the practical application of **deep learning, image preprocessing, CNNs, and binary image classification** in a computer vision problem. It also provides a foundation for developing real-world applications such as automated mask monitoring and safety compliance systems.
