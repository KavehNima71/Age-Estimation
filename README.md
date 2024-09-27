![1](https://github.com/user-attachments/assets/c8cbf9ef-9094-413c-b651-1aceef645dbd)
# Age-Estimation
Age estimation using computer vision is an image processing technique that aims to predict a person's
age from their facial image. This process typically involves the following steps:
1. Face detection: First, the face is identified in the image.
2. Feature extraction: Important facial features such as the shape of the eyes, hair color, mouth, skin
texture, and wrinkles are extracted.
3. Analysis: These features are analyzed by a machine learning model (usually deep neural networks).
4. Age estimation: Based on patterns learned from training data, the model estimates the age.
This technique has various applications in fields such as security, targeted marketing, and humancomputer interaction.

## Our Method
In this study, the ResNet50 model with a final output layer of 100 classes has been utilized for estimating
the ages of individuals. ResNet50 is a powerful architecture in deep learning, capable of extracting
complex features from images. This model effectively mitigates the problem of information loss in deep
networks by employing deep convolutional layers and residual connections.
The final layer of the network is designed for regression, allowing the model to estimate precise age
values based on the extracted features rather than predicting discrete classes. Regression is a statistical
technique that enables models to capture relationships between independent and dependent variables,
facilitating the prediction of continuous values.
For training this model, the UTKFace dataset was used, which includes images of individuals across
various age groups. After preprocessing the images and splitting the data into training and testing sets,
the model was trained to accurately estimate the ages of individuals solely based on their facial images.
The model's performance was evaluated using metrics such as accuracy and mean absolute error. The
results obtained demonstrate the model's high capability in age estimation, making it applicable in
various fields such as security, marketing, and social services.


![IMG_20240925_232414_133](https://github.com/user-attachments/assets/194b5ba1-797b-44da-aaa0-274d884ecd9c)

## Dataset

UTKFace dataset is a large-scale face dataset with long age span (range from 0 to 116 years old). The
dataset consists of over 20,000 face images with annotations of age, gender, and ethnicity. The images
cover large variation in pose, facial expression, illumination, occlusion, resolution, etc. This dataset could
be used on a variety of tasks, e.g., face detection, age estimation, age progression/regression, landmark
localization, etc. For more information and download, please refer to the [UTKFace]( https://susanqq.github.io/UTKFace/)


### Highlights

- consists of 20k+ face images in the wild (only single face in one image)
- provides the correspondingly aligned and cropped faces
- provides the corresponding landmarks (68 points)
- images are labelled by age, gender, and ethnicity


## Exploratory Data Analysis

Exploratory Data Analysis (EDA) of the UTKFace dataset is conducted to examine various features of facial images. This dataset contains facial images labeled with age, gender, and ethnicity, and it is widely used for tasks related to facial recognition, age estimation, and gender classification.

### Key steps in EDA for this dataset

#### 1. Statistical distribution analysis: 
Analyze the distribution of age, the number of images for each gender and ethnicity
![2](https://github.com/user-attachments/assets/c47e148e-b4e5-4197-89e3-7aedf874bc96)




![3](https://github.com/user-attachments/assets/f7b60797-7c5f-45dd-afaf-6f81b38af5b0)




![4](https://github.com/user-attachments/assets/1e597ab6-0e22-47dd-91c4-4d3d72ecd7d2)


![5](https://github.com/user-attachments/assets/585b4870-3d10-4205-b1d9-64679167dfae)

#### 2. Anomaly detection:
Identify mislabeled images or duplicate data and clean the dataset



/content/UTKFace/39_1_20170116174525125.jpg.chip.jpg
/content/UTKFace/61_1_20170109142408075.jpg.chip.jpg
/content/UTKFace/61_1_20170109150557335.jpg.chip.jpg


#### 3. Data visualization: 
Use graphs and charts to visualize the age, ethnic, and gender distributions.


![6](https://github.com/user-attachments/assets/ddb7fb72-a92c-4097-a00c-6cad846f8e9a)



![7](https://github.com/user-attachments/assets/19fb2da8-4723-45f2-a872-59f609de5511)


This analysis provides a deeper understanding of the UTKFace dataset's characteristics and lays the foundation for more complex modeling tasks, such as classification or facial recognition.


### Plotting age histograms in training, validation and testing sets:

![8](https://github.com/user-attachments/assets/5f024999-618a-4455-bf5d-5e00abf0ae48)

This histograms will help ensure that the distributions of age in these sets are similar, indicating a balanced and representative dataset split.
This step is crucial for further analysis or modeling tasks, as it allows you to access and manipulate each set individually.



