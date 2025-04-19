# 👗 Fashion Recommendation System
This project recommends similar fashion items based on a user-uploaded image. It uses a pre-trained ResNet50 model to extract features from the image and compares them with a dataset using Euclidean distance. The top 5 visually similar fashion items are then returned as recommendations.
## Table of Contents

-  [Project Overview](#project-overview)  
-  [System work Flow](#system-work-flow-diagram)  
-  [How it Works](#how-it-works)  
-  [Built With](#built-with)
-  [Output](#output)
  
##  Project Overview

The Fashion Recommendation System is a deep learning-based project designed to suggest visually similar fashion items based on an uploaded image. By leveraging the power of ResNet50 for feature extraction and using Euclidean distance for similarity comparison, the system can identify and return the top 5 most similar fashion products from the dataset. This approach offers a more intuitive and image-driven shopping experience, eliminating the need for keyword-based searches.

## System Work Flow Diagram

1. **Dataset Loading**  
   Load the kaggle dataset to the system which contains fashion item images which serve as the base for comparison.You can download the dataset [here.](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)

2. **Feature Extraction**  
   Each image from the dataset is passed through a pre-trained ResNet50 model to extract deep feature representations.

3. **Feature Storage**  
   The extracted features are stored in a file (e.g., `.npy` or `.pkl`) for faster retrieval during comparison.

4. **User Image Upload**  
   The user uploads an image of a fashion item they want similar recommendations for.

5. **Query Feature Extraction**  
   The uploaded image is also passed through the ResNet50 model to extract its feature vector.

6. **Similarity Comparison using Euclidean Distance**  
   The query image's features are compared with the stored dataset features using Euclidean distance.

7. **Top 5 Similar Image Recommendations**  
   The 5 images with the smallest distances to the query are returned as the most visually similar items.
   
**Work Flow Diagram** is given below:
![image alt](https://github.com/Sushree-ritu23/Fashion-Recommendation-System/blob/9bbc4be5544a96fdda975982ef871ed7d7645716/fashionrecommflow.png)

## How it Works
1. The user uploads a fashion image as a query.
2. The image is passed through a pre-trained ResNet50 model to extract deep features.
3. The system uses pre-extracted features of dataset images stored earlier.
4. Euclidean distance is calculated between the query and dataset features.
5. The top 5 images with the smallest distances are returned as recommendations.


##  Built With

**Libraries & Tools**  
- **NumPy** – For numerical operations and handling feature vectors  
- **Pillow** – For image processing and format handling  
- **OpenCV** – For reading, resizing, and manipulating images  
- **Scikit-learn** – For preprocessing and utility functions  
- **tqdm** – For progress visualization during feature extraction

**Model & Technique**  
- **ResNet50** – Pre-trained CNN model used for extracting image features  
- **Euclidean Distance** – Used to compute similarity between the query and dataset images

**Framework**  
- **TensorFlow & Keras** – For deep learning operations and model management  
- **Streamlit** – For building the user-friendly web interface

## Output
![video alt](
