# DeepFake Detection Model

This project involves building a deep learning model using the InceptionV3 architecture to classify real and fake videos by detecting faces within them. The model is trained to identify whether a given face belongs to a real or fake video.

## Project Overview

The project involves the following steps:

### Dataset Preparation: 
Extract faces from the frames of videos provided in the train_sample_videos directory.Each video is processed to extract up to 8 frames with faces detected, and the faces are saved into two folders: fake and true, based on the labels provided in the metadata file.

### Model Training:

The InceptionV3 model (pre-trained on ImageNet) is used as the base model, with some layers unfrozen for fine-tuning.
Additional fully connected layers are added to increase model complexity and improve accuracy.
The model is trained on the extracted face images to classify them into real or fake categories.

### Model Evaluation:

The model is evaluated using several classification algorithms: SVM, Random Forest, KNN, Naive Bayes, Decision Trees, and Logistic Regression.

### Technologies Used
1) Python
2) OpenCV for video and face detection.
3) Dlib for face detection.
4) TensorFlow for model training.
5) Keras for neural network construction.
6) TQDM for progress visualization.

### Model Results

| Model               | Accuracy    |
| :-----------------: | :---------: |
| InceptionV3         | 97%         |
| SVM                 | 86.19%      |
| Random Forest       | 88.52%      |
| KNN                 | 91.01%      |
| Naive Bayes         | 69.55%      |
| Decision Trees      | 81.53%      |
| Logistic Regression | 87.85%      |


## License

This project is licensed under the MIT License - see the LICENSE file for details.
