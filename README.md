## Dermatology-AI
AJL: Equitable AI for Dermatology Kaggle Competition 

## Table of Contents
- [Project Overview](#project-overview)
- [Methodology](#methodology)
- [Results and Key Findings](#results-and-key-findings)
- [Impact Narrative](#impact-narrative)
- [Next Steps and Future Improvements](#next-steps-and-future-improvements)
- [Total Score](#total-score)
- [Project Milestones and Timeline](#project-milestones-and-timeline)
- [Data Overview](#data-overview)
- [Python Libraries Used](#python-libraries-used)
- [License](#license)
- [Acknowledgements](#acknowledgements)
    
## Project Overview
- Build an ML model in order to classify 21 different skin conditions across diverse skin tones using the database provided by Kaggle, bttai-ajl-2025 folder. The model will be evaluated using weighted average F1 score.
- This project aims to address the disparity in skin treatment of people with darker skin tones in Dermatology AI by training the model on different skin conditions across ranges of skin tones.
- We participated in a Kaggle competition hosted by the Algorithmic Justice League (AJL), an organization dedicated to highlighting the social implications and potential harms of AI. AJL works to increase awareness and advocate for ethical AI practices to help prevent these harms.
- Through this competition, we engaged in hands-on problem-solving, gaining deeper insights into biases in AI and the importance of developing inclusive machine learning models.

### Project Highlights
- A member, Marylyn Uzoukwu, has created the first submission with the Resnet34 model that resulted in an F1 score of 0.03757.
- A member, Izabel Miminoshvili, has submitted a predicitons csv file with a ResNet100 model that resulted in an F1 score of 0.04687.
- A member, Gowri Nanda, has tested the Resnet18 model with the F1 score of 0.001.

## Methodology
-  Before starting on the models, we researched the AJL dataset, investigated the categories of data, and preformed data preprocessing and cleaning. The data preprocessing and cleaning portion included our research and understanding of the data including which categories to keep and use for the model.
-  
Our group approached investigating one image classification model to try to find the model for the best results. We first researched many models and decided to start with implementing the ResNet models, assigning each teammate to build one variant of the model. The ResNet models were chosen as they had many variants of convolutional neural network layers which we could use to compare the accuracy of different models. We achieved results for the ResNet18, ResNet34, and ResNet101 image classification models which respectively contained 18, 34, and 101 layers in the neural network. We then implemented the models in a Jupyter Notebook, ipynb, file to process the data and model. To implement the models in the Jupyter notebook files, we first followed our cleaning and preprocessing stages, utilized PyTorch and Keras to build the original models, and then finetuned and tested the models based on our training and testing dataset. Afterwards, we evaluated the f1 score for evaluating how precise a model is. After initially implementing our models, we worked on debugging issues with our current models and started on implementing data augmentation methods.  

### Setup & Execution
- Members used Google Colab in order to run the models on their devices. The folder, bttai-ajl-2025, provided by Kaggle was uploaded to a shared folder on Google drive, which all team members have access to. To run the project, make sure that the correct paths are provided to gain access to the train.csv and test.csv files.

- For the ResNet18 model, Kaggle was used as the main development tool to build and test the model for the GPU capabilities. The model was built, tested, and ran on the Kaggle website in a notebook. 

### Data Exploration
- The team explored the data by analyzing which columns were available, which datasets and values, how many data points, and the images of the conditions that were provided in the data.

![image](https://github.com/user-attachments/assets/b5422fb6-0e96-43af-ac69-8db844dbd477)

![image](https://github.com/user-attachments/assets/da564dff-9292-4749-ba04-a13b0f538a2e)

![image](https://github.com/user-attachments/assets/8576d03d-a4bf-4537-ae66-520cb14c2619)

![image](https://github.com/user-attachments/assets/97ff730b-3079-4abf-98a0-9ee8ca72c503)

![image](https://github.com/user-attachments/assets/0f5d90bc-b530-4dd4-a565-0c03a1765306)

![image](https://github.com/user-attachments/assets/c9caaa05-9217-4da1-a141-871711eb9c50)

![image](https://github.com/user-attachments/assets/6e3f2b3d-c7cd-411e-900e-62645f103e29)



### Model Development
- We investigated five of the largest and most popular image classification algorithms and models, and we decided to use the ResNet models for image classificaiton. Each group member looked at one variant of the ResNet models and created a corresponding model that calculated predictions for the given data set. 

## Results and Key Findings
The F1 score was used to evaluate the model's performance 
- Resnet18 highest F1 score: 0.00150
- Resnet32 highest F1 score: 0.04107
- Resnet101 highest F1 score: 0.04687

Key Insights: 
- The F1 score improved as the depth of the Resnet architecture increased
- Deeper models like ResNet-101 were better at identifying patterns and distinguishing features in images compared to shallower models like ResNet-18 and ResNet-32.
- Shallow models (ResNet-18) may have difficulties in capturing subtle differences in skin conditions, especially across diverse skin tones.
- Deeper models (ResNet-101) can learn more complex patterns, helping to improve detection and classification accuracy.
- Skin conditions can appear differently on various skin tones, making classification more challenging.
- A deeper model can capture fine details like color variations, texture differences, and lesion shapes, leading to better generalization across different skin tones

Visuals
  ![image](https://github.com/user-attachments/assets/58d25723-a0e4-4210-aedf-e9e5af91b0c7)



## Impact Narrative
The impact of bias within the field of dermatology is distinct and observed through the clear disparity in rates of study, diagnosis, and treatment of people with darker skin tones. In this competition, we are working to address these disparities in the treatment of people with darker skin tones through the employment of AI tools that can be used to classify various skin conditions across color lines. 

We utilized data augmentation techniques to offset some of the hardships that come along with this field of study, such as overfitting and the inability to generalize over unseen data. Particularly in cases in which you have a small data set, as in the case of study of skin conditions in darker skin, these issues are prone to arise due to biased research methods that may occur. Therefore, in our augmentation, we perform techniques such as increasing rotation, zoom, and brightness of the images in the data set to try and offset the model’s propensity to over or underfit. 

Our project has the capacity to correct disparities in the diagnostic capability and treatment of people of diverse skin tones, and our use of data augmentation allows us to improve parity of model performance.


## Next Steps and Future Improvements 
  We were able to show that without further optimization, higher levels of the ResNet models had higher accuracies and scores with predicting images. The ResNet18 model had the lowest accuracy, while the ResNet101 model had the highest. For the future, we aim to focus on one model to optimize it to try to get better results. Additionally, the ResNet image classification model was not the only image classificaiton model that we were planning to use. We also investigated the DenseNet, GoogleNet, AlexNet, and LENet models for image classification which can be possible options to test.
    While our current ResNet models had lower accuracies, the best path would be to try a variety of data augmentation strategies and optimization strategies to improve the model's accuracy. Since the ResNet101 model had the highest, we can aim for optimizing the ResNet101 model using the additional data given by Kaggle. One step we were working on before the competition ended was implementing data agumentation in the ResNet34 model, which was able to slightly increase the accuracy. If we are able to apply data augmentation as well as future testing towards our most accurate model, then it is likely that we can improve the results of our model. 
    If we choose to build and implement models that are alternative to ResNet models, we can also utilize similiar optimization strategies that can improve the accuracy of our model. 
    The first next step is to optimize our highest accuracy model. For further research, we can also try to optimize and adjust the other models with a lower accuracy and compare the optimization strategies with the different models. More research and development is needed to improve the models. 



## Total Score
Our selected ResNet101 model ended up with an F1 score of 0.04687. 

## Project Milestones and Timeline 
- **Milestone 1:** Exploratory Data Analysis
- **Milestone 2:** Data Preprocessing
- **Milestone 3:** Explore Data and Identify Model
- **Milestone 4:** Modeling
- **Milestone 5:** Evaluation
- **Milestone 6:** Report

## Data Overview
- **Training Data:** `train.csv`
- **Testing Data:** `test.csv`
- **Datasets obtained from:** `bttai-ajl-2025`

## Python Libraries Used
- Pandas
- Scikit-learn
- Numpy
- Tensorflow.keras
- OS

## License
Copyright 2025 Marylyn Uzoukwu, Gowri Nanda, Sarah Mammen and Izabel Miminoshvili

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

## Acknowledgements
Thanks to the Break Through Tech (BTT) and the student team TA from BTT, Zening Wang, for their help and guidance with this project.  
Further thanks to the student team Marylyn Uzoukwu, Gowri Nanda, Sarah Mammen and Izabel Miminoshvili.
