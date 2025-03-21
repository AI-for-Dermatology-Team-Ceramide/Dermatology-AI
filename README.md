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

### Project Highlights
- A member, Marylyn Uzoukwu, has created the first submission with the Resnet34 model that resulted in an F1 score of 0.03757.
- A member, Izabel Miminoshvili, has submitted a predicitons csv file with a ResNet100 model that resulted in an F1 score of 0.04687.
- A member, Gowri Nanda, worked on the Resnet18 model. 

## Methodology

### Setup & Execution
- Members used Google Colab in order to run the models on their devices. The folder, bttai-ajl-2025, provided by Kaggle was uploaded to a shared folder on Google drive, which all team members have access to. To run the project, make sure that the correct paths are provided to gain access to the train.csv and test.csv files. 

### Data Exploration
- The team explored the data by analyzing which columns were available, which datasets and values, how many data points, and the images of the conditions that were provided in the data. 

### Model Development
- We investigated five of the largest and most popular image classification algorithms and models, and we decided to use the ResNet models for image classificaiton. Each group member looked at one variant of the ResNet models and created a corresponding model that calculated predictions for the given data set. 

## Results and Key Findings
- Clearly presents overall model performance using the evaluation metric, along with key insights and appropriate visuals.

## Impact Narrative
- AJL: Describes specific steps taken to address model fairness. Explores the broader potential impact of their work. Incorporates creative storytelling technique(s) to make their work accessible.

- Identifies model limitations, potential improvements, and future directions with strong reasoning. 


## Total Score
* Needs to be added * 

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
