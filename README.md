# Car-Classification-Project
#### Use CNN to do image classification on 18 most popular cars (2018 models and up) in Indonesia with 90.85% accuracy

### Examples:
<p align="center"> <img src=https://github.com/jsantoso2/Car-Classification-Project/blob/master/Screenshots/demo-1.JPG width="600"></p>
<p align="center">Demo for Images<p align="center">

### Dataset
- Datasource: https://garasi.id/
- ~7k Training images from 18 different class of cars
- ~2k Testing Images from 18 different class of cars
- List of Cars Models (2018 models and up): 
Daihatsu Ayla, Daihatsu Sigra, Daihatsu Terios, Daihatsu Xenia, Honda BR-V, Honda Brio, Honda CR-V, Honda HR-V, Mitsubishi Pajero Sport, Mitsubishi Xpander, Suzuki Ertiga, Toyota Agya, Toyota Avanza, Toyota Calya, Toyota Fortuner, Toyota Kijang Innova, Toyota Rush, Toyota Yaris

### Tools/Framework Used
- Webscraping: BeautifulSoup, Selenium
- ML model: ResNet50, VGG16, InceptionV3, MobilenetV2
- Evaluation of ML models & Experiment Tracking: Weights and Biases (https://github.com/Cartucho/mAP)
- Data Cleaning/Manipulation: Python

### Procedure
- Web Scrape car exterior images from https://garasi.id/
- Preprocess data and convert labels into appropriate format
- Train and Evaluate on 4 base models (ResNet50, VGG16, InceptionV3, MobilenetV2)
- Pick best model

### Results
<p align="center"> <img src=https://github.com/jsantoso2/Car-Classification-Project/blob/master/Screenshots/results-3.JPG height="450"></p>
<p align="center">Experiment Tracking: Train Loss, Train Acc, Val Loss, Val Acc<p align="center">
<p align="center"> <img src=https://github.com/jsantoso2/Car-Classification-Project/blob/master/Screenshots/results-1.JPG height="450"></p>
<p align="center">Confusion Matrix for ResNet50<p align="center">
<p align="center"> <img src=https://github.com/jsantoso2/Car-Classification-Project/blob/master/Screenshots/results-2.JPG height="450"></p>
<p align="center">Confusion Matrix for Inception v3<p align="center">

- Test Accuracy
| Model | Test Accuracy | 
|-------|-------------- |
| ResNet50 Base | 90.85% | 
| VGG16 Base | 22.23% | 
| InceptionV3 Base | 88.75% |
| MobileNetV2 Base | 32.40% | 

### Final Notes:
- To see more technical details, please see notes.docx for all my detailed notes
