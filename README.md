## Dermatology-AI
AJL: Equitable AI for Dermatology Kaggle Competition 

## Table of Contents
- [Project Overview](#project-overview)
- [Methodology](#methodology)
- [Results and Key Findings](#results-and-key-findings)
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
- A member, Gowri Nanda, worked on the Resnet18 model.

## Methodology

### Setup & Execution
- Members used Google Colab in order to run the models on their devices. The folder, bttai-ajl-2025, provided by Kaggle was uploaded to a shared folder on Google drive, which all team members have access to. To run the project, make sure that the correct paths are provided to gain access to the train.csv and test.csv files. 

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
- The Resnet18 highest F1 score: 0.00150
- The Resnet32 highest F1 score: 0.04107
- The Resnet101 highest F1 score: 0.04687

Key Insights: 
- The F1 score improved as the depth of the Resnet architecture increased
- Deeper models like ResNet-101 were better at identifying patterns and distinguishing features in images compared to shallower models like ResNet-18 and ResNet-32.
- Shallow models (ResNet-18) may have difficulties in capturing subtle differences in skin conditions, especially across diverse skin tones.
- Deeper models (ResNet-101) can learn more complex patterns, helping to improve detection and classification accuracy.
- Skin conditions can appear differently on various skin tones, making classification more challenging.
- A deeper model can capture fine details like color variations, texture differences, and lesion shapes, leading to better generalization across different skin tones

Visuals
  ![image](https://github.com/user-attachments/assets/7639905e-b67a-4744-be3e-5a010485cfbe)
  ![image](https://github.com/user-attachments/assets/58d25723-a0e4-4210-aedf-e9e5af91b0c7)



## Impact Narrative
- AJL: Describes specific steps taken to address model fairness. Explores the broader potential impact of their work. Incorporates creative storytelling technique(s) to make their work accessible.


## Next Steps & Future Improvements 
- Identifies model limitations, potential improvements, and future directions with strong reasoning. 




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
